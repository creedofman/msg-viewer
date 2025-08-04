<div align="center">
    <img src="https://github.com/user-attachments/assets/f065cc3a-c40b-4917-ac51-006cfbc78f0f" alt="Icon"/>
    <p><strong>https://creedofman.github.io/msg-viewer/</strong><p>
</div>

---

**Note:** This project is a fork. I am not the original creator—credit for the original code and idea goes to [molotochok/msg-viewer](https://github.com/molotochok/msg-viewer).  
I have made minor changes to remove all analytics and ensure there are no external calls whatsoever.  
No analytics, tracking, or external requests of any kind are present.

---

### Description
This tool allows you to read Outlook `.msg` files in your browser without sending any data to an external server. It is extremely fast, works on any device as long as you have an Internet connection.

### Motivation
At work, I needed to read a .msg file. Since I use a Mac, I quickly realized that this task wasn't straightforward. The official Outlook app on Mac doesn’t support .msg files and instead expects you to use a Windows machine or Outlook Web. Therefore, I decided to build a simple tool that would allow the following:
  - It must display the file’s content;
  - It must not rely on any server;
  - It must be fast.

### Features
  - Free (Open Source)
  - No Server, no data sharing
  - No analytics or tracking
  - No external calls of any kind
  - Extremely fast
  - Works on any device that can open the page

### Deployment

This site is deployed using **GitHub Pages** at [https://creedofman.github.io/msg-viewer/](https://creedofman.github.io/msg-viewer/).  
Automated updates and deployments are handled via a GitHub Actions workflow included in this repository for ease of maintenance and continuous delivery.

### Development

#### Build
The project uses Bun. To build it simply run:
```
bun .\build.ts
```
The command will put a final HTML in the `build` folder.

#### Branches
The repository uses the following branches:
 - `dev` - for development
 - `main` - for production (deployed to GitHub Pages)

---

**Original project:** https://github.com/molotochok/msg-viewer
