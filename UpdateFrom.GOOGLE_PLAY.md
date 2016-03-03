## Basic Usage
```Java
return new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.GOOGLE_PLAY)
       .start();
```

## Notes
* Your app MUST BE published on Google Play with one production release at least.
* Apps with updates that varies by devices are not supported.
* The update retrieved by the library will be the latest production one.