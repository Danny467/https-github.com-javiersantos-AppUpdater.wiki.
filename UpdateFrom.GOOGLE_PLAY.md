## Basic Usage
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.GOOGLE_PLAY)
       .start();
```

### Notes
* Your app must be published on Google Play with one production release at least.
* Apps with updates that varies by devices are not supported.
* The latest update retrieved by the library will be the latest production one.
* Google Play doesn't support `versionCode`. You should use `UpdateFrom.JSON` or `UpdateFrom.XML` instead.
* `Update#getLatestVersionCode()` will be null when using `AppUpdaterUtils`. You should use `Update#getLatestVersion()` instead.

ℹ️ Using `UpdateFrom.GOOGLE PLAY` is not recommended as the Google Play website may vary at any time, use [UpdateFrom.XML](https://github.com/javiersantos/AppUpdater/wiki/UpdateFrom.XML) or [UpdateFrom.JSON](https://github.com/javiersantos/AppUpdater/wiki/UpdateFrom.JSON) instead. More info in issue #132.