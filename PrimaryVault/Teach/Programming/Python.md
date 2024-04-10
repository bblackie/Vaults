---
tags: programming/python
---

# Basics



## Vritual Environments

### Install virtual env

Enter this command into terminal
```
pip install virtualenv
```


### Create a venv

```
[Win] virtualenv {venv_name}
```
e.g. virtualenv dev
```
[Mac] virtualenv dev
```


Other options:
Specific python version
```python
virtualenv -p <path-to-new-python-installation> <new-venv-name>
# OR 
python -m virtualenv -p C:\Python39\python.exe venv39
```  


Issues:
- The term 'virtualenv' is not recognised
	- solution:  
```
	python -m virtualenv env
```

### Activate venv

[Win] {venv_name}/Scripts/activate
e.g. dev/Scripts/activate

[Mac] source {venv_name}/bin/activate 
e.g. source env/bin/activate

### Gotchas
[Win]
Error: "The file \<filename\> is not digitally signed "
```
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```
### To exit the virtualenv
deactivate

# Dependencies

### How to create a requirements.txt file

Option A:  You have the imports in the code but nothing installed as yet

You can use the following code to generate a requirements.txt file:

```
pip install pipreqs
pipreqs /path/to/project
```

Advantages:
- pip freeze only saves the packages that are installed with pip install in your environment.
- pip freeze saves all packages in the environment including those that you don't use in your current project (if you don't have virtualenv) and;
- sometimes you just need to create requirements.txt for a new project without installing modules.

Option B: You want to create a requirements.txt from the libs you have installed

```
pip freeze > requirements.txt
```

### How to check what libs are installed

```
pip list
```
### How to use a requirements.txt

```
pip install -r requirements.txt
```

# Best practices

### Tips

[6 CLEAN Tips To IMPROVE Your Python Functions](https://www.youtube.com/watch?v=qvSjZ6AKfXQ)
By Indently
Here are 6 clean tips that you can use for improving the readability & the practicality of your functions in Python.




# Error Handling

### Exception groups

https://www.youtube.com/watch?v=jsL1I6g-XJE


# Lessons


[Getting Started with Python on Replit - Tips, Tricks and Examples](https://www.youtube.com/watch?v=VGiCFnyTRRk&t=11s)
Includes:
- creating a website
- screen scraping example
