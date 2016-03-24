## Basic Usage
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

### Notes
No additional notes.