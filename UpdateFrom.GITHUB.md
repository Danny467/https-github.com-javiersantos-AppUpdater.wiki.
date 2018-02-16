## Basic Usage
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.GITHUB)
       .setGitHubUserAndRepo("javiersantos", "AppUpdater")
       .start();
```

### Notes
* You must have one published release (at least) in the provided repository, tagged as X.X.X.X or vX.X.X.X.
* Repo must be public.
* GitHub doesn't support `versionCode`. You should use `UpdateFrom.JSON` or `UpdateFrom.XML` instead.
* `Update#getLatestVersionCode()` will be null when using `AppUpdaterUtils`. You should use `Update#getLatestVersion()` instead.