## 6. Linux User Information

User account information ကို အောက်က file ထဲမှာထားပါတယ်။

```text
/etc/passwd
```

ဖတ်ရန်—

```bash
cat /etc/passwd
```

User တစ်ယောက်တည်းရှာရန်—

```bash
getent passwd eingonpwint
```

ဥပမာ—

```text
eingonpwint:x:1001:1001:Ei Ngon:/home/eingonpwint:/bin/bash
```

| Field | Meaning |
|---|---|
| `eingonpwint` | Username |
| `x` | Password information ကို `/etc/shadow` မှာထားသည် |
| `1001` | UID |
| `1001` | Primary GID |
| `Ei Ngon` | Full name/comment |
| `/home/eingonpwint` | Home directory |
| `/bin/bash` | Login shell |

Encrypted password information ကို—

```text
/etc/shadow
```

ထဲမှာထားပါတယ်။

### `/etc/passwd` ကိုဖတ်ခြင်း

မှန်သော command—

```bash
cat /etc/passwd
```

အောက်က command က မမှန်ပါဘူး။

```bash
sudo /etc/passwd
```

ဘာကြောင့်လဲဆိုတော့ `sudo` က `/etc/passwd` ကို program လို execute လုပ်ဖို့ ကြိုးစားတာဖြစ်ပါတယ်။

---