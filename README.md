# VIX calculator

The purpose of this repository is to to provide an example of using streamlit to the students.

## Introduction

The source code uses Yahoo Finance to get the vix prices.
The data is gotten by using a python library called [yfinance](https://pypi.org/project/yfinance/).

The library enables us to get stock data from Yahoos publicly available APIs.

To read more about yfinance, head to https://aroussi.com/post/python-yahoo-finance

After fetching the data, we calculate whetever today is day when the user should either buy, sell, or do nothing.

This is then presented to the user using [streamlit](https://streamlit.io/)

![Image over the flow of data](./images/diagram.png)

## Getting started

To get started, make sure you have python 3 installed.
Install the required packaged either with conda, or with pip.

### Setup with Conda

Run the command:

```bash
conda env create -f environment.yml
```

### Setup with pip

Run the command:

```bash
python3 -m pip install -r requirements.txt
```

## Running the code

Enter the folder where you have downloaded the code, and open a terminal in the current folder. For a guide, take a look at the following guide: https://www.groovypost.com/howto/open-command-window-terminal-window-specific-folder-windows-mac-linux/


NOTE: In Windows, you might have to use the anaconda prompt instead of the 
command prompt or powershell.

To run the streamlit version of the app, run the command:

If you used conda, you need to enter your environment by doing the following:

```bash
conda activate vix-env
```
## Example output

Normal example:

![Example of how a lack of indicator looks like when presented to the use](https://raw.githubusercontent.com/billimek/vix_trigger/master/images/daily_vix_normal.png)

Sell indicator example:

![Example of how the sell indicator looks like when presented to the use](https://raw.githubusercontent.com/billimek/vix_trigger/master/images/sell_trigger_example.png)
