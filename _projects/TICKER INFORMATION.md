---
layout: page
title: TICKER INFORMATION
description: CS50p FINALPROJECT
img: assets/img/ticker_price.png
importance: 4
category: Python
---

# TICKER INFORMATION

#### Video Demo: [here](https://youtu.be/z2xsYft5r74)

#### Description: This program can graphically provide a 30-day period of adjusted closing price of two stocks as a PNG image and textual ticker information.

## USAGE

The way to choose the desired option is with up and down arrows.

## MENU

### Option 1

#### Compare graphically a period of 30 days of adjusted closing price of two actions

In this option, I decided to use regular expressions to continue in the program until the user enters the date as requested. This way, I could separate the entered data into groups and request it in an organized way from `yfinance`. It also verifies the tickers entered because there are many that may be similar, have no information, or do not exist.  
At the end, it generates an image with a `.png` extension.

### Option 2

#### Business Summary

You must enter a ticker for which it will print the company's full name, sector, and a summary. If the ticker does not exist, it will ask for one again. If it exists but has no summary information, it will notify you.

## APPROACH

I chose to use graphs and request data from a third party to process it. Then, I wanted to make it a bit more graphical and implement a small menu. Regular expressions came in handy to verify the data the user enters.  
This project helped me understand how to start a project, value the importance of reading documentation, and consider alternatives because there are multiple approaches to the same problem. It also allowed me to implement the knowledge acquired throughout the course.

### Functions

#### `main()`

Here, in addition to the main part of the program, you will find option 1 of the program.

#### `menu()`

The menu is located here and returns the user's selection.

#### `menu_option2()`

Handles option 2 of the menu and also calls `ticker_validation()` to validate.

#### `ticker_validation()`

Validates the entered ticker and handles possible errors, such as if the ticker does not exist.

#### `date_verification()`

Uses regular expressions and `datetime` to validate the date entered and handle possible errors, such as dates that have not yet passed, dates that are too old, or dates that do not exist. This function calls the function **`date_process()`**.

#### `date_process()`

Takes the date entered and standardizes it. Thus, in `main()`, option 1, you can set the 30-day period to do your processing.

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/estadistico.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/estadistico.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
{% jupyter_notebook jupyter_path %}
{% else %}

<p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}