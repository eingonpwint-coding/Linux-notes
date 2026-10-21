## 3. Viewing Files and Directories

| Command | Purpose |
|---|---|
| `ls` | Files နှင့် directories ကြည့်ရန် |
| `ls -l` | Permission, owner, group အပါအဝင်ကြည့်ရန် |
| `ls -a` | Hidden files ပါကြည့်ရန် |
| `ls -la` | Hidden files နှင့် details အားလုံးကြည့်ရန် |
| `ls -ld directory` | Directory ကိုယ်တိုင်ရဲ့ details ကြည့်ရန် |
| `ls -li` | Inode number ပါကြည့်ရန် |

ဥပမာ—

```text
-rw-r----- 1 eingonpwint developer 120 notes.txt
```

| Part | Meaning |
|---|---|
| `-` | File type |
| `rw-r-----` | Permissions |
| `eingonpwint` | Owner |
| `developer` | Group |
| `120` | File size |
| `notes.txt` | Filename |