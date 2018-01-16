[version]: https://api.bintray.com/packages/jagrosh/maven/JDA-Utilities/images/download.svg
[download]: https://bintray.com/jagrosh/maven/JDA-Utilities/_latestVersion
[license]: https://img.shields.io/badge/License-Apache%202.0-lightgrey.svg
[issues]: https://img.shields.io/github/issues/JDA-Applications/JDA-Utilities.svg 
[issueslink]: https://github.com/JDA-Applications/JDA-Utilities/issues

[ ![version][] ][download]
[ ![license][] ](https://github.com/JDA-Applications/JDA-Utilities/tree/master/LICENSE)
[ ![issues][] ][issueslink]

## JDA-Utilities
JDA-Utilities is a series of tools and utilities for use with [JDA](https://github.com/DV8FromTheWorld/JDA) 
to assist in bot creation.

## Version 2.0 Notice
Version 2.0 comes with a lot of big (some breaking) changes to the library.

If you use this library for anything, it is **STRONGLY** recommended you read 
[this gist](https://gist.github.com/TheMonitorLizard/4f09ac2a3c9d8019dc3cde02cc456eee)
which documents all of the changes that have been made.

If you have questions or concerns about any of these changes, please contact **Shengaero**#9090.

## Packages

Since JDA-Utilities 2.0, the library has been split into multiple modular projects,
in order to better organize it's contents based on what developers might want to use and not use.

+ [Command Package](https://github.com/JDA-Applications/JDA-Utilities/tree/master/command)
+ [Commons Package](https://github.com/JDA-Applications/JDA-Utilities/tree/master/commons)
+ [CommandDoc Package](https://github.com/JDA-Applications/JDA-Utilities/tree/master/doc)
+ [Examples Package](https://github.com/JDA-Applications/JDA-Utilities/tree/master/examples)
+ [Menu Package](https://github.com/JDA-Applications/JDA-Utilities/tree/master/menu)

Visit individual modules to read more about their contents!

## Getting Started
You will need to add this project as a dependency (either from the latest .jar from the releases page, 
or via maven or gradle), as well as [JDA](https://github.com/DV8FromTheWorld/JDA). 

With maven:
```xml
  <dependency>
    <groupId>com.jagrosh</groupId>
    <artifactId>jda-utilities</artifactId>
    <version>2.0</version>
    <scope>compile</scope>
  </dependency>
  <dependency>
    <groupId>net.dv8tion</groupId>
    <artifactId>JDA</artifactId>
    <version>LATEST</version>
  </dependency>
```
```xml
  <repository>
    <id>central</id>
    <name>bintray</name>
    <url>http://jcenter.bintray.com</url>
  </repository>
```

With gradle:
```groovy
dependencies {
    compile 'com.jagrosh:jda-utilities:2.0'
    compile 'net.dv8tion:JDA:LATEST'
}

repositories {
    jcenter()
}
```

Individual modules can be downloaded using the same structure shown above, with the addition of the module's
name as a suffix to the dependency:

With maven:
```xml
  <dependency>
    <groupId>com.jagrosh</groupId>
    <!-- Notice that the dependency notation ends with "-command" -->
    <artifactId>jda-utilities-command</artifactId>
    <version>2.0</version>
    <scope>compile</scope>
  </dependency>
```

With gradle:
```groovy
dependencies {
    // Notice that the dependency notation ends with "-command"
    compile 'com.jagrosh:jda-utilities-command:2.0'
}
```

## Examples
Check out the [ExampleBot](https://github.com/jagrosh/ExampleBot) for a simple bot example.

Other guides and information can be found on the [wiki](https://github.com/JDA-Applications/JDA-Utilities/wiki).

## Projects
[**Vortex**](https://github.com/jagrosh/Vortex) - Vortex is an easy-to-use moderation bot that utilizes the JDA-Utilities library for the Command Client and some of the menus<br>
[**JMusicBot**](https://github.com/jagrosh/MusicBot) - This music bot uses the Command Client for its base, and several menus, including the OrderedMenu for search results and the Paginator for the current queue<br>
[**GiveawayBot**](https://github.com/jagrosh/GiveawayBot) - GiveawayBot is a basic bot for hosting quick giveaways!<br>
