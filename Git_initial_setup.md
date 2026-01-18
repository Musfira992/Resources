### 1. Install Git

**Windows**

- Download the installer from https://git-scm.com/downloads
- Run it with default options (it’ll install Git Bash, which gives you a Linux-like shell).


### 2. Configure Git (Name & Email)

```
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

Check your settings:

```
git config --list
```

### 3. Create an SSH Key

This allows GitHub to authenticate you without typing your password every time.

```
ssh-keygen -t ed25519 -C "your_email@example.com"
```
- Press Enter to accept the default file location (~/.ssh/id_ed25519).

- Choose a passphrase if you want extra security (or just press Enter to skip).

Start the ssh-agent:
```
eval "$(ssh-agent -s)"
```
Add your key to the agent:
```
ssh-add ~/.ssh/id_ed25519
```
Copy the public key to your clipboard:
```
cat ~/.ssh/id_ed25519.pub
```
(copy the entire line starting with ssh-ed25519)

### 4. Add SSH Key to GitHub
- Go to GitHub → Settings → SSH and GPG keys.

- Click New SSH Key, paste the key, give it a name, save.
Test the connection:
```
ssh -T git@github.com
```
You should see something like:
```
Hi your-username! You've successfully authenticated...
```

### 5. Create a Local Repository
Inside your project folder:
```
cd path/to/your/project
git init
```
This creates a .git folder — Git is now tracking this directory.


### Debug - Extra command

```
git remote set-url origin git@github.com:username/repo-name.git
```
