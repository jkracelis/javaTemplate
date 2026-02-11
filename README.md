# 📦 javaTemplate
Simple Java 25 template project using Gradle with testing and formatting support.

---
## 🚀 Tech Stack
* Java 25
* Gradle
* JUnit 5
* Spotless (Palantir formatter)
* GitHub Actions (CI)

---
## 📁 Project Structure
```
javaTemplate/
├── .github/workflows/java-ci.yml
├── build.gradle
├── settings.gradle
├── gradlew
├── gradlew.bat
├── src/
│   ├── main/java/
│   └── test/java/
```

---
## 🛠 Installation
### Ubuntu
Install JDK 25:
```bash
sudo apt install openjdk-25-jdk
```

---
## 🔧 Build
### Linux / macOS
```bash
./gradlew build
```
### Windows
```bash
gradlew.bat build
```
Run the generated JAR:
```bash
java -jar build/libs/javaTemplate.jar
```
---
## ▶ Run Application

```bash
./gradlew run
```

---
## 🧪 Run Tests
```bash
./gradlew test
```
---
## 🎨 Code Formatting
Format code:
```bash
./gradlew spotlessApply
```
Check formatting:
```bash
./gradlew spotlessCheck
```
Formatting is enforced during `build`.

## 🔄 Continuous Integration (CI)
This project uses GitHub Actions to automatically:
✅ Run formatting check (spotlessCheck)
✅ Build the project
✅ Run all tests

CI runs on:
Every push
Every pull request
If formatting fails or tests fail, the build will fail.
Workflow file:
```bash
.github/workflows/ci.yml
```

