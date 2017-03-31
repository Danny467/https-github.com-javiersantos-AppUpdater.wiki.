## Basic Usage
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.XML)
       .setUpdateXML("https://raw.githubusercontent.com/javiersantos/AppUpdater/master/app/update.xml")
       .start();
```

#### Example XML
https://raw.githubusercontent.com/javiersantos/AppUpdater/master/app/update.xml

```xml
<AppUpdater>
  <update>
    <latestVersion>1.2.2</latestVersion>
    <url>https://github.com/javiersantos/AppUpdater/releases</url>
  </update>
</AppUpdater>
```

#### Adding release notes
https://raw.githubusercontent.com/javiersantos/AppUpdater/master/app/update-changelog.xml

```xml
<AppUpdater>
  <update>
    <latestVersion>1.2.2</latestVersion>
    <latestVersionCode>10</latestVersionCode>
    <url>https://github.com/javiersantos/AppUpdater/releases</url>
    <releaseNotes>
- First evolution
- Second evolution
- Bug fixes
    </releaseNotes>
  </update>
</AppUpdater>
```

### Values
`latestVersion`: required.

`latestVersionCode`: optional.

`url`: required.

`releaseNotes`: optional.

### Notes
* If `latestVersionCode` is included in the JSON, `latestVersion` will only be used to display the latest version in the dialog and the `versionCode` will be used to compare the installed and latest update.