# Lessons

## Week 6

1. [The Evolution of Computing](https://theportus.github.io/presentations/usf-dh-history.html)
2. Discussion: Race, Gender, Class, and Computation

---

## Week 7

1. Python (Using PyCharm)
    1. What are Lists, Dictionaries, Functions, and Objects?
    2. Working with [Data](data/week6/awn_usf_2015.csv).
        1. Change Columns
        2. Replace Endlines
        3. Do Word Count
        4. Save Results

---

## Week 8

1. Python (Using PyCharm)
    1.  Work with last week's code....
    2.  Clean with Regex
    3.  Output to folder of text files
2.  OpenRefine
    1.  Working with [Dirty Data](data/week8/fl-postcards-img-locs.csv)

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

---

## Week 9

1. Purposes of Visualization: Exploration and Argumentation
2. Discussion: [What is a Visual Essay?](http://viz.wtf/)
3. Working with Tableau
    1. Visualizing Big Data:
        1. [Iraq Dataset](http://www.thePortus.com/open_data/war_diaries/Iraq.xls)
        2. How to create basic charts
        3. How to ask meaningful questions
        4. Droplines, formatting, dashboarding
    2. Visualizing Linked Data: Florida Postcards
        1. [Cards](http://www.thePortus.com/open_data/fl_postcards/Cards.csv)
        2. [Images](http://www.thePortus.com/open_data/fl_postcards/Images.csv)
        3. [Image-Locations](http://www.thePortus.com/open_data/fl_postcards/Image-Locations.csv)
        4. [Image-Subjects](http://www.thePortus.com/open_data/fl_postcards/Image-Subjects.csv)
        5. [Institutions](http://www.thePortus.com/open_data/fl_postcards/Institutions.csv)
        6. [Texts](http://www.thePortus.com/open_data/fl_postcards/Texts.csv)
4. [Designing a Project Workflow](https://sketchboard.io)

**Flex Activity:** Back to Basics with Excel

---


