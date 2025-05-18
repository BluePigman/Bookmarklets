# Bookmarklets
Useful bookmarklets. Save the code as a bookmark, and then click it to run. An easy way is to bookmark a random site and then edit the URL with the code.
## X → Nitter
Redirects from X.com (Twitter) to Nitter.net. Useful for seeing replies without an account.

**Code:**
```javascript
javascript:(function(){ 
  var url = window.location.href;  
  var newUrl = url.replace(/^https:\/\/x\.com\//, 'https://nitter.net/');  
  window.location.href = newUrl;
})();
```

## Instagram -> Imginn
Alternate instagram viewer


**Code:**
```javascript
javascript:(function() {  var url = window.location.href;  url = url.replace("instagram.com", "imginn.com");  var match = url.match(/(?:\/p\/|\/reel\/)([^/?]+)/);  if (match) {    var newUrl = `https://imginn.com/p/${match[1]}/`;    window.location.href = newUrl;  } else {    window.location.href = url;  }})();
```

## Reddit -> old.reddit.com
Useful for seeing NSFW content without an account.

**Code:**
```javascript
javascript:(function(){  var url = window.location.href;  if (url.includes('reddit.com')) {    var newUrl = url.replace('www.reddit.com', 'OLD.reddit.com');    window.location.href = newUrl;  }})(); 
```

## Wayback machine
Searches current URL into the Wayback Machine.

**Code:**
```javascript
javascript:(function(){var currentUrl = window.location.href; var prefix = "https://web.archive.org/web/20250000000000*/"; window.location.href = prefix + currentUrl;})();
```
