# Gson
[![](https://jitpack.io/v/FunkyMuse/KAHelpers.svg)](https://jitpack.io/#FunkyMuse/KAHelpers)


## Usage
1. Add JitPack to your project build.gradle

```gradle
allprojects {
  repositories {
    ...
    maven { url 'https://jitpack.io' }
   }
}
```

2. Add the dependency in the application build.gradle

```gradle
dependencies {

implementation "com.github.FunkyMuse.KAHelpers:gson:$utilsVersion"


}
```

3. Add an object to your prefs (discouraged)
```kotlin
requireContext().defaultPrefs.putObject("myObj", MyObj())
```

4. Convert JSON string to object
```kotlin
val myObj : MyObj = gson.fromJson<MyObj>(someExternalJson)
```

5. Convert object to JSON
```kotlin
val json : String = myObjectInstance.toJson()
```
