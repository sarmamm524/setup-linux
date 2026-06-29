# Linux Setup Guide

A step-by-step guide to setting up a Linux development environment with Chrome, VS Code, Git, and GitHub SSH access.

---

## 1. Install Google Chrome
```bash
cd Downloads/
ls
sudo dpkg -i google-chrome-stable_current_amd64.deb
```

---

## 2. Install Visual Studio Code

```bash
cd
sudo dpkg -i code_1.126.0-1782208079_amd64.deb
```

---

## 3. Update & Upgrade System Packages

```bash
sudo nano /etc/apt/sources.list.d/google-chrome.list
sudo apt update
sudo apt upgrade
```

---

## 4. Install Git

```bash
sudo apt install git
```

---

## 5. Configure Git

```bash
git config --global user.email "sarmamm.524@gmail.com"
git config --global user.name "sarmamm524"
```

---

## 6. Set Up SSH Key for GitHub

### Generate SSH Key

```bash
ssh-keygen -t rsa -b 4096 -C "sarmamm.524@gmail.com"
```

### Add key to SSH agent 

```bash
cat -/.ssh/id_rsa.pub
```

### Test GitHub connection

```bash
ssh -T git@github.com
```

---

## 7. Clone Repository

```bash
git clone git@github.com: sarmamm524/setup-linux.git
ls
cd setup-linux/
```