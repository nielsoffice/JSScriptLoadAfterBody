# JS Script Load next after body tag
Load JS script on documents after body tag HTML 

```HTML
 <!-- Structure -->
 <html>
  <head></head>
  <body id="app-id">
  
  <div id="parentTag" class="try">
   <p>Demo Content...</p>
  </div>
  
  <script id="app-data">
       
     const docID     = document.body.id = 'app-id';
     const childElem = document.getElementById('app-id');
     const appData   = document.getElementById('app-data');
        
     childElem.insertAdjacentElement('afterend', appData );
        
  </script>
 </body>
 </html>
```

```HTML
<!-- Result -->
<html>
 <head></head>
  <body id="app-id">
  
 <div id="parentTag" class="try">
  <p>Demo Content...</p>
 </div>
 
</body>
  <!-- move JS next after body -->
  <script id="app-data">     
    const docID     = document.body.id = 'app-id';
    const childElem = document.getElementById('app-id');
    const appData   = document.getElementById('app-data');
        
    childElem.insertAdjacentElement('afterend', appData );
  </script>
 </html>
```

```HTML
 <!-- Snippet -->
 <script id="app-data">

  // set ID to boby tag
  const docID = document.body.id = 'app-id';
  
  // set ID to the script tag
  const childElem = document.getElementById('app-id');
   
  // get ID of the script tag
  const appData = document.getElementById('app-data');

  // Use JS function insertAdjacentElement();
  // select the body ID and use param 'afterend' to pull 
  // the script next on the target ID which is body
  // get the target element by ID as second param
  childElem.insertAdjacentElement('afterend', appData );

  </script>
```
