# EasyBugReport  [![API](https://img.shields.io/badge/API-9%2B-blue.svg?style=flat)](https://android-arsenal.com/api?level=9)
A simple Android library to create bug report email intents easily.

---

## Releases:

#### Current release: N/A.

You can see all the library releases [here](https://github.com/marcoscgdev/EasyBugReport/releases).

---

##Screenshots

<img src="https://raw.githubusercontent.com/marcoscgdev/EasyBugReport/master/device-2017-03-12-171059.gif" width="350">

<a href='#'><img alt='Get it on Google Play' src='https://play.google.com/intl/en_us/badges/images/generic/en_badge_web_generic.png' height='90'/></a>

---

## Usage:

### Adding the depencency

Add this to your root *build.gradle* file:

```
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

Now add the dependency to your app build.gradle file:

```
Coming soon...
```

### Creating the email intent

Here is a complete snippet of it usage:

```java
EasyBugReport.on(this)
                .withEmail("example@email.com") // Your email
                .withSubject("Bug report for " + getResources().getString(R.string.app_name)) // Email subject
                .withExtraText("Extra text.") // Email extra text
                .withDeviceInfo(false) // Default true, generates a .txt file with some user device info
                .go();
```

---
>See the *sample project* to clarify any queries you may have.

---

##License

```
Copyright 2017 Marcos Calvo García

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

