 # JS Date (using Moment.js)
 
 refer [here](https://devhints.io/moment) for this topic
 include moment.js in script
 ```
 <script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.24.0/moment.min.js">
 </script>
```

# Date Formatting
```        
<script>
var date = new Date(), //just to notice diff between js date and moment date
        d = moment();

    document.write(date + "<br>");

    console.log(date);
    document.write(d);
    console.log(d.format('DD/MM/YYYY'));
</script>
```