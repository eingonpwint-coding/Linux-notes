## 10. Permissions: Owner, Group and Others

Permission ကို သုံးပိုင်းခွဲပါတယ်။

```text
Owner | Group | Others
```

ဥပမာ—

```text
rwxr-x---
```

| User Class | Permission |
|---|---|
| Owner | `rwx` |
| Group | `r-x` |
| Others | `---` |

### File Permissions

| Permission | Meaning |
|---|---|
| `r` | File ဖတ်နိုင် |
| `w` | File ပြင်နိုင် |
| `x` | File/program run နိုင် |

### Directory Permissions

| Permission | Meaning |
|---|---|
| `r` | Directory ထဲက filenames ကြည့်နိုင် |
| `w` | Files create, delete, rename လုပ်နိုင် |
| `x` | Directory ထဲဝင်နိုင် |

Directory မှာ `x` မရှိရင် `cd` နဲ့ဝင်လို့မရပါဘူး။

---

## 11. Numeric Permissions

| Permission | Number |
|---|---:|
| `r` | 4 |
| `w` | 2 |
| `x` | 1 |
| `rwx` | 7 |
| `rw-` | 6 |
| `r-x` | 5 |
| `r--` | 4 |
| `---` | 0 |

### Common Permissions

| Number | Permission | Common Use |
|---:|---|---|
| `700` | `rwx------` | Private directory/script |
| `750` | `rwxr-x---` | Owner နှင့် group access |
| `755` | `rwxr-xr-x` | Directory/script |
| `644` | `rw-r--r--` | Normal text file |
| `600` | `rw-------` | Private file |
| `666` | `rw-rw-rw-` | Execute permission မရှိ |

ဥပမာ—

```bash
chmod 755 script.sh
chmod 644 notes.txt
chmod 700 private-directory
```

Directory ကို—

```bash
chmod 666 directory
```

မပေးသင့်ပါဘူး။ `x` မရှိတော့တာကြောင့် directory ထဲဝင်လို့မရနိုင်ပါဘူး။

Directory အတွက် အသုံးများတာ—

```bash
chmod 755 directory
chmod 750 directory
chmod 700 directory
```

---

## 12. Symbolic Permissions

| Symbol | Meaning |
|---|---|
| `u` | Owner/User |
| `g` | Group |
| `o` | Others |
| `a` | All |
| `+` | Permission ထည့် |
| `-` | Permission ဖယ် |
| `=` | Exact permission သတ်မှတ် |

Owner ကို execute permission ထည့်ရန်—

```bash
chmod u+x script.sh
```

User အားလုံးကို execute permission ထည့်ရန်—

```bash
chmod a+x script.sh
```

Group ကို write permission ထည့်ရန်—

```bash
chmod g+w notes.txt
```

Others permission အားလုံးဖယ်ရန်—

```bash
chmod o-rwx notes.txt
```

---