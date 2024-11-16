2024-10-1520:34
Tags:[[Library]]
# pathlib

### Intro Example
```python
from pathlib import path

current_dir= Path('.') #current directory
new_path= current_dir/'some_folder' #Concatinates to create a new path
print(new_path.resolve()) #Shows the path associated with this Path object
```

### Utility 
```python
p = Path(__file__) #current file
p.parent #parent file 

p.exists() #Tells you if path exits in disk
p/= 'something'#appends file to path 
p.mkdir() #creates new directory at given path if path didn't exist

p.parts #shows all content inside path (like ls in linux)

p/= 'text.txt'
p.touch() #creates file at path

with p.open() as file: #opens the file at path
    file.readline()
```

### Looping
```python

for f in my_path.iterdir():
    if f.match('*.txt'): #match works with any glorb style pattern
        print(f)
    
```

>[!note]- Glorb style Patterns in Python
>A glob pattern is used to match filenames or directory names using wildcards. 
>Common Wildcards: 
>1. \* (asterisk): Matches zero or more characters. Example: *.txt matches file.txt, notes.txt, etc.
>2. ? (question mark): Matches exactly one character. Example: file?.txt matches file1.txt, file2.txt (but not file12.txt).
>3. [abc]: Matches any one character inside the brackets. Example: file[123].txt matches file1.txt, file2.txt, or file3.txt. 
>4. [!abc] or [^abc]: Matches any one character NOT inside the brackets. Example: file[!0-9].txt matches fileA.txt (but not file1.txt). 
>5. {a,b,c}: Matches any of the comma-separated patterns inside the braces. Example: file.{txt,md} matches file.txt and file.md.
>Usage Example in Python: from pathlib import Path # List all .txt files in the current directory for file in Path('.').glob('*.txt'): print(file)



---
# References
[Explanation Video](https://www.youtube.com/watch?v=YwhOUyTxXVE&ab_channel=PyCharm%2CaJetBrainsIDE)
[Documentation](https://docs.python.org/3/library/pathlib.html)

