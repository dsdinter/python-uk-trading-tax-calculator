

    Python UK trading tax calculator
    
    Copyright (C) 2015  Robert Carver
    

1) LEGAL BIT

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.
    
    If you copy, modify or redistribute this software you must retain this file. 
    
    Any additional files added must include the header section
    
"""
    Python UK trading tax calculator
    
    Copyright (C) 2015  Robert Carver
    
    You may copy, modify and redistribute this file as allowed in the license agreement 
         but you must retain this header
    
    See README.txt

"""

## Installation
We use a Python venv and install dependencies first.

```
git clone [THIS-REPOSITORY]
python -m venv python-tax-calculator-venv
cd python-tax-calculator-venv/
source bin/activate
pip install beautifulsoup4
pip install pandas
pip install quandl
cd ../python-uk-trading-tax-calculator
```

## Instructions

In Interactive Brokers Account Management, go to Reports/Tax Docs > Activity.
Then set Period to 'Fiscal Year', set Date to whichever year your're creating the report for, Format to 'HTML/Download'.
Place the downloaded file in the program folder and name it `2019_tradeconfirms.html` (you can adjust the name in `example.py`).
Run the file: `python example.py`

This generates a file named `TaxReport.txt` which you can pass to HMRC in your tax return. 
