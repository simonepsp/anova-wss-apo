# Anova APO Web Tool | An unofficial client for your APO 2.0

This (unofficial) web tool that allows you to connect to your APO 2.0 oven. It can detect firmware update events and even push OTA updates to it.

This is a 2-hours project so expect bugs, random code and *dragons* spitting fire on your house [^1].


## Just show me the tool!
✅ The tool can be accessed on github pages: https://simonepsp.github.io/anova-wss-apo/

## How to obtain an access token
A full guide on how to obtain an Anova access token has been posted here by @bogd https://github.com/bogd/anova-oven-api/blob/main/docs/README.md
I've copy pasted it below


### Getting the refresh token

The actual application runs on Firebase, and authenticates via Google's Identity Platform (OAuth, I believe?). So you will need either an access token (which has a limited lifetime before it expires), or the refresh token (which you can exchange for a new access token whenever needed).

1. Using Chrome, connect to [https://oven.anovaculinary.com](https://oven.anovaculinary.com) . Authenticate using whatever mechanism you normally use. 
2. Press F12, and go to `Application > Storage > IndexedDB > firebaseLocalStorageDB > firebaseLocalStorage > value > stsTokenManager > refreshToken`
3. If you are able to copy/paste that token, great! In my case, Chrome did not allow that, so I had to install a third-party extension (IndexedDBEdit). This adds a new tab under F12, so you can easily go to `F12 > IndexedDBEdit > firebaseLocalStorageDB > firebaseLocalStorage` and get the `refreshToken` value from the JSON.
4. While you are here, also get the `apiKey` (it should be the same one for everyone)

## Screenshots
<img width="2974" height="2202" alt="Anova Webtool" src="https://github.com/user-attachments/assets/be75fc8a-f532-4516-aeba-9c7e63c3367d" />

## Disclaimer
This tool is an independent project and is not affiliated with, endorsed by, or supported by Anova Culinary or its parent companies. All trademarks and brand names are the property of their respective owners.

[^1]: Dragons are real dangerous. Beware
