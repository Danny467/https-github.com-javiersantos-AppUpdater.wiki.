## Basic Usage
```Java
return new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.AMAZON)
       .start();
```

## Notes
* Your app must be published on Amazon App Store with one production release at least.
* The latest update retrieved by the library will be the latest production one.