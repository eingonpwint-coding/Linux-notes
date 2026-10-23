## 7. User Management

### User ဖန်တီးခြင်း

```bash
sudo useradd -m -s /bin/bash testuser
```

Password သတ်မှတ်ရန်—

```bash
sudo passwd testuser
```

| Option | Meaning |
|---|---|
| `-m` | Home directory ဖန်တီးရန် |
| `-s /bin/bash` | Login shell သတ်မှတ်ရန် |
| `-u 1200` | Custom UID သတ်မှတ်ရန် |
| `-g developer` | Primary group သတ်မှတ်ရန် |
| `-G group1,group2` | Supplementary groups သတ်မှတ်ရန် |

Custom UID နဲ့ user ဖန်တီးရန်—

```bash
sudo useradd -m -u 1200 -s /bin/bash testuser
```

Ubuntu interactive method—

```bash
sudo adduser testuser
```

### Login Shell ပြောင်းခြင်း

```bash
sudo usermod -s /bin/bash testuser
```

Current user ရဲ့ shell ပြောင်းရန်—

```bash
chsh -s /bin/bash
```

### User ဖျက်ခြင်း

User account တစ်ခုပဲဖျက်ရန်—

```bash
sudo userdel testuser
```

User နဲ့ Home directory ပါဖျက်ရန်—

```bash
sudo userdel -r testuser
```

> `userdel -r` သုံးရင် user ရဲ့ Home directory နဲ့ data တွေပါ ပျက်နိုင်ပါတယ်။

### Command Spacing

မမှန်—

```bash
sudo useradd testuser -s/bin/bash
```

မှန်—

```bash
sudo useradd -m -s /bin/bash testuser
```

`-s` နဲ့ `/bin/bash` ကြားမှာ space ရှိရပါတယ်။

---

[Back to Home](../README.md)
