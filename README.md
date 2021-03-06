# ARCHIVE NOTICE

This project has been archived for the following reasons:

1. Lack of developer attention/interest.
2. The planned elimination of Electron plugins and the general state of its ecosystem.

If you would like to resume maintainership of this repository, please open an issue describing your plan to contribute and the repository may be unarchived.

# Jellyfin Desktop

Jellyfin Desktop is a desktop client that connects to a Jellyfin server.

![image](screenshots/Home.PNG)

## Installing
You can download jellyfin desktop for your operating system from the
[releases page](https://github.com/jellyfin/jellyfin-desktop/releases).

### Nightly Versions
You can download the latest, shiniest (and probably buggiest) version built straight from master
[from the build system](https://dev.azure.com/jellyfin-project/jellyfin/_build?definitionId=22&_a=summary&repositoryFilter=13&branchFilter=1835)

## FAQ
### Jellyfin Desktop Settings Location

Q: Where can I find the settings of Jellyfin Desktop?

A: The settings for Jellyfin Desktop, including the server URL, are
stored in the following folders:

- ~~%APPDATA%/Jellyfin Theater on Windows~~ (outdated)
- ~/.config/jellyfin-desktop on Linux
- ~~\~/Library/Application Support/Jellyfin Theater on macOS~~ (outdated)

## Contributing
### Prerequisites
This application is implemented as an Electron app and is built off of 
a NodeJS code base. Because of this you will need the NodeJS runtime and
the `yarn` package manager. The following versions have been tested: 

| Software Name | Version          |
| ------------- | ---------------- |
| Node JS       | 12               |
| yarn          | 1.22             |

To contribute you will need to set up a fork. To learn more about how to use forks, you can read
"[Fork a repo](https://help.github.com/en/github/getting-started-with-github/fork-a-repo)" and
"[Working with forks](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/working-with-forks)".

### Building Jellyfin Desktop
After setting up you fork, you will need to install the dependencies for the project. You can do so by
typing the following into your commandline:
```
$ yarn install
```

Once the installation has been finished you can start a test version of the application by using this
command:
```
$ yarn start
```

#### Building Packages for Windows

```$ yarn run build:win```

#### Building Packages for Linux
_Ubuntu: You need to install `rpmbuild` to build all linux packages_

```$ yarn run build:linux```

#### Building Packages for Macintosh

```$ yarn run build:mac```

## Screenshots

![image](screenshots/Login.PNG)
![image](screenshots/Movies.PNG)
![image](screenshots/TV_Shows.PNG)
![image](screenshots/Music.png)
