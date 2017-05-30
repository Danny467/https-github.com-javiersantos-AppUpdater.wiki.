### Why AppUpdater doesn't self-update my Android app?
AppUpdater is a tool that let the user know about an app update, but it doesn't offer a mechanism to download and install the update. This is because a Google Play Developer Content policy, it says:

> An app downloaded from Google Play may not modify, replace or update its own APK binary code using any method other than Google Play's update mechanism.

Google Play bans self-updating Android apps, so I suggest you to don't include a mechanism to update your app. AppUpdater has been developed to pass the Google Play Developer Content Policy and, for this reason, the library doesn't offer the possibility to download and install an update.