Kotlin is a modern, expressive language that blends elegance with JVM power. Here's a way to try it out on Windows!

#### Setup

> Download [OpenJDK](https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.14+7/OpenJDK17U-jdk_x64_windows_hotspot_17.0.14_7.zip) and unzip to `C:\tools\jdk-17`.<br/>
> Download [Kotlin compiler](https://github.com/JetBrains/kotlin/releases/download/v2.2.21/kotlin-compiler-2.2.21.zip) and unzip to `C:\tools\kotlin-compiler`.

## Write code

Create a new folder for your project `(eg. C:\kotlin_projects\hello_project\)`. <br/>
Write code in /src subdirectory:

```kotlin
data class User(val name: String) { 
    fun write() = println("Hello, $name!")
} 
User("Kotlin").write()

// eg. C:\kotlin_projects\hello_project\src\Main.kt
```

## Compile & Run

From your project root, compile &amp; run:

```
cd C:\kotlin_projects\hello_project
C:\tools\kotlin-compiler\kotlin\bin\kotlinc -cp "c:\tmp_dl\kotlin-compiler\kotlinc\lib\kotlin-stdlib.jar" src/Main.kt -include-runtime -d app.jar
C:\tools\jdk-17\bin\java -jar app.jar
```
> &gt;&gt; Hello, Kotlin!

