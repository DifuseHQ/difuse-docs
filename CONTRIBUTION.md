## Contribution To Documentation

### Prerequisites

This documentation uses mdbook for rendering and generation. We also use git version control system for managing the documentation. To contribute to the documentation, you need to have the following tools installed on your system:

* [git](https://git-scm.com/downloads)
* [mdbook](https://github.com/rust-lang/mdBook/releases/tag/v0.4.31)

You can install both of that for the operating system you're using, be it mac, windows or linux. Once you have them installed, you can clone the repository and start contributing.

### Introduction to Git

Git is a very powerful version control system that allows you to track changes in your code and collaborate with other people. It is a distributed version control system, which means that you can work on your code locally and then push it to a remote repository. You can also pull changes from the remote repository to your local repository. This is very useful when you're working with other people on a project.

#### Cloning the Repository

Cloning the repository basically means downloading the repository from the remote server to your local machine. To clone the repository, you need to run the following command (in CMD for windows or terminal for linux/mac):

```bash
git clone https://github.com/DifuseHQ/difuse-docs
```

This will clone the repository into a folder called `difuse-docs` in your current working directory (which is the directory you are in).

If you want to open a CMD prompt in a specific folder you can type in "cmd" in the address bar of the folder and press enter. This will open a CMD prompt in that folder, see the below picture for reference:
 
![https://i.imgur.com/T7O9wN6.jpg](https://i.imgur.com/T7O9wN6.jpg)


#### Editing the Documentation

Once you have cloned the repository, you can start editing the documentation. The documentation is written in markdown, which is a very simple markup language. You can learn more about markdown [here](https://www.markdownguide.org/basic-syntax/).

All the markdown files are in the `src` folder. You can edit any of the files in that folder. Once you have made your changes, you can preview them by running the following command:

```bash
mdbook serve
```

This will start a local server on your machine and you can preview the documentation by going to `http://localhost:3000` in your browser.

#### Committing Changes

Committing changes basically means saving your changes to the local repository. To commit your changes, you need to run the following command:

```bash
git add .
git commit -m "Commit Message"
```

This will add all the changes you have made to the local repository and then commit them with the commit message you have provided. You can replace `Commit Message` with a message that describes the changes you have made. Please make sure that the commit message is descriptive and explains the changes you have made. You can have a title and body to commit message, like this if you want:

```bash
git commit -m "Title" -m "Body"
```

#### Pushing Changes

Pushing changes basically means uploading your changes to the remote repository. To push your changes, you need to run the following command:

```bash
git push origin master
```