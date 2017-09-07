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
* `Update#getLatestVersionCode()` will be null when using `AppUpdaterUtils`. You should use `Update#getLatestVersion()` instead.