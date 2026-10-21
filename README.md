# Linux Learning Notes

ဒီ repository မှာ Linux administration အခြေခံ commands၊ users၊ groups၊ permissions၊ sudo နှင့် shell scripts အကြောင်း လေ့လာထားတဲ့ notes တွေကို စုစည်းထားပါတယ်။

---

## Linux Notes List

| No. | Topic | Description |
|---:|---|---|
| 1 | [Linux Basic Notes](md/linux-note.md) | Linux အခြေခံမှတ်စုများ |
| 2 | [Directory Navigation](md/Directory%20Navigation.md) | `cd`, `pwd`, `.`, `..`, `~` နှင့် directory navigation |
| 3 | [Absolute and Relative Paths](md/Absolute-Relative-Paths.md) | Absolute path နှင့် relative path ကွာခြားချက် |
| 4 | [View Files and Directories](md/View-file-and-Directories.md) | `ls`, `ls -l`, `ls -a` နှင့် file listing commands |
| 5 | [File and Directory Operations](md/FileAndDirectoriesOperations.md) | `touch`, `mkdir`, `cp`, `mv`, `rm` commands |
| 6 | [Echo and Operators](md/EchoAndOperators.md) | `echo`, `>`, `>>`, pipe, `&&`, `||` နှင့် `;` |
| 7 | [Linux User Information](md/linux-user-information.md) | UID, GID, `/etc/passwd`, shell နှင့် Home directory |
| 8 | [User Management](md/User-Management.md) | `useradd`, `usermod`, `passwd`, `userdel` commands |
| 9 | [Group Management](md/Group-Management.md) | `groupadd`, `groupdel`, primary နှင့် supplementary groups |
| 10 | [Owner and Group](md/Owner-And-Group.md) | `chown`, `chgrp` နှင့် file ownership |
| 11 | [Linux Permissions](md/Permession.md) | Owner, group, others နှင့် `rwx` permissions |
| 12 | [Permission Denied](md/Permession-Denied.md) | Permission denied ဖြစ်ရတဲ့အကြောင်းရင်းနှင့် ဖြေရှင်းနည်း |
| 13 | [Sudo and Sudoers](md/Sudo-And-Sudores.md) | `sudo`, sudo group နှင့် `/etc/sudoers` |
| 14 | [Shell Scripts](md/Shell-Scripts.md) | `.sh` files၊ execute permission နှင့် script run နည်း |
| 15 | [Hard Link and Soft Link](md/HardLink-And-SoftLink.md) | Hard link နှင့် symbolic link ကွာခြားချက် |
| 16 | [Terminal Colours](md/Terminal-Colours.md) | Terminal file နှင့် directory colours |
| 17 | [Common Mistakes](md/Common-mistakes.md) | Linux commands သုံးရာတွင် ဖြစ်လေ့ရှိတဲ့အမှားများ |

---

## Important Commands

| Purpose | Command |
|---|---|
| Check current user | `whoami` |
| Check current location | `pwd` |
| List files | `ls -l` |
| Go to Home | `cd ~` |
| Create user | `sudo useradd -m -s /bin/bash username` |
| Create group | `sudo groupadd groupname` |
| Add user to group | `sudo usermod -aG groupname username` |
| Change owner | `sudo chown owner file` |
| Change group | `sudo chgrp group file` |
| Change permission | `chmod 755 file` |
| Edit sudoers safely | `sudo visudo` |

---

## Permission Memory

```text
r = Read    = 4
w = Write   = 2
x = Execute = 1
```

```text
7 = rwx
6 = rw-
5 = r-x
4 = r--
0 = ---
```

---

## Learning Flow

```text
Linux Basics
    ↓
Files and Directories
    ↓
Users and Groups
    ↓
Ownership
    ↓
Permissions
    ↓
Sudo and Sudoers
    ↓
Shell Scripts
```