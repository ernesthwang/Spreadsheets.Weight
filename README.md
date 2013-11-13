Spreadsheets.Weight
===================

A simple spreadsheet for tracking your daily weight, along with 7/30/90 day moving averages and max/min values.

![Weight.xlsx Spreadsheet](https://raw.github.com/ernesthwang/Spreadsheets.Weight/master/doc/images/WeightSpreadsheet.png "Weight.xlsx Excel Spreadsheet")


## How to use this spreadsheet

### Set the Dates

Column A contains the list of days that you track.  You should enter a row for every day starting with your earliest reading, even if you skip a day.  If you don't get a chance to weight yourself during a specific day, you can either copy the weight from the previous day, or interpolate your approximate weight based on the next time you record.

If today is your first day weighing yourself, start with today's date!  Then fill in the date column for the next 100 days or so.  The easiest way to do this is to enter today's date in cell A3, enter tomorrow's date in cell A4, highlight them both and drag the black square in the lower right-hand corner of the selection downward.  If you want to get fancy, you can enter 
```
=A3+1
```
in cell A4 and then copy/paste the formula in the rest of the A column.  I personally prefer the hard-coded dates.

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
...or just delete the column :)  Who uses stone, anyway?

## Weight Graph

There's a basic graph that comes with this spreadsheet, but you need to tweak the settings to your personal preferences.

![Weight Graph](https://raw.github.com/ernesthwang/Spreadsheets.Weight/master/doc/images/GraphExample.png "Weight Graph")

There are four lines graphed:
* Daily Weight
* 7 Day Moving Average
* 30 Day Moving Average
* 90 Day Moving Average

I find that the 30 day moving average is the most useful.  Yes, you should be concerned if your weight jumps on a day-to-day basis, but your average weight over the past 30 days is the best indicator on how your weight mantenance goals are coming along.

