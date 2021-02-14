# Python Variable Changer
Have you ever got tired of your variable names? 
Has debugging your code ever gotten too easy?
Do ever feel confined by programming conventions? 
Are you looking to obfuscate your python code but only kinda?

If you answered yes to any of these questions, you still probably should not use this script. The script changes up your variable names to spice up your python. 

### Requirements

### Installation

This script requires python 3 to run.
It only uses the Python Standard Library so no additional packages need to be installed. 

To install this, copy and paste it to your environment with Python 3. 
*This does not deserve to be a package at this time.*



### Usage
```bash
python enrich.py -f <insert_file_path> 
```
#### Flags
```
$ python3 enrich.py -h
usage: enrich.py [-h] [-r REPLACE] (-i INPUT | -f FILE)

Python Variable Changer Script

optional arguments:
  -h, --help            show this help message and exit
  -r REPLACE, --replace REPLACE
                        Replace file

required named arguments (mutually exlusive):
  -i INPUT, --input INPUT
                        Input file name
  -f FILE, --file FILE  Alternative argument for input file name
```

### Example
#### Before
```python
# example.py
while True:
    a = "how"
    b = "do"
    c = "i"
    d = "make"
    e = "this"
    f = "stop"
    aB = a + b
    cD = c + d
    eF = e + f
    print(aB + cD + eF)
```
```bash 
# -f input filename argument
# -r replace input file with changes (optional) 
python enrich.py -f ../example.py -r True
```
#### After
```python
while True:
    awful_pendulum = "how"
    olden_cable = "do"
    fixed_piano = "i"
    elastic_bull = "make"
    final_nun = "this"
    balmy_kaleidoscope = "stop"
    chief_scarf = awful_pendulum + olden_cable
    filmy_dot = fixed_piano + elastic_bull
    stock_germ = final_nun + balmy_kaleidoscope
    print(chief_scarf + filmy_dot + stock_germ)
```