# DOM traversal

Traversing along DOM is real fun.
Everythimg in DOM is a tree structure. Before getting ahead first take a look at the first code [here](https://github.com/hardikvupadhyay/js-notes/blob/master/DOM/DOMTraversal.html). Note how we traversed through 
```
element.parentNode.lastChild.PreviousSibling  
```
This is a very big problem that we face in Node traversal..
Let's take a look at why this happened..
when we pressed enter after any tag..html modified it and created an another text element to store enter. These can be better understood by understanding how html modifies itself.
When we write this..
```
<div>
<label></label>
<input type="text">
<\div> 

```
HTML considers it this..
```
<div>
<text></text>//to store enter
<label></label>
<text></text>//to store enter
<input type="text">
<text></text>//to store enter
<\div> 

```
And that's why we go to previous sibling of the last child and not the last child..
But wait when we minify this it would be changed..wouldn't it? So whats the solution..
Take a look at [this](https://github.com/hardikvupadhyay/js-notes/blob/master/DOM/DOMTraversalModified.html)
This is where QuerySelector comes to help..
Though we have to give an extra condition..this is the only way I know uptill now..stay there for updates 

