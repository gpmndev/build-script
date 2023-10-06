Add to top of **< library module >/build.gradle**
```groovy
project.ext.buildScriptVersion = "https://raw.githubusercontent.com/gpmndev/build-script/master/1.0/"
apply from: "${project.ext.buildScriptVersion}outputs.gradle"
```

--------------
Sample: locating/build.gradle
```groovy
plugins {
    id 'com.android.library'
    id 'org.jetbrains.kotlin.android'
}
project.ext.buildScriptVersion = "https://raw.githubusercontent.com/gpmndev/build-script/master/1.0/"
apply from: "${project.ext.buildScriptVersion}outputs.gradle"

android {
...
}
```
