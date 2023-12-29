# Financial Analysis JavaScript 

## Description 
I have been tasked with writing a JavaScript code that analyzes a financial record and calculate each of the following:

The total number of months included in the dataset.

The net total amount of Profit/Losses over the entire period.

The average of the changes in Profit/Losses over the entire period.

Track what the total change in profits is from month to month and then find the average.

(Total/(Number of months - 1))

The greatest increase in profits (date and difference in the amounts) over the entire period.

The greatest decrease in losses (date and difference in the amounts) over the entire period.


## How I Approached this Project

```Pseudocode
// Financial data
let finances = [ ];

// Total number of months
totalMonths = length of finances

// Net total amount of Profit/Losses
total = 0
for i from 0 to totalMonths - 1:
  total += finances[i][1]

// The average of the changes in Profit/Losses 
changes = []
for i from 1 to totalMonths - 1:
  changes.push(finances[i][1] - finances[i - 1][1])
sumChanges = sum of changes
averageChange = sumChanges / (totalMonths - 1)

// Greatest increase and decrease
greatestIncrease = maximum value in changes
greatestDecrease = minimum value in changes

// Corresponding dates for increase and decrease
increaseIndex = index of greatestIncrease in changes + 1
decreaseIndex = index of greatestDecrease in changes + 1

// Financial analysis display
display("Financial Analysis")
display("----------------------------")
display("Total Months:", totalMonths)
display("Total: £", format total as currency)
display("Average Change: £", format averageChange as currency)
display("Greatest Increase in Profits/Losses:", finances[increaseIndex][0], " (£", format greatestIncrease as currency, ")")
display("Greatest Decrease in Profits/Losses:", finances[decreaseIndex][0], " (£", format greatestDecrease as currency, ")")
```


## References
[Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)


## Deployed Project Link 
(https://hwilson-hub.github.io/Horiseon-C-1/)


## License

This project is licensed under the MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to conditions.

View full License: (https://github.com/hwilson-hub/Challenge1-Horiseon/blob/main/LICENSE)

©2023. Haydawn Wilson. All Rights Reserved.
