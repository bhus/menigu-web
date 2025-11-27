Kotlin is a modern, expressive language that blends elegance with JVM power. Try it out!

### Setup

> Download [OpenJDK](https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.14+7/OpenJDK17U-jdk_x64_windows_hotspot_17.0.14_7.zip) and unzip to `C:\tools\jdk-17`, then add to PATH with `setx PATH "%PATH%;C:\tools\jdk-17\bin"`.<br/>
> Download [Kotlin compiler](https://github.com/JetBrains/kotlin/releases/download/v2.2.21/kotlin-compiler-2.2.21.zip) and unzip to `C:\tools\kotlin-compiler`, then add to PATH with `setx PATH "%PATH%;C:\tools\kotlin-compiler\bin"`.

---

## 1. Write code

Create a new folder for your project (e.g., `C:\kotlin_projects\hello_project`).

Write code in /src directory (eg. `C:\kotlin_projects\hello_project\src\Main.kt`):

```kotlin
data class User(val name: String) { 
    fun write() = println("Hello, $name!")
} 
User("Kotlin").write()

// src/Main.kt
```

## 2. Compile & Run

From your project root (e.g., `C:\kotlin_projects\hello_project`), run:

```
kotlinc src/Main.kt -include-runtime -d app.jar
java -jar app.jar
```
> &gt;&gt; Hello from Kotlin!

