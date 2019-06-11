# Graddle

Tags: java, build

Gradle is a build automation tool for JVM based languages like java, scala etc.

## Things to know

- `build.gradle` is the entry point file
- All build scripts are written in groovy
- Each project is made of collection of Tasks: these are atomic units of work that represent the
things needed to be done to build the project
- `gradle tasks` returns the default Tasks
- `gradle tasks --all` returns all the Tasks
- `plugin { id 'java' }` applies other extra tasks from java plugin
- `gradle properties` returns list of gradle properties
- `sourceSets` property is set by Java plugin, this tells the path of java src

## Making a custom task

    task customRun(type: JavaExec) {
      classpath = sourceSets.main.runtimeClasspath
      standardInput = System.in
      main = 'tictactoe.cli.Main'
    }

`gradle customRun` would run this customRun task
