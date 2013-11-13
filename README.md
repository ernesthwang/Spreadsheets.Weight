Spreadsheets.Weight
===================
A simple spreadsheet for tracking your daily weight, with various columns to help you track weight maintenance goals.

![Weight.xlsx Spreadsheet](https://raw.github.com/ernesthwang/Spreadsheets.Weight/master/doc/images/WeightSpreadsheet.png "Weight.xlsx Excel Spreadsheet")

## Features
* Track your weight daily
* Understand trends by tracking your average weight over 7, 30 and 90 day intervals (Daily Moving Average)
* Keep track of your weekly and monthly highs and lows
* Know what your weight is in Pounds/Kilos/Stone

## How to use this spreadsheet

### Initialize the Date Column (Column A)
Column A contains the list of days that you track.  You should enter a row for every day starting with your earliest reading, even if you skip a day.

If today is your first day weighing yourself, start with today's date!  Then fill in the date column for the next 100 days or so.  The easiest way to do this is to enter today's date in cell A3, enter tomorrow's date in cell A4, highlight them both and drag the green square in the lower right-hand corner of the selection downward.

![Excel Drag Handle](https://raw.github.com/ernesthwang/Spreadsheets.Weight/master/doc/images/ExcelCellDragHandle.png "Excel Drag Handle")

If you want to get fancy using formulas, you can enter 
```
=A3+1
```
in cell A4 and then copy/paste the formula in the rest of the A column.  I personally prefer the hard-coded dates.

If you don't get a chance to weight yourself during a specific day, you should either copy the weight from the previous day, or interpolate your approximate weight based on the next time you record.

#### Interpolation
Interpolation for skipped days is preferred to just copying the previous day's data because it can help "smooth the transition" if your weight jumps during those skipped days.  For example, if you went on a business trip for 4 days and you didn't have access to a scale or a gym, you may have gained 2 pounds.  For the three skipped days, you might add 0.5 pounds per day to make it look like you didn't just skyrocket from 180 lbs to 182.

You can get super accurate with your interpolation, but I find it best to just guesstimate what the values should be.  Hopefully, the gaps will be few and far between.

### Set Your Weight
Enter your weight for the day in column B.  The column header is not labeled as Pounds or Kilos, so you can enter what ever value you are used to.  This spreadsheet assumes that you are using Pounds, so if you are entering Kilos, you need to adjust the formula and column header of column K.  I have a column for Stone in there, too.  You'd have to adjust that formula as well.

#### Kilos to Pounds Formula
```
=A3*2.2
```

#### Kilos to Stone Formula
```
=A3*30.8
```
...or just delete the column :)  Who uses stone, really?

## Weight Graph
There's a basic graph that comes with this spreadsheet, but you need to tweak the settings to your personal preferences.

![Weight Graph](https://raw.github.com/ernesthwang/Spreadsheets.Weight/master/doc/images/GraphExample7Years.png "Weight Graph")

There are four lines graphed:
* Daily Weight
* 7 Day Moving Average
* 30 Day Moving Average
* 90 Day Moving Average

I find that the 30 day moving average is the most useful.  Yes, you should be concerned if your weight jumps on a day-to-day basis, but your average weight over the past 30 days is the best indicator on how your weight mantenance goals are coming along.

## Y-Axis Formatting
* The graph is most helpful if you set the Y-Axis (vertical axis) with minimum and maximum values tuned to your weight goals.  The max value should be your heaviest weight plus 5% or so.  The min value should be your realistic target weight minus 5%.  Don't get too far ahead of yourself!  It's better if you set a short term goal and then readjust the graph when you hit it.

![Graph Settings](https://raw.github.com/ernesthwang/Spreadsheets.Weight/master/doc/images/GraphFormatAxisSettings1.png "Graph Settings")


## Tips
* Get a [Fitbit Aria](http://www.fitbit.com/aria) scale!  I have one and it makes tracking your weight a breeze!
* If you don't have access to this spreadsheet, email yourself your daily weight with your smartphone.
* Make sure you adjust your chart to your needs.