# Power Delete Suite

## Usage

- Go to your [account overview.](https://old.reddit.com/user/me/overview)

- Click on the bookmark you made while focused on the account overview tab. 

- Adjust settings to your prefrences. 


***Firefox***: Open the Hamburger menu> Bookmarks --> Manage Bookmarks --> Right Click on empty space --> Add Bookmark --> Paste the code below into the URL section --> Save --> Done!

***Chromium/Chrome***: Go to `chrome://bookmarks/` --> Right click on empty space --> Add new bookmark --> Paste the code below into the URL section --> Save --> Done!

***Edge***: Press the three dots --> Favorites --> Star with a plus icon --> Right click the new favorite --> Edit --> Paste the code below into the URL section --> Save --> Done!

***Brave***: Go to `chrome://bookmarks` --> Right click on empty space -->  Add new bookmark --> Paste the code below into the URL section --> Save --> Done!

```
javascript:(function(){window.bookmarkver='1.4';var isReddit=document.location.hostname.split('.').slice(-2).join('.')==='reddit.com';var isOverview=!!document.location.href.match(/\/overview\b/i);if(isReddit&&isOverview){var cacheBustUrl='https://raw.githubusercontent.com/carstentrink/PowerDeleteSuite/master/powerdeletesuite.js?'+(new Date().getDate());fetch(cacheBustUrl).then(function(response){return response.text();}).then(function(data){var script=document.createElement('script');script.id='pd-script';script.innerHTML=data;document.getElementsByTagName('head')[0].appendChild(script);}).catch(function(){alert('Error retrieving PowerDeleteSuite from GitHub');});}else if(confirm('This script can only be run from your own user profile on Reddit. Would you like to go there now?')){document.location='https://old.reddit.com/user/me/overview';}else{alert('Please go to your Reddit profile before running this script');}})();
```


 
## all credits to go to 


 https://github.com/j0be/PowerDeleteSuite
 
