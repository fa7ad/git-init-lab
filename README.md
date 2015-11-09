# git-init-lab
---

Initialize an empty git repo both **locally** and on [**gitlab**](https://gitlab.com/)

## Requirements
---

1. [jq](https://stedolan.github.io/jq/download/)
2. [git](http://www.git-scm.com/download/)
3. [curl](http://curl.haxx.se/download.html#LinuxUbuntu)

#### On Ubuntu

```bash
 sudo apt-get install jq git curl
```

## Installation
---
* **Download the main file**

```bash
 sudo curl -fsSL -o /usr/local/bin/git-init-lab https://raw.github.com/fa7ad/git-init-lab/master/git-init-lab
```

* **Make the downloaded file executable**

```bash
 sudo chmod +x /usr/local/bin/git-init-lab
```

* **Create the config file and populate it**

```
 nano ~/.gitlab.token
 # Paste in the private key from https://gitlab.com/profile/account and save the file using ^O and then exit using ^X
```

* **Done**
  Now, use either **git init-lab** or **git-init-lab**

## Usage

```bash
 git-init-lab <repo name> <Project description>
```
**Example:**
```bash
 git-init-lab my-config "My personal configuration files"
```

## License

[GPL3](https://www.gnu.org/copyleft/gpl.html)
