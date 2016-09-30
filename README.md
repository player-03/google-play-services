# Google Play Services

Provides Google Play Services support for OpenFL 4.1+.

This library imports the Google Play Services libraries into your project, but doesn't help you access them.

## Choosing libraries

This library allows you to choose which parts of the Google Play Services you want to use. To enable features, pick one or more lines from this list, and add them to your project.xml file:

```xml
<set name="google-plus" />
<set name="google-account-login" />
<set name="google-actions" />
<set name="google-address-api" />
<set name="google-app-indexing" />
<set name="google-app-invites" />
<set name="google-analytics" />
<set name="google-awareness" />
<set name="google-cast" />
<set name="google-cloud-messaging" />
<set name="google-drive" />
<set name="google-fit" />
<set name="google-location" />
<set name="google-maps" />
<set name="google-mobile-ads" />
<set name="google-places" />
<set name="mobile-vision" />
<set name="google-nearby" />
<set name="google-panorama-viewer" />
<set name="google-play-game-services" />
<set name="safety-net" />
<set name="android-pay" />
<set name="android-wear" />
```

Feel free to use camelCase, snake_case, or UPPERCASE_WITH_UNDERSCORES instead. OpenFL converts all of those to the same thing.

## Support libraries

You can also include support-v4 and/or appcompat-v7:

```xml
<set name="support-v4" />
<set name="appcompat-v7" />
```

Note that appcompat-v7 requires API Level 23 or later:

```xml
<android target-sdk-version="23" />
```
