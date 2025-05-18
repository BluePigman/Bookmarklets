# Bookmarklets
Useful bookmarklets. Save the code as a bookmark, and then click it to run. An easy way to make a bookmarklet is to bookmark any webpage and then edit the bookmark's URL with the code.

## X → Nitter
Redirects from X.com (Twitter) to Nitter.net. View replies without an account.

```javascript
javascript:location=location.href.replace(/^https:\/\/x\.com\//,'https://nitter.net/');
```

## Reddit -> old.reddit.com
View NSFW posts without an account.

```javascript
javascript:location=location.href.replace('www.reddit.com','old.reddit.com');
```

## Wayback Machine
Searches current URL into the Wayback Machine.

```javascript
javascript:location="https://web.archive.org/web/20250000000000*/"+location.href;
```

## Instagram -> Imginn
Alternate instagram viewer

```javascript
javascript:location=location.href.match(/(?:\/p\/|\/reel\/)([^/?]+)/)?`https://imginn.com/p/${location.href.match(/(?:\/p\/|\/reel\/)([^/?]+)/)[1]}/`:location.href.replace("instagram.com","imginn.com");
```
