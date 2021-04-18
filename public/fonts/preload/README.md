## FONTS - PRELOAD

### Problem
When browser downloads the needed resources for displaying the website with custom fonts, it doesn't prioritize this resource enough.
Sometimes you may want display your text asap because it's important for your UX.
In this case you could indicate the browser to preload the font (tell him this is a high prio resource) and swap the font (use a system one until your font is downloaded)

Take into account each browser has a default behavior with font-face (some hide the text until font is loaded or do it during some seconds)

### How to test this?
1. Run the "before" example throttling the network to 3G and check how the website is displayed and how the resources are downloaded
2. Run the "after" example throttling the network to 3G and check how the text is inmediatly displayed while the resources are downloaded and how the font is in the top of download queue

### Resources
* https://developer.mozilla.org/en-US/docs/Web/HTML/Preloading_content
* https://developer.mozilla.org/en-US/docs/Web/CSS/@font-face/font-display
