# Git Flow - Ararabots

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Get Started](#get-started)
- [References](#references)

# Introduction
**Git flow** is an alternative Git branching model that involves the use of feature branches and multiple primary branches.

# Installation
In order to facilitate the commands, git flow has a package specific for the usage of the method.

For **linux**:
```bash
sudo apt install git-flow
```

For **MacOS**:
```bash
brew install git-flow
```
For **Windows**: [Download link.](https://gitforwindows.org/ 
)

# Get Started

For a **new repository**, run:

```bash
git flow init
```

You should see:

```text
Initialized empty Git repository in ~/project/.git/ 
No branches exist yet. Base branches must be created now. Branch name for production releases: [main] 
Branch name for "next release" development: [develop] 
How to name your supporting branch prefixes? 
Feature branches? [feature/] 
Release branches? [release/] 
Hotfix branches? [hotfix/] 
Support branches? [support/] 
Version tag prefix? []
```

this command will format the git repository and ask you the names of each branch to set the convetion for this project, for common convetion just keep it blank

### Basic Commands

#### Create and merge branch

You can create and merge a branch automatically, here is an example to a feature branch:

 ```bash
git flow feature start [FEATURE]
 ```
 ```bash
 git flow feature finish [BRANCH NAME]
 ```

For the other branchs just switch feature to **release**/**hotfix**/**support**

#### Publish and Pull

To update the remote server with the modifications in your local workspace:


 ```bash
git flow feature publish [BRANCH NAME]
 ```

To update the your local workspace with new added modification in the remote server:

 ```bash
git flow feature pull origin [BRANCH NAME]
 ```

### Commit convention

Each commit has a purpose, to identify what was done with it, we need a commit name convetion, here's a table with the most common tags to use when commiting:

| Commit Type | Title                    | Description                                                                                                 
| ----------- | ------------------------ | ----------------------------------------------------------------------------------------------------------- 
| `feat`      | Features                 | A new feature                                                                                               
| `fix`       | Bug Fixes                | A bug Fix                                                                                                   
| `docs`      | Documentation            | Documentation only changes                                                                                  
| `style`     | Styles                   | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      
| `refactor`  | Code Refactoring         | A code change that neither fixes a bug nor adds a feature                                                   
| `perf`      | Performance Improvements | A code change that improves performance                                                                     
| `test`      | Tests                    | Adding missing tests or correcting existing tests                                                           
| `build`     | Builds                   | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         
| `ci`        | Continuous Integrations  | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) 
| `chore`     | Chores                   | Other changes that don't modify src or test files                                                           
| `revert`    | Reverts                  | Reverts a previous commit                                                                                   

# References



[Git Flow - Cheat Sheet](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwi64pnr1b2CAxXSrZUCHcpnDcwQFnoECAkQAQ&url=https%3A%2F%2Fdanielkummer.github.io%2Fgit-flow-cheatsheet%2F&usg=AOvVaw3cztku7-5n6R6SV0OLPQkZ&opi=89978449)

https://medium.com/linkapi-solutions/conventional-commits-pattern-3778d1a1e657 


https://www.alura.com.br/artigos/git-flow-o-que-e-como-quando-utilizar  


https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow 


https://youtu.be/wzxBR4pOTTs?si=eEqrQQfoekFsWvWg 
