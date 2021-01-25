# Shell Data Processing Notes

## Basic Prowershell Commands 
*(that I have used so far)*

1. mkdir - create a new directory.
2. cd - change directory.
3. cd .. - move to previous directory.
4. ls - list all files in the current folder.
5. ni - create new file.

## Git Bash Commands
*(that I have used so far)*

1. Command to read a URL page and return text data and then store it in data.txt file.
```
bash curl "https://www.hymnal.net/en/hymn/h/313" -O "data.txt"
```
2. Command to return \12 in place of ' ' and sort the data in data.txt in numeric, reverse order. This data is then stored in a new file called result.txt.
```
$ tr ' ' '\12' < "data.txt" | sort | uniq -c | sort -nr > "result.txt"
```
- I have used the following URL for data  processing:
``` 
https://www.hymnal.net/en/hymn/h/313
```
3. Commands for Bash preview:
```
$ cat "result.txt"
$ head -5 "result.txt"
$ tail -2 "result.txt"
```
4. Commands for Powershell cat (I did not use these commands yet):
```
Get-Content "result.txt"
gc one.txt -head 2
gc one.txt -tail 2
```

## Links

* [Data file](https://github.com/annie0sc/shell-data-processing/blob/master/data.txt)
* [Results file](https://github.com/annie0sc/shell-data-processing/blob/master/result.txt)