# Groovy

A JVM language similar to java but with a more concise syntax.

## Installation

Mac OSX - `brew install groovy`

## Things to know

- Valid Java code is valid Groovy
- `groovysh` Opens interactive groovy shell
- We don't need surrounding class and main method to execute our code
- Supports closure
- Can be used as code as configuration

## Example

    dependencies {
      testCompile group: 'junit', name: 'junit', version: '4.12'
    }

here dependencies is a method which takes a "runnable" block of code(a closure). Inside which we've
called the `testCompile` method with 'junit' etc as arguments (the group, name, version section is
actually short hand for a groovy map, essentially a list of key value pairs)

