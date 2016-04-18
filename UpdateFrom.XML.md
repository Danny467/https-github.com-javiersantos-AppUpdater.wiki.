## Basic Usage without changelog / release notes
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.XML)
       .setUpdateXML("https://raw.githubusercontent.com/javiersantos/AppUpdater/master/app/update.xml")
       .start();
```

### Example XML
```xml
<AppUpdater>
  <update>
    <latestVersion>1.2.2</latestVersion>
    <url>https://github.com/javiersantos/AppUpdater/releases</url>
  </update>
</AppUpdater>
```

## Basic Usage with changelog / release notes
```Java
new AppUpdater(this)
       .setUpdateFrom(UpdateFrom.XML)
       .setUpdateXML("https://raw.githubusercontent.com/javiersantos/AppUpdater/master/app/update-changelog.xml")
       .start();
```

### Example XML
```xml
<AppUpdater>
  <update>
    <latestVersion>1.2.2</latestVersion>
    <url>https://github.com/javiersantos/AppUpdater/releases</url>
    <releaseNotes>
- First evolution
- Second evolution
- Bug fixes
    </releaseNotes>
  </update>
</AppUpdater>
```

### Notes
No additional notes.