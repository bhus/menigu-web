Kotlin is a modern, expressive language that blends elegance with JVM power. Try it out!

```kotlin
data class User(val name: String) { 
    fun write() = println("Hello, $name!")
} 
User("Kotlin").write()
```

### 1. Install

#### jdk
Download openjdk. (For example, <a href='https://github.com/adoptium/temurin17-binaries/releases/download/jdk-17.0.14+7/OpenJDK17U-jdk_x64_windows_hotspot_17.0.14_7.zip'>Windows version</a>). <br/>
Unzip somewhere. (For example, into C:\tools\jdk-17)<br/>
Add bin to path: ``` setx PATH "%PATH%;C:\tools\jdk-17\bin" ```

#### kotlin

Download Kotlin compiler (For example, <a href='https://github.com/JetBrains/kotlin/releases/download/v2.2.21/kotlin-compiler-2.2.21.zip'>here</a>).<br/>
Unzip somewhere. (For example, into C:\tools\kotlin-compiler)<br/>
Add bin to path: ``` setx PATH "%PATH%;C:\tools\kotlin-compiler\bin" ```

### 3. Create a project

In a new folder, create /src/Main.kit:

```kotlin
// In src/Main.kit
fun main() { println("Hello from Kotlin on the command line!") }
```

### 4. Compile & Run

From the new project root, run:

```
kotlinc src/Main.kt -include-runtime -d app.jar
java -jar app.jar
```

_>> Hello from Kotlin on the command line!_

### 4. Onward!

It's that easy to get up and going!
