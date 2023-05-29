# Piano Composer Show Template for Android
![Maven Central](https://img.shields.io/maven-central/v/io.piano.android/composer-show-template)

## Getting started
This is helper for simplifying "Show Template" event processing

### Dependencies

The Piano Composer Show Template is available as an AAR via Maven Central. To add dependencies, open your project’s build.gradle/build.gradle.kts and update the dependencies block as follows:

Kotlin DSL
```kotlin
dependencies {
    implementation("io.piano.android:composer-show-template:$VERSION")
}
```

### Usage
Add code into your show template listener

Kotlin
```kotlin
// Use one of these
ShowTemplateController(showTemplateEvent, customJavascriptInterface).show(activity)
ShowTemplateController(showTemplateEvent, customJavascriptInterface).show(activity, inlineWebViewProvider)
```

## How to show templates inline

First, you need to prepare some content with a webview placed inline:

![SDK](images/1.png)

Then, you can target this webview in Composer by adding the ID of the webview into the inline container selector field:

![SDK1](images/2.png)

This will result in the template to be shown inline in your Android app. For example like this:

![SDK2](images/3.png)

