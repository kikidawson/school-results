# school-results

A school report company would like a program, which finds out how students do on their tests. A string of comma separated values are provided by the school and this is used to build a report.

"Green, Green, Amber, Red, Green" => "Green: 3\nAmber: 1\nRed: 1"
"Green,Dave,Whimsy,Red" => "Green: 1\nRed: 1\nUncounted: 2"

Results can fall into 4 categories: Red, Amber, Green, Uncounted

## Planning

| input | output |
| -------- | --------- |
| "" | "No results given" |
| "," | "No results given" |
| "Green" | "Green: 1" |
| "Amber" | "Amber: 1" |
| "Red" | "Red: 1" |
| "Orange" | "Uncounted: 1" |
| "Green, Green, Amber, Red, Green" | "Green: 3\nAmber: 1\nRed: 1" |
| "Green,Dave,Whimsy,Red" | "Green: 1\nRed: 1\nUncounted: 2" |

- if empty or comma
- return "No results given"
- if not empty or comma
- split string into array by ","
- Count length or array
- count greens, reds and ambers
- anything left over is uncounted.
- return in string e.g. "Green: 3\nAmber: 1\nRed: 1"
