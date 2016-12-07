# Google Play Services

Provides Google Play Services support for OpenFL 4.1+.

This library lets you import the [Google Play Services](https://developers.google.com/android/guides/overview), and/or [Android Support Libraries](https://developer.android.com/topic/libraries/support-library/features.html). However, it doesn't help you access them.

## Version numbers

By default, this library will use Google Play Services version 9.6.1 and Android Support Library version 24.2.1. You can override these by setting one or both of these variables in your project.xml file:

```xml
<set name="playServicesVersion" value="9.0.0" />
<set name="supportLibraryVersion" value="24.0.0" />
```

This is [discouraged](http://blog.danlew.net/2015/09/09/dont-use-dynamic-versions-for-your-dependencies/), but instead of specifying an exact version, you can add a plus sign to use the latest available version:

```xml
<!-- Use the latest version. -->
<set name="playServicesVersion" value="+" />
<!-- "Pin" the major version to 24 and the minor version to 0, but use the latest patch. -->
<set name="supportLibraryVersion" value="24.0.+" />
```

Note that this will only look at the library versions you downloaded through the Android SDK Manager, so it isn't a completely automatic process.

## Choosing libraries

Instead of importing the entire library, you can choose which parts of the Google Play Services and Android Support Libraries you need. To enable features, pick one or more lines from this list, and add them to your project.xml file:

```xml
<!-- Google Play Services -->
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

<!-- Android Support Libraries -->
<set name="support-compat" />
<set name="support-core-utils" />
<set name="support-core-ui" />
<set name="support-media-compat" />
<set name="support-fragment" />
<set name="cardview-v7" />
<set name="gridlayout-v7" />
<set name="mediarouter-v7" />
<set name="palette-v7" />
<set name="recyclerview-v7" />
<set name="preference-v7" />
```

Feel free to use camelCase, snake_case, or UPPERCASE_WITH_UNDERSCORES instead. OpenFL converts all of those to the same thing.

Note that some of the v7 libraries require API Level 23 or later:

```xml
<android target-sdk-version="23" />
```

## Full libraries

You can also include the entire support-v4 and/or appcompat-v7 libraries:

```xml
<set name="support-v4" />
<set name="appcompat-v7" />
```

However, keep in mind that this will make your APK larger.
