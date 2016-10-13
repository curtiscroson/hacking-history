# Lessons

## Week 6
1. [The Evolution of Computing](https://theportus.github.io/presentations/usf-dh-history.html)
2. Discussion: Race, Gender, Class, and Computation

## Week 7
1. Python (Using PyCharm)
    1. What are Lists, Dictionaries, Functions, and Objects?
    2. Working with [Data](data/week6/awn_usf_2015.csv).
        1. Change Columns
        2. Replace Endlines
        3. Do Word Count
        4. Save Results

## Week 8
1. Python (Using PyCharm)
    1.  Work with last week's code....
    2.  Clean with Regex
    3.  Output to folder of text files
2.  OpenRefine
    1.  Working with [Dirty Data](data/week8/fl-postcards-img-locs.csv)
3. Excel
    1. Clean text in excel
    2. Do formulae
    3. Pivot Tables
4. Tableau

``` python
import csv

DATA_FILE = 'awn_usf_2015.csv'
CLEAN_FILE = 'awn_usf_2016_clean.csv'
FIELDNAMES = ['title', 'date', 'author', 'edition', 'section', 'column', 'page', 'source', 'text', 'browse_page_next-href', '\ufeffbrowse_page_next', 'link_to_story-href', 'link_to_story']

def readfile(filename):
    raw_data = []
    with open(filename, mode='r', encoding='utf-8') as csvfile:
        csv_reader = csv.DictReader(csvfile)
        for row in csv_reader:
            raw_data.append(row)
    return raw_data

def writefile(filename, filedata):
    with open(filename, mode='w', encoding='utf-8') as csvfile:
        csv_writer = csv.DictWriter(csvfile, FIELDNAMES)
        csv_writer.writeheader()
        for row in filedata:
            csv_writer.writerow(row)

data = readfile(DATA_FILE)

for row in data:
    row['text'] = row['text'].replace('\n', '')

writefile(CLEAN_FILE, data)
```

## Flex Activities
4. Text Analysis. Analyze cleaned text with Overview or Voyant
5. First Steps to Visualization: What is a Visual Essay?