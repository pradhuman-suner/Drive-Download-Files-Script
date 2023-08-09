# Drive-Download-Files-Script-
A Javascript file to run on drive folder to download all files within folder without zipping 


**
var token = "[Add Here Your Token]";
document.querySelectorAll('[data-id]').forEach( (item) =>  {
  URL = "https://drive.google.com/uc?export=download&id=" + item.getAttribute('data-id') + token ;
  var win = window.open(URL, '_blank');
  win.test = function () {
    
  console.log('New script appended!')
    }
    win.test();
    setTimeout(function () {
         document.querySelector('[type="submit"]').click()
        console.log('New script appended!')
    }, 10);
});
**
