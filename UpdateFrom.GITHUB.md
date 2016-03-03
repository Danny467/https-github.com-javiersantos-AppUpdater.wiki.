## Basic Usage
```Java
return new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.GITHUB)
       .setGitHubUserAndRepo("javiersantos", "AppUpdater")
       .start();
```

### Notes
* You must have one published release (at least) in the provided repository, tagged as X.X.X.X or vX.X.X.X.
* Repo must be public.