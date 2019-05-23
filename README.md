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

[Presentation Mobuis 2019 RUS](https://drive.google.com/open?id=1r68gebquy6nSALzrCyP3kpK14tFL51pd)
