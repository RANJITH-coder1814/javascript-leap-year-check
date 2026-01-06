# javascript-leap-year-check
This repository contains a simple JavaScript program to check whether a given year is a **leap year** or **not** using conditional statements.
##  What is a Leap Year?
A year is a leap year if:
- It is divisible by 4  
- But not divisible by 100  
- Unless it is also divisible by 400 

##  Logic Used
- If year % 4 === 0  
- If year % 100 === 0  
- If year % 400 === 0 → Leap Year  
- Else → Not a Leap Year  

```javascript
function isLeap(year) {
    if (year % 4 === 0) {
        if (year % 100 === 0) {
            if (year % 400 === 0) {
                return "Leap year";
            } else {
                return "Not a leap year";
            }
        } else {
            return "Leap year";
        }
    } else {
        return "Not a leap year";
    }
}
