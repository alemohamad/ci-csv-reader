# CodeIgniter Library: CSVReader

**ci-csv-reader**

## About this library

This CodeIgniter's Library is used to read a CSV file and return an array with its info.

Its usage is recommended for CodeIgniter 2 or greater.

* The original code can be found in [CSVReader](https://github.com/EllisLab/CodeIgniter/wiki/CSVReader) by Pierre-Jean Turpeau.

## Usage

```php
$this->load->library('CSVReader');
$csvData = $this->csvreader->parse_file('Test.csv'); //path to csv file
```

### Accepted CSV Format:

```csv
Title,Text,Date

Title,Some description.,2013-09-28 16:56:09
Another item,"Another description, my friend.",2013-11-13 15:30:41
First title,Description from the item.,2013-12-08 11:33:55
```

### Result:

```
Array(
    [0] => Array(
        [Title] => Title,
        [Text] => Some description.,
        [Date] => 2013-09-28 16:56:09
    )
    [1] => Array(
        [Title] => Another item,
        [Text] => Another description, my friend.,
        [Date] => 2013-11-13 15:30:41
    )
    [2] => Array(
        [Title] => First title,
        [Text] => Description from the item.,
        [Date] => 2013-12-08 11:33:55
    )
)
```

![Ale Mohamad](http://alemohamad.com/github/logo2012am.png)