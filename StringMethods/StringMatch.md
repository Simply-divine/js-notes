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
