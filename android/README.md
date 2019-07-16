<img src="https://bluemixassets.eu-gb.mybluemix.net/api/Products/image/logos/weather.svg?key=[starter-weather]&event=readme-image-view" alt="Weather Logo" width="200px"/>

## Weather
Bluemix Mobile Starter for Weather in Java

[![](https://img.shields.io/badge/bluemix-powered-blue.svg)](https://bluemix.net)
[![](https://img.shields.io/badge/platform-android-lightgrey.svg?style=flat)](https://developer.android.com/index.html)

### Table of Contents
* [Summary](#summary)
* [Requirements](#requirements)
* [Configuration](#configuration)
* [Run](#run)
* [License](#license)

### Summary

The Bluemix Mobile Starter for Weather showcases getting a forecast using the coordinates from Google Maps and gives you integration points for each of the Bluemix Mobile services.

### Requirements

* A [Bluemix](http://bluemix.net) Account
* [Android Studio](https://developer.android.com/studio/index.html) and [Gradle](https://gradle.org/gradle-download/)
* [Google Maps API Key](https://developers.google.com/maps/documentation/embed/get-api-key)
* [Weather](https://new-console.ng.bluemix.net/catalog/weather-company-data) service instance obtained from the [Bluemix Catalog](https://new-console.ng.bluemix.net/catalog/)

### Configuration

* Open the project in Android Studio and perform a Gradle Sync.
* Navigate to `res/values/google_maps_api.xml` and update the generated api key from the google developer console
* Input your credential information from the weather service

```HTML
<resources>
    <!--
    TODO: Before you release your application, you need a Google Maps API key.
    To do this, you can either add your release key credentials to your existing
    key, or create a new key.
    Note that this file specifies the API key for the release build target.
    If you have previously set up a key for the debug target with the debug signing certificate,
    you will also need to set up a key for your release certificate.
    Follow the directions here:
    https://developers.google.com/maps/documentation/android/signup
    Once you have your key (it starts with "AIza"), replace the "google_maps_key"
    string in this file.
    -->
    <string name="google_maps_key" templateMergeStrategy="preserve" translatable="false">YOUR_KEY_HERE</string>
</resources>
```
* Navigate to `res/values/weather_credentials.xml` and input your credential information:

```HTML
<resources>
    <string name="weather_username">YOUR_USERNAME_HERE</string>
    <string name="weather_password">YOUR_PASSWORD_HERE</string>
    <string name="weather_host">YOUR_HOST_HERE</string>
</resources>
```

Replace the credentials from your Weather instance.

**Service Credentials:**

  <img src="README_Images/service-credentials.png" alt="Service credentials" width="500px"/>

> **Note:** If one of your credentials has a special character (for example: `&`) you might need to escape it, as follows:  `&amp;`



### Run

Click **Run** to start the app in Android Studio.

<img src="README_Images/weather.png" alt="Weather App Screenshot" width="250px"/>

The application allows you determine the forecast of any location using your Weather instance on Bluemix. Long click to view the forecast.

### License
This package contains code licensed under the Apache License, Version 2.0 (the "License"). You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 and may also view the License in the LICENSE file within this package.
