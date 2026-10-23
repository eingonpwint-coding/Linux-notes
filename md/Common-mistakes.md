## 18. Common Mistakes

| Wrong/Problem | Correct/Explanation |
|---|---|
| `cd home` | System Home အတွက် `cd /home` သုံးရန် |
| `cd ein` | Full directory name `cd eingonpwint` သုံးရန် |
| `sudo /etc/passwd` | `cat /etc/passwd` သုံးရန် |
| `useradd -s/bin/bash` | `useradd -s /bin/bash` သုံးရန် |
| `chmod 666 directory` | Directory မှာ `x` လိုလို့ `755`, `750` သို့မဟုတ် `700` သုံးရန် |
| `./script.sh` Permission denied | `chmod +x script.sh` အရင်လုပ်ရန် |
| Quote မပိတ်လို့ `>` ပေါ် | Quote ပိတ် သို့မဟုတ် `Ctrl + C` နှိပ်ရန် |
| User က sudo သုံးမရ | Authorized account နဲ့ user ကို `sudo` group ထဲထည့်ရန် |

---

# Final Memorization Card

```text
User → Group → Ownership → Permission
```

```text
Permission = Owner | Group | Others
```

```text
r = 4
w = 2
x = 1

7 = rwx
6 = rw-
5 = r-x
4 = r--
0 = ---
```

| Need | Command |
|---|---|
| Go to own Home | `cd` or `cd ~` |
| Go to system Home | `cd /home` |
| Check current location | `pwd` |
| Check current user | `whoami` |
| Check user details | `id username` |
| Create user | `sudo useradd -m -s /bin/bash username` |
| Set password | `sudo passwd username` |
| Create group | `sudo groupadd groupname` |
| Add user to group | `sudo usermod -aG group user` |
| Change owner | `sudo chown owner file` |
| Change owner and group | `sudo chown owner:group file` |
| Change group | `sudo chgrp group file` |
| Change permission | `chmod 755 file` |
| Make script executable | `chmod +x script.sh` |
| Run current script | `./script.sh` |
| Edit sudoers safely | `sudo visudo` |
| Read user database | `cat /etc/passwd` |
| Create hard link | `ln source link` |
| Create soft link | `ln -s source link` |

## Three Commands to Remember

```text
chown = Change owner
chgrp = Change group
chmod = Change permission
```
[Back to Home](../README.md)