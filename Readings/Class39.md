## Location

- Benefits and Downfalls of **'getLastLocation()'** Method:

*Benefits:*
1. Quick Retrieval: The getLastLocation() method provides a quick way to obtain the last known location of the device without actively requesting continuous location updates.
2. Battery Efficiency: It minimizes battery usage associated with your app, as it relies on the cached location data without actively polling for a new location.

*Downfalls:*
1. Possibly Outdated: The main downfall is that the obtained location might be outdated if no other location-aware apps have requested location updates recently. This is because the system caches the last known location, and if it hasn't been updated by other apps, it may not reflect the current location.
2. Null Result: The method can return null in situations where location is turned off in device settings, or if the device is new, restored to factory settings, or Google Play services has restarted without an active Fused Location Provider client.

**'getCurrentLocation()'** Method:

*Benefits:*
1. Fresh and Accurate: The getCurrentLocation() method provides a fresher and more accurate location estimate compared to getLastLocation(). It actively computes the location, giving you a more up-to-date position.
2. Consistency: This method is consistent in providing more accurate location information, reducing the risk of relying on potentially outdated data.

*Downfalls:*
Increased Power Consumption: While getCurrentLocation() provides a more accurate location, it can lead to increased power consumption. This is because it may trigger active location computation on the device, especially if a fresh location is not readily available.