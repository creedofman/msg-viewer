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
This library allows you to read Outlook `.msg` files in the browser.

### Install
Simply run this command in your terminal:
```
npm i @molotochok/msg-viewer
```

### Usage
First import the library:

```js
import { parse } from "@molotochok/msg-viewer";
```

Then parse the input array buffer:
```js
const message = parse(new DataView(arrayBuffer));
```

The result is an object that contains relevant information about the message. Its structure is defined [here](https://github.com/molotochok/msg-viewer/blob/main/lib/scripts/msg/types/message.d.ts).

### Example
Refer to this [page](https://github.com/molotochok/msg-viewer/blob/main/lib/scripts/index.ts#L34) for the example usage of this library in the live experience.

### Repository
You can find the source code on [Github](https://github.com/molotochok/msg-viewer).

---

**Note on Deployment:**  
The demo site is deployed via **GitHub Pages** (not Cloudflare).  
Automated updates and deployments are handled via a GitHub Actions workflow included in this repository.

---

**Original project:** https://github.com/molotochok/msg-viewer