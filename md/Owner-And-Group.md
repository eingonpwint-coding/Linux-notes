## 9. Owner and Group

File တစ်ခုမှာ—

```text
Owner + Group + Permission
```

ရှိပါတယ်။

### Owner တစ်ခုပဲပြောင်းရန်

```bash
sudo chown testuser notes.txt
```

### Owner နဲ့ Group နှစ်ခုလုံးပြောင်းရန်

```bash
sudo chown testuser:developer notes.txt
```

Command pattern—

```text
chown owner:group filename
```

### Group တစ်ခုပဲပြောင်းရန်

```bash
sudo chgrp developer notes.txt
```

### Memory Note

```text
chown = Change owner
chgrp = Change group
chmod = Change permission
```

---