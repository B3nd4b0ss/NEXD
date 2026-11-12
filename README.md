<div align="center">

<img src="assets/logo.svg" width="96" height="96" alt="">

<h1>NEXD</h1>

<p>
<b>One desktop app for all your projects.</b><br>
Start their dev servers, commit and pull, run Docker and databases,<br>
and keep the tools they need up to date. For Windows and Linux.
</p>

<p>
<a href="https://github.com/B3nd4b0ss/NEXD/releases"><img src="https://img.shields.io/github/v/release/B3nd4b0ss/NEXD?include_prereleases&sort=date&display_name=release&label=latest&style=flat-square&color=6b5cf6" alt="Latest version"></a>
<a href="https://github.com/B3nd4b0ss/NEXD/releases"><img src="https://img.shields.io/github/downloads/B3nd4b0ss/NEXD/total?style=flat-square&color=2f6fd6&label=downloads" alt="Downloads"></a>
<img src="https://img.shields.io/badge/Windows%20%C2%B7%20Linux-555?style=flat-square" alt="Windows and Linux">
</p>

<p>
<a href="https://github.com/B3nd4b0ss/NEXD/releases/download/v0.0.2-beta/NEXD-0.0.2-beta-windows-setup.exe"><img src=".github/readme/download-windows.svg" height="56" alt="Download NEXD 0.0.2-beta for Windows"></a>&nbsp;&nbsp;
<a href="https://github.com/B3nd4b0ss/NEXD/releases/download/v0.0.2-beta/NEXD-0.0.2-beta-linux-x64.tar.gz"><img src=".github/readme/download-linux.svg" height="56" alt="Download NEXD 0.0.2-beta for Linux"></a>
</p>

<p><sub>Version <b>0.0.2-beta</b> (beta), 12 November 2026 &nbsp;·&nbsp; <a href="https://github.com/B3nd4b0ss/NEXD/releases/tag/v0.0.2-beta">Release notes</a> &nbsp;·&nbsp; <a href="https://github.com/B3nd4b0ss/NEXD/releases">All versions</a> &nbsp;·&nbsp; <a href="https://github.com/B3nd4b0ss/NEXD/releases/download/v0.0.2-beta/SHA256SUMS.txt">Checksums</a></sub></p>

</div>

<br>

NEXD finds the projects in your workspace folders and knows what each one is: a Node.js app, Spring Boot, .NET, Python, Go, a Docker compose stack, or several of them linked together. You get one place for what you otherwise do in a handful of terminals.

<table>
<tr>
<td width="50%" valign="top">

### Run

Dev servers and scripts in their own terminals, with the address to open, groups that start an API before its frontend, and processes that restart when they crash or go on when NEXD quits.

</td>
<td width="50%" valign="top">

### Git

The everyday without the command line: changes and commits, branches, merges, tags, cherry-picks, stashes, blame, and getting out of a merge that stopped on conflicts. Pull requests on GitHub, GitLab, Gitea, Forgejo and Bitbucket, and GitHub Actions.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Docker

Containers and compose stacks per project, dev containers, and new containers from an image or a Dockerfile.

</td>
<td width="50%" valign="top">

### Databases

PostgreSQL, MySQL, MariaDB, MongoDB, Redis and SQLite, in Docker or on a server you connect. Browse and edit data, back up and restore, CSV in and out, migrations, and the connection wired into Spring Boot, ASP.NET Core or Django.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Tools

Which JDK, Node.js, Python, Maven or Gradle a project uses, installing the ones that are missing, and the default version on your PATH.

</td>
<td width="50%" valign="top">

### Environment

Environment variables per project, in profiles, with secrets in the system keychain instead of a file.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Tickets and notes

Tickets, notes and saved commands per project, kept on your computer.

</td>
<td width="50%" valign="top">

### Yours alone

Nothing leaves your computer except what you ask for, like pushing to Git. Tokens and passwords stay in the system keychain, never in a file.

</td>
</tr>
</table>

## Install

Download the build for your system with the buttons at the top, or from the [releases](https://github.com/B3nd4b0ss/NEXD/releases).

**Windows 10 and 11.** Run `NEXD-0.0.2-beta-windows-setup.exe`. It installs for your user only (no administrator rights) in `%LOCALAPPDATA%\Programs\NEXD`. The builds are not code-signed yet, so SmartScreen asks once: **More info → Run anyway**.

**Linux (x64, Ubuntu 22.04 or newer).** Unpack `NEXD-0.0.2-beta-linux-x64.tar.gz` where you want to keep it and run `./install-launcher.sh` once, which adds NEXD to the application menu. On Debian and Ubuntu it needs:

```bash
sudo apt install libgtk-3-0 libayatana-appindicator3-1 libsecret-tools libglib2.0-bin xdg-utils
```

**macOS.** Not built at the moment.

NEXD needs Git, and for the rest whatever your projects use (Node.js, a JDK, Docker…): its Tools page shows what is missing and installs it.

## Updates

NEXD looks for a new release when it starts and every six hours, and installs it when you say so. Every release is signed: NEXD checks the signature and the checksum of what it downloads, and refuses anything that does not match. **Settings → Updates → Betas too** gets you the versions before a release.

## What's new

<details open>
<summary><b>0.0.2-beta</b> &nbsp;·&nbsp; 12 November 2026 &nbsp;·&nbsp; beta</summary>

- Windows: typing into a terminal works again. Letters and other characters did not arrive, only keys like Enter, Backspace and the arrows.
- Git tab: a tag made in the Branches view shows up right away. It showed only after the next commit.

<sub><a href="https://github.com/B3nd4b0ss/NEXD/releases/tag/v0.0.2-beta">Downloads and checksums of 0.0.2-beta</a></sub>
</details>

<details>
<summary><b>0.0.1-beta</b> &nbsp;·&nbsp; 12 November 2026 &nbsp;·&nbsp; beta</summary>

The first beta of NEXD: create, run and maintain all your projects (dev servers, Git, Docker, databases) on Windows and Linux.

<sub><a href="https://github.com/B3nd4b0ss/NEXD/releases/tag/v0.0.1-beta">Downloads and checksums of 0.0.1-beta</a></sub>
</details>

## Problems and ideas

In NEXD: **Settings → About → Report a problem** (or the Logs page). It opens an issue here with your version, your system and the end of NEXD's log, with tokens, passwords and your home folder taken out. You can also [open an issue](https://github.com/B3nd4b0ss/NEXD/issues/new) yourself.

## Your data

Everything NEXD keeps is in `~/.nexd` (`%USERPROFILE%\.nexd` on Windows), and tokens and passwords in the system keychain. **Settings → Move to another computer** exports your settings to a file for the next one.

---

<sub>© 2026 Ben Grob. NEXD is not open source; the builds here are free to use.</sub>
