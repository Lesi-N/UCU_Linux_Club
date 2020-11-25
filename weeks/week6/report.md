### Week 6 Regular Expressions Homework

### This is a template for the report of 21 problems on [this site](http://regextutorials.com/excercise.html).

### Fork this repository, change this file and send us the link for grading.

### We recommend you (re)watch our presentation, and use a [cheatsheet](./cheatsheet.md) while working on the following problems.

### If you are having problems with figuring out the correct solution, skip it for later, and if you are completely lost, use the hints and try to understand them.

---

### Problem 1: Floating point numbers
```
(\d)\.\d+
```
### Problem 2: Years before 1990
```
.+.19[1-8][0-9].
```
### Problem 3: Hexadecimal colors
```
#(\w|\d){6}
```
### Problem 4: Grayscale colors
```
#([a-z0-9]{2}|[A-Z0-9])\1{2,}
```
### Problem 5: Too long lines
```
.{30,}
```
### Problem 6: Remove repeating words
```
(\s[\w-']+)\1
$1
```
### Problem 7: Match HTML tags
```
<[!/]?\w+\s?(\w+)?>
```
### Problem 8: Cut numbers two digits after floating point
```
(\d\.\d{2})\d+
$1
```
### Problem 9: Digit commas formatting
```
(\d)(?=(\d{3})+\b)
$1,
```
### Problem 10: Match lowercase function declarations
```
function(?=\s[a-z])\s\w+.\w?.
```
### Problem 11: Change date formats
```
(\d{4})-(\d{2})-(\d{2})
$3.$2.$1
```
### Problem 12: Validate 24h time format
```
\b([0-1]\d|2[0-3]):[0-5]\d
```
### Problem 13: Validate AM/PM time format
```
\b(0?\d|1[0-2]):[0-5]\d [AP]M
```
### Problem 14: Pascal style to C-style parameters
```
(?<=[\s][a-z]);
```
### Problem 15: Change variable initialization
```
var\s+(\w+)\s+=\s+new\s+((\w|<|>)+)(.+)
$2 $1$3
```
### Problem 16: IPv6 adresses
```
\d{4}:[a-z0-9]{3,4}(:([\d\w]?){4}){4,6}
```
### Problem 17: Validate 32 or 24 bit hexadecimal colors
```
#(([a-f\d]{6})|([a-f\d]{8}))\b
```
### Problem 18: Replace operators with function calls
```
(((\w+)[\.(]\w[)*](\w\d\.\w)?)|(\w\d))\s\+\s(((\w+)[\.(]\w[)*](\w\d\.\w)?)|(\w\d))
Add($1, $6)
```
### Problem 19: Extract query string from URL
```
\?(\w+=.+)
```
### Problem 20: Extract host from URL
```
\b\w{4}://(www\.)?\w+\.com
```
### Problem 21: Strings not containing word
```
^(.(?!chocolate))*$
```
