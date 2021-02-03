# <img src="https://raw.githubusercontent.com/islands-wars/guidelines/master/assets/icon.png" width="64"> Islands Wars 


> Islands Wars is a Minecraft sky block server.

> Basic development rules and how to contribute.


# Getting started & generality
---

These instructions will get you a copy of the project up. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them
* [JDK] is the Java Development Kit, Islands Wars need version 15 or higher.

### Git flow

We use git flow as branching-model, simply init a new feature :
```shell
$> git flow feature start featureName
$> git add file
$> git commit -m "Clear commit message"

$> git flow feature publish featureName
```
And then open a new pull request. In the case that you see an error on production (master branch), you can supply a PR using hotfix instead of a feature.
Please refer to this [cheatsheet] if you are new to git flow and wants to learn the basics.

# Contributing
---

### Write good pull request

Follow the opening issues, or else create a dedicated one. Always works from develop (git flow feature init ..) and proposed your change to develop branch.
Don't forget to add a unit test if needed, to comment your code or adapt documentation. Be concise in your commit message.

# Java
---
### Deployment

Compile your modifications using gradle :
```shell
$> ./gradlew or gradlew task
```

### Coding guidelines

Adopting the [Google Java Style] with the following changes:

```
3
    A source file consists of, in order:

      * Package statement
      * Import statements
      * Default generated header (Cf 2.2 Header)
      * Exactly one top-level class
      * All class variables
      
      Exactly one blank line separates each section that is present.

4.2
    Our block indent is +4 characters

4.4
    Our line length is 200 characters.
```
Please use our project's [code style] and import him in Intellij Idea.
Be concise when naming method, var, class according to Java standard naming conventions.
Write a good commit [message].

### Header

Import and use this [header] when contributing, or your code will be rejected.

### Javadoc

Comment every public method you create and also whatever you judge necessary (a long stream for example).

# Rust
---

# License
---

> GNU GENERAL PUBLIC LICENSE Version 3

# Authors
---

Project members and contributors :)

* **[Vinetos :](https://twitter.com/vinetos)**
  * Initial works, lead dev
* **Xharos :**
  * Initial works, lead dev
* **[LightDiscord :](https://twitter.com/LightDiscord)**
  * Initial works on web site
* **[NormanFeltz :](https://twitter.com/normanfeltz)**
  * Initial works on admin sys
* **[DeltaEvo :](https://twitter.com/DeltaEvo_)**
  * Give advice and which stack use
* **[Creart :](https://twitter.com/Creaaart)**
  * Spellchecking

    
   [JDK]: <http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html>
   [cheatsheet]: <https://danielkummer.github.io/git-flow-cheatsheet/>
   [message]: <https://chris.beams.io/posts/git-commit/>
   [Google Java Style]: <https://google.github.io/styleguide/javaguide.html>
   [code style]: <https://github.com/islands-wars/guidelines/blob/master/java/is_scheme.xml>
   [header]: <https://github.com/islands-wars/guidelines/blob/master/java/HEADER>