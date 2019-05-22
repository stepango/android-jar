# AndroidJar
Gradle plugin which will find your android.jar


In your root `build.gradle` add
```
plugins {
	id 'com.stepango.androidjar' version “0.1”
}
ext.androidJar = androidjar.find(targetSdkVersion)
```

And add this in module `build.gradle`
```
dependencies {
	implementation Libs.kotlin
	compileOnly androidJar
}
```
