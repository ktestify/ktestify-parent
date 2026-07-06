<p align="center">
  <img src="https://raw.githubusercontent.com/ktestify/.github/refs/heads/main/profile/assets/png/ktestify-banner-2x.png" alt="ktestify-core" width="100%"/>
</p>

# ktestify-parent

Parent POM for all [ktestify](https://github.com/ktestify) modules.

## What it provides

- **Single source of truth** for all dependency versions (Kafka, Cucumber, JUnit, Testcontainers, etc.)
- **Centralised plugin management** (compiler, surefire, failsafe, jacoco, spotless, source, javadoc, etc.)
- **Shared profiles** (`release`, `skip-tests`, `integration-tests`)
- **Confluent repository** declaration
- **Jackson BOM** import for consistent Jackson module versions

## Usage

```xml
<parent>
    <groupId>io.github.ktestify</groupId>
    <artifactId>ktestify-parent</artifactId>
    <version>1.0.0</version>
</parent>
```

After setting the parent, child modules can omit versions from all managed dependencies and plugins.

## Dependabot

Only this repository needs Dependabot for shared dependency updates. Child modules only need to bump the parent version to pick up all dependency changes.

<p align="center">
  <img src="https://raw.githubusercontent.com/ktestify/.github/refs/heads/main/profile/assets/png/ktestify-logo-128.png" width="32" height="32" alt="KTestify"/>
  <br/>
  <sub>Assert the stream. Own the pipeline.</sub>
</p>