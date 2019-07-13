
# String Replace
-----------------

```
var str="Upadhyaydhyay";  
document.writeln(str.replace("dhyay","Script"));
document.writeln(str.replace("/dhyay/","Script")); //first match replace
document.writeln(str.replace("/dhyay/g","Script"));//global match
```
# toLowerCase
'''
    str="HARDIk";
    str.toLowerCase();  
'''
# toLocaleLowerCase
&nbsp;
In an earlier section, we had learnt that a string can be easily converted to lowercase letter using toLowerCase() method. While converting the string to lowercase letter the result may vary due to conflicts between different languages. In Western languages the letter 'i' upper cases to letter 'I' while in Turkish the letter 'i' uppercases to dotted letter '?' . To overcome these problems, we can use toLocaleLowerCase() method.
'''
    str="HARDIk";
    str.toLocaleLowerCase();  
'''
# slice 
The JavaScript string slice() method is used to fetch the part of the string and returns the new string. It required to specify the index number as the start and end parameters to fetch the part of the string. The index starts from 0.
```
    string.slice(start,end); 
```
```
var str = "HardikUpadhyay";  
document.writeln(str.slice(2,5)); 
```
Here, we will provide starting index only. In such case, the method fetches the string up to its length.
```
var str = "HardikUpadhyay";  
document.writeln(str.slice(0));   
```
In next example, we will provide negative number as an index. In such case, the method starts fetching from the end of the string.
```
var str = "HardikUpadhyay";  
document.writeln(str.slice(-5)); //starts with -1 index starting from end 
``` 