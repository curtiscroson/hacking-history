# Code Examples
---

## Week 4

---

Code for the USF World News exercise for [Week 4](plan.md)

Necessary imports
```python
import csv
import re
```

Reading in a CSV
```python
def read_csv(filename, fields):
    """Returns file data as list of dicts

    Args:
        filename (str): name of the file to be loaded
        fields (list): strings specifying column names

    Returns:
        list: dicts containing record data
    """
    records = []
    with open(filename) as readfile:
        # ready the csv dictionary reader
        reader = csv.DictReader(readfile, fieldnames=fields)
        # loop through records and append each
        for record in reader:
            records.append(record)
    return records
```

Scrub a single text
```python
def clean_text(raw_text):
    """Scrubs the text of endlines, editorials, and extra spaces

    Args:
        raw_text (str): text to be scrubbed

    Returns:
        str: cleaned form of the text
    """
    # Remove endlines
    clean_text = raw_text.replace('\n', '')
    # Remove editorial statements
    clean_text = re.sub("\[(.*?)\]", '', clean_text)
    # Remove redundant spaces
    clean_text = re.sub(r'\s+', ' ', clean_text)
    return clean_text
```

Scrub all the texts
```python
def clean_records(records, text_col):
    """Scrubs textual data in specified column of list of dicts

    Args:
        records (list): dicts with raw data
        text_col (str): specifies which dict key corresponds to text data

    Returns:
        list: cleaned dicts
    """
    for record in records:
        raw_text = record[text_col]
        cleaned_text = clean_text(raw_text)
        record[text_col] = cleaned_text
    return records
```

Writing to a text file
```python
def write_txt(text_data, filename):
    """Writes textual data to a specified file

    Args:
        text_data (str): text to be written
        filename (str): name of desired file to write to

    Returns:
        bool: True for success
    """
    with open(filename, 'w+') as writefile:
        writefile.write(text_data)
    return True
```

Write all records to file
```python
def write_records(records, filename_col, text_col):
    """Writes text data from list of records to series of files

    Args:
        records (list): dicts with data to write
        filename_col (str): column containing desired filename
        text_col (str): column containing text data to write

    Returns:
        bool: True for success
    """
    for record in records:
        filename = record[filename_col] + '.txt'
        text_data = record[text_col]
        write_text(text_data, filename)
    return True

```

---
