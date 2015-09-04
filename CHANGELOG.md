# Util Library Change Log

Note that the "Build Tools" component is decoupled and has its own change log.

## 1.0

Initial release

## 1.1

Changed the configuration mechanism to use a properties POJO and one (or more) properties builder(s). Properties
Builders can extract properties from various sources, and produce a properties POJO. A default implementation
that extracts properties of a Map<String, String> is provided in this implementation.

Library consumers can use their own mechanism to populate the properties POJO. Examples include Spring configuration,
injection mechanisms, creating a new builder that uses Java Properties, etc.