## 14. Permission Denied

အောက်က directory permission ကိုကြည့်ပါ။

```text
drwxr-x--- eingonpwint eingonpwint
```

| User Class | Permission |
|---|---|
| Owner `eingonpwint` | `rwx` |
| Group `eingonpwint` | `r-x` |
| Others | `---` |

`thura` က owner မဟုတ်၊ `eingonpwint` group member မဟုတ်ရင်—

```bash
cd /home/eingonpwint
```

လုပ်တဲ့အခါ—

```text
Permission denied
```

ဖြစ်နိုင်ပါတယ်။

စစ်ရန်—

```bash
ls -ld /home/eingonpwint
id thura
```

---

[Back to Home](../README.md)
