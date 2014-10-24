keystokePhonegap
================

This is the precompiled code for a phonegap build of the webapp located here: (https://keystokestorytime.herokuapp.com)Keystoke StoryTime


This app literally does one thing, and one thing only. It loads a brower window on an android device, and then directs the window
to the Keystoke Storytime webapp.

The reasons for twofold: 
1. Simplicity
2. The app doesn't need to be updated because all updates to the website are automatically reflected here.

However there are drawbacks to this approach. The app requires an internet connection (although it would need one anyway
in order to connect to the mongo database), and it wouldn't get App Store approval were it to be ported over to iOS. Apple 
requires new functionality, and this just mimics the browser.


Logic
================

Here's what's goin' on with this bad boy:

```
 <script type="text/javascript">
    app.initialize();
    window.location="http://keystokestorytime.herokuapp.com";
  </script>
```
