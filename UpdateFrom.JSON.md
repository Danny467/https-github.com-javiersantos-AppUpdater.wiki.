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
  "latestVersionCode": 10,
  "url": "https://github.com/javiersantos/AppUpdater/releases",
  "releaseNotes": [
    "- First evolution",
    "- Second evolution",
    "- Bug fixes"
  ]
}
```

### Values
`latestVersion`: required.

`latestVersionCode`: optional.

`url`: required.

`releaseNotes`: optional.

### Notes
* If `latestVersionCode` is included in the JSON, `latestVersion` will only be used to display the latest version in the dialog and the `versionCode` will be used to compare the installed and latest update.