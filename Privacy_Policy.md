# FakeGPS: Privacy Policy

Welcome to the FakeGPS app for Android!

## Overview

FakeGPS is a location spoofing application that allows you to change your device's GPS location for testing and development purposes. This privacy policy explains how our app handles data and the permissions it requires to function properly.

## Data Collection Policy

**I hereby state, to the best of my knowledge and belief, that this app does not collect any personally identifiable information.** All data (app preferences, subscription status, location history, and favorite locations) created by you (the user) is stored locally on your device only, and can be simply erased by clearing the app's data or uninstalling it.

The app does not:
- Collect or transmit your real location data to any servers
- Track your movements or location history across sessions
- Share any data with third parties

While the app does use Google AdMob for displaying advertisements (in the free version), the ad platform may collect certain anonymous data according to Google's privacy policies. You can opt out of personalized advertising through your device settings.

## Local Data Storage

The app stores the following data locally on your device:

1. **Location History**: Records of locations you have spoofed (stored in a local SQLite database)
2. **Favorite Locations**: Any locations you have saved as favorites
3. **Preferences**: Your app settings such as map style, theme preferences, etc.
4. **Subscription Status**: Information about your premium subscription status

All of this data is stored exclusively on your device and is not transmitted to any external servers.

## Explanation of Permissions Requested

The list of permissions required by the app can be found in the AndroidManifest.xml file. Here's an explanation of why each permission is needed:

| Permission | Why it is required |
|------------|-------------------|
| `android.permission.INTERNET` | Required to download map tiles and display advertisements in the free version. |
| `android.permission.ACCESS_NETWORK_STATE` | Allows the app to check internet connectivity status for map and ad loading. |
| `android.permission.ACCESS_FINE_LOCATION` | Required to access your device's actual location (optional) to show on the map. Only used when you choose to show your real location on the map. |
| `android.permission.ACCESS_COARSE_LOCATION` | Used alongside FINE_LOCATION to get approximate location (optional). |
| `android.permission.FOREGROUND_SERVICE` | Enables the location spoofing service to run in the foreground with a notification. |
| `android.permission.FOREGROUND_SERVICE_LOCATION` | Required for Android 10+ to run location-related services in the foreground. |
| `android.permission.ACCESS_MOCK_LOCATION` | The core permission that allows the app to create mock locations. This is deprecated but included for compatibility. |
| `android.permission.POST_NOTIFICATIONS` | Required for Android 13+ to show notifications when location spoofing is active. |
| `android.permission.WRITE_EXTERNAL_STORAGE` and `android.permission.READ_EXTERNAL_STORAGE` | Used for caching map tiles to improve performance and reduce data usage. Limited to Android 12 and below due to scoped storage. |
| `android.permission.WAKE_LOCK` | Allows the app to keep the spoofing service running even when the device screen is off. |

## Google Play Billing

For premium subscriptions, the app uses Google Play Billing. All subscription transactions are handled directly by Google Play and are subject to Google's privacy policy. We do not store any payment information.

## Security Practices

- All location data is stored securely on your device
- No transmission of sensitive data to external servers
- Regular security updates and vulnerability patching

## Changes to This Policy

This privacy policy may be updated from time to time. Any changes will be reflected in the app and in this document.

## Contact Information

If you find any security vulnerability that has been inadvertently caused by the app, or have any questions regarding how the app protects your privacy, please send an email, and I will try to fix it or help you.

Sincerely,

Jan Kopejtko

FakeGPS Developer

j.kopejtko.tech@gmail.com
