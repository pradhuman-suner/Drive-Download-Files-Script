# Download Files From Google Drive Without Zipping

This repository contains a JavaScript file that allows you to download all files within a Google Drive folder without zipping them. This can be useful when you want to quickly download multiple files from a Google Drive folder without having to create a zip archive.

## How to Use

1. Clone this repository to your local machine or download the JavaScript file (`download.js`) directly.
2. Open your Google Drive folder containing the files you want to download.
3. Obtain your Google Drive API token and replace `[Add Here Your Token]` in the JavaScript code with your actual token.
4. Open the DevTools console in your browser while viewing the Google Drive folder (usually done by pressing `F12` or `Ctrl+Shift+J`).
5. Copy and paste the modified JavaScript code from the `download.js` file into the DevTools console and press `Enter`.

The script will iterate through all the files in the folder and initiate a download for each file individually. This allows you to download files without the need to zip them, making it faster and more convenient for large numbers of files.



# Script 
```js
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


## Disclaimer

Please note that this script relies on Google Drive's web interface and its behavior. Google Drive's web interface may change over time, which could potentially affect the functionality of this script. Additionally, using scripts to interact with websites might violate their terms of use, so use this script responsibly and at your own risk.

## Contributions

Contributions to improve the functionality or usability of this script are welcome. If you encounter any issues or have ideas for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).


