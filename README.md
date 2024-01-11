<div align="center">
  <br />
  <img src="assets/logo.png" alt=".gitgitgoLogo" width="30%"/>
  <h1>.gitgitgo</h1>
  <p>
     A template for your gitgitgo repository
  </p>
</div>

<!-- Badges -->
<div align="center">
   <a href="https://github.com/cophilot/.gitgitgo/blob/main/LICENSE">
       <img src="https://img.shields.io/github/license/cophilot/.gitgitgo" alt="license" />
   </a>
   <a href="https://github.com/cophilot/.gitgitgo/stargazers">
       <img src="https://img.shields.io/github/stars/cophilot/.gitgitgo" alt="stars" />
   </a>
   <a href="https://github.com/cophilot/.gitgitgo/commits/main">
       <img src="https://img.shields.io/github/last-commit/cophilot/.gitgitgo" alt="last commit" />
   </a>
</div>

---

-   [Concept](#concept)
-   [Installation](#installation)
-   [Templates](#templates)
-   [Placeholder](#placeholder)

---

## Concept

This repository is a template for your own gitgitgo repository. It contains a basic structure and some useful files to get you started. Gigitgo helps you to initilize a git repository with a single command. It also helps adding additional files to your repository.

This repository will contains the file templates that will be used by a gitgitgo tool.

To get started with gitgitgo, you can use the [GitGitGo-CLI](https://github.com/cophilot/GitGitGo-CLI).

---

## Installation

1. Make your own repository with this template.
2. Edit the files.json file to your needs.
3. Specify the repository owner as the provider in the GitGitGo-CLI.
4. run `gitgitgo print -n` to see the files that can be added to your repository.

---

## Templates

Take a look at the [files.json](files.json). Here you can see a json object called `files`. This object contains all the files that can be added to your repository. Modify this object to your needs.
A file can have the following properties:

-   `name`: The name of the file. This will be the name of the file in your repository when it is added. Here you can also specify a path to the file. The path will be created if it does not exist.
-   `text`: A string array that contains the text that will be written to the file. Each string in the array will be a new line in the file.
-   `oninit`: A boolean that specifies if the file should be added to the repository when you run `gitgitgo init`. If not specified, the value will be `false`.
-   `gitignore`: A boolean that specifies if the file should be added to the .gitignore file when you run `gitgitgo init`. If not specified, the value will be `false`.
-   `keywords`: A comma seperated string that contains keywords to descripe the usage of the file.
-   `description`: A string that contains a description of the file.

---

## Placeholder

You can use placeholders in your files. A placeholder is a string that starts with `${{` and ends with `}}`. The placeholder will be replaced with a value when the file is added to your repository.

The following placeholders are available:

-   `${{YEAR}}`: The current year.
-   `${{MONTH}}`: The current month.
-   `${{DAY}}`: The current day.
-   `${{REPONAME}}`: The name of your repository.
-   `${{GITHUBNAME}}`: Your github username.
-   `${{FULLNAME}}`: Your full name.

---

by [Philipp B.](https://github.com/cophilot)
