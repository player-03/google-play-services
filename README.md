# Google Play Services

Provides Google Play Services support for OpenFL. Unlike SempaiGames/extension-googleplayservices-lib, this library uses Gradle.

Currently, this library imports the Google Play Services libraries into your project, but doesn't help you access them.

## Installation

First, clone the repository:

```text
> haxelib git google-play-services https://github.com/player-03/google-play-services.git
```

Next, add it to project.xml:

```xml
<haxelib name="google-play-services" />
```

## Specific libraries

This library allows you to choose which parts of the Google Play Services you want to use. To enable features, pick one or more lines from this list, and add them to your project.xml file:

```xml
<set name="googlePlus" />
<set name="googleAccountLogin" />
<set name="googleActions" />
<set name="googleAddressAPI" />
<set name="googleAppIndexing" />
<set name="googleAppInvites" />
<set name="googleAnalytics" />
<set name="googleAwareness" />
<set name="googleCast" />
<set name="googleCloudMessaging" />
<set name="googleDrive" />
<set name="googleFit" />
<set name="googleLocation" />
<set name="googleMaps" />
<set name="googleMobileAds" />
<set name="googlePlaces" />
<set name="mobileVision" />
<set name="googleNearby" />
<set name="googlePanoramaViewer" />
<set name="googlePlayGameServices" />
<set name="safetyNet" />
<set name="androidPay" />
<set name="androidWear" />
```

You must add these lines above "`<haxelib name="google-play-services" />`," not below.
