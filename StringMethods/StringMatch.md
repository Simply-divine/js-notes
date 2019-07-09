# String match #
-------------------------
&nbsp;
## Syntax ##
-------
```
String.match(regex);
```
## Example 1 
```
var str="hardik";
str.match("ardik");
//simple regex match
```
## Example 2
```
var str="Hardik";
str.match(/Hard/g);
//g denotes global match
```

## Example 3
```
var str="Hardik";
str.match(/hard/g);
//case sensitive so no match
```

## Example 4
```
var str="Hardik";
str.match(/hard/gi);
//matches as case insensitive(gi stands for global insensitive)
```
## Example 5
```
var str="Hardik";
str.match(/[a-p]/gi);
//prints all matched in the range
```
## Example 6
```
var str="Hardik";
str.match(/[a-p]/gi);
//prints all matched in the range
```
## Example 7
```
var str="Hardik";
str.match(/[a-p]/);
//prints first matched in the range
```
