## Basic Usage
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.JSON)
       .setUpdateJSON("https://raw.githubusercontent.com/javiersantos/AppUpdater/master/app/update-changelog.json")
       .start();
```

#### Example JSON
https://raw.githubusercontent.com/javiersantos/AppUpdater/master/app/update-changelog.json

```json
{
  "latestVersion": "1.2.2",
  "url": "https://github.com/javiersantos/AppUpdater/releases",
  "releaseNotes": [
    "- First evolution",
    "- Second evolution",
    "- Bug fixes"
  ]
}
```

### Notes
No additional notes.