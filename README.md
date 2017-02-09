
Android NetworkConnect Sample
===================================

This sample demonstrates how to connect to the network and fetch raw HTML using
HttpsURLConnection. AsyncTask is used to perform the fetch on a background thread.

Introduction
------------

This sample demonstrates how to connect to the network and fetch raw HTML using
[`HttpsURLConnection`][4]. Since API 11, it is required by default that all network
operations run on a background thread in order to avoid hanging on the UI thread. Only
when the network response is ready should the work return to the main thread to update
the UI. An [`AsyncTask`][3] is a viable background task manager that is used to perform
the network operation and return to the UI thread upon completion.

The sample also utilizes the [`ConnectivityManager`][1] to determine if you have
a network connection, and if so, what type of connection it is.

Using an [`AsyncTaskLoader`][6] or an [`IntentService`][5] are two common alternatives
for managing longer running background work.

[1]: https://developer.android.com/reference/android/net/ConnectivityManager.html
[2]: https://developer.android.com/reference/android/net/NetworkInfo.html
[3]: https://developer.android.com/reference/android/os/AsyncTask.html
[4]: https://developer.android.com/reference/javax/net/ssl/HttpsURLConnection.html
[5]: https://developer.android.com/reference/android/app/IntentService.html
[6]: https://developer.android.com/reference/android/content/AsyncTaskLoader.html

Pre-requisites
--------------

- Android SDK 25
- Android Build Tools v25.0.2
- Android Support Repository

Screenshots
-------------

<img src="screenshots/main.png" height="400" alt="Screenshot"/> 

Getting Started
---------------

This sample uses the Gradle build system. To build this project, use the
"gradlew build" command or use "Import Project" in Android Studio.

Support
-------

- Google+ Community: https://plus.google.com/communities/105153134372062985968
- Stack Overflow: http://stackoverflow.com/questions/tagged/android

If you've found an error in this sample, please file an issue:
https://github.com/googlesamples/android-NetworkConnect

Patches are encouraged, and may be submitted by forking this project and
submitting a pull request through GitHub. Please see CONTRIBUTING.md for more details.

License
-------

Copyright 2016 The Android Open Source Project, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.
