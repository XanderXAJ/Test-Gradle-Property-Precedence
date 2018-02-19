# Test Gradle Property Precedence

Tests whether properties in `gradle.properties` can be overridden from the command line.

## Result

Yes, they can, using project properties:

```bash
$ ./gradlew -q print
valueFromFile

$ ./gradlew -q -PgradlePropertiesProp=valueFromCli print
valueFromCli
```

## Usage

```bash
./gradlew -q print
./gradlew -q -PgradlePropertiesProp=valueFromCli print
```
