## Basic Usage
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.FDROID)
       .start();
```

### Notes
* It doesn't support `versionCode`. You should use `UpdateFrom.JSON` or `UpdateFrom.XML` instead.
* `Update#getLatestVersionCode()` will be null when using `AppUpdaterUtils`. You should use `Update#getLatestVersion()` instead.