# sGUI
**my sGUI** is a program which can produce an `.xlsx file` to execute `Clicker.py`.
It can also import romax reports to organize the damage in `Result.csv`.

Then you can use the interface of lookup.

Let's start!

# PyPI 套件
* beautifulsoup -     `pip install beautifulsoup4`
* tkinter -     `pip install tk`
* mysql-connector -     `pip install mysql-connector-python`
* numpy -     `pip install numpy`
* openpyxl -     `pip install openpyxl`
* pandas -     `pip install pandas`
* PyAutoGUI -     `pip install PyAutoGUI`
* pygame -     `pip install pygame`
* scipy -     `pip install scipy`
* urllib3 -     `pip install urllib3`

# Usage
### First, prepare following files:
1. sGUI.py
2. FillOut.py
3. CombineExcel.py

### Second, check all the paths in code
Recommend：put all the files in the same folder

### Third, ensure the following codes
* paragraph `check_T()` : torque range
 ```py
if (torque<=250 and torque>=10):
  result = 'Ok'
```

* paragraph `check_S()` : speed range
```py
if (speed<=7500 and speed>=100):
  result = 'Ok'   
```

* paragraph `check_start()` : range
```py
if(torque<10 or torque>250 or speed<100 or speed>7500):
  messagebox.showinfo(title=None, message='你在白癡什麼?')
```
### Then, how to use this program?
1. Enter the bearing number and gear number you want.
2. Enter your 
    * torque range
    * speed range
    * temperature
    * duration time 
        in graphic user interface.
4. Click ***start button***
5. Open 
    * `Clicker.py`
    * `test.xlsx`
    * `Romax model`
        to execute Quick Macro
PS. You can find more information in `Clicker.py`
