## Basic Usage
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.AMAZON)
       .start();
```

### Notes
* Your app must be published on Amazon App Store with one production release at least.
* The latest update retrieved by the library will be the latest production one.
* Google Play doesn't support `versionCode`. You should use `UpdateFrom.JSON` or `UpdateFrom.XML` instead.
* `Update#getLatestVersionCode()` will be null when using `AppUpdaterUtils`. You should use `Update#getLatestVersion()` instead.