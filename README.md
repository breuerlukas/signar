# Signar

Signar is a lightweight Java framework for event signaling and reactive hooks.

It makes it easy to emit, listen for, and respond to events across your application, without heavy dependencies or extra boilerplate code.

## Status

|      | Build Status                                                                                         |
|------|------------------------------------------------------------------------------------------------------|
| main | ![Java CI with Gradle](https://github.com/breuerlukas/signar/actions/workflows/gradle.yml/badge.svg) |

## Installation

```
repositories {
  maven {
    url = uri("https://maven.pkg.github.com/breuerlukas/signar")
    credentials {
      username = project.findProperty("gpr.user")?.toString() ?: System.getenv("GITHUB_USERNAME")
      password = project.findProperty("gpr.token")?.toString() ?: System.getenv("GITHUB_TOKEN")
    }
  }
}

dependencies {
  implementation("de.lukasbreuer:signar:1.0.0-SNAPSHOT")
}
```

## License

[GPL](https://github.com/breuerlukas/signar/blob/main/LICENSE.md)