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