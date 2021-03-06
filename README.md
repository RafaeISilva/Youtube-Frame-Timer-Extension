# Youtube Frame Timer "Extension"
Displays a frame timing tool on speedrun.com's verifying page or in YouTube (must be logged in) so you don't need to open it in another tab.

## Extensions you will need
* [Stylish](https://chrome.google.com/webstore/detail/stylish-custom-themes-for/fjnbnpbmkenffdnngjfgmeleoegfcffe)
* [Custom JavaScript for Websites 2](https://chrome.google.com/webstore/detail/custom-javascript-for-web/ddbjnfjiigjmcpcpkmhogomapikjbjdk)
* [Code Injector (FireFox)](https://addons.mozilla.org/firefox/addon/codeinjector/)

## How to set it up on speedrun.com
**CSS:** Click on the extension -> 3 dots on the top-right corner -> create new style. Copy [this code](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/style_src.css) and paste it there, click on specify and select "URLs matching this regexp" and paste `https://www.speedrun.com/[_a-zA-Z0-9]*/run.+` then click on save.

**JavaScript:**
Click on the extension -> New Regexp -> paste `https://www.speedrun.com/[_a-zA-Z0-9]*/run.+` -> add -> paste [this code](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/main_src.js) and click on the save button at the top-left corner.

## How to set it up on YouTube
**CSS:** Click on the extension -> 3 dots on the top-right corner -> create new style. Copy [this code](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/style_yt.css) and paste it there, click on specify and select "URLs matching this regexp" and paste `https:\/\/www\.youtube\.com\/watch.+` then click on save.

**JavaScript:** Click on the extension -> New Regexp -> paste `https:\/\/www\.youtube\.com\/watch.+` -> add -> paste [this code](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/main_yt.js) and click on the save button at the top-left corner.

## Firefox
Click on the extension and on Add rule, then do the following:

**For speedrun.com:** Paste `https://www.speedrun.com/[_a-zA-Z0-9]*/run.+` on the URL field and paste (downloading and uploading the files works too) [JavaScript](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/main_src.js) && [CSS](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/style_src.css) on It's respective fields

**For YouTube:** `https:\/\/www\.youtube\.com\/watch.+` on the URL field and paste (downloading and uploading the files works too) [JavaScript](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/main_yt.js) && [CSS](https://github.com/RafaeISilva/Youtube-Frame-Timer-Extension/blob/main/style_yt.css) on It's respective fields
