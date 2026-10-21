## 8. Group Management

Group ဖန်တီးရန်—

```bash
sudo groupadd developer
```

User ကို supplementary group ထဲထည့်ရန်—

```bash
sudo usermod -aG developer testuser
```

User ကို sudo group ထဲထည့်ရန်—

```bash
sudo usermod -aG sudo testuser
```

Primary group ပြောင်းရန်—

```bash
sudo usermod -g developer testuser
```

User ပါဝင်တဲ့ groups စစ်ရန်—

```bash
groups testuser
```

သို့မဟုတ်—

```bash
id testuser
```

Group ဖျက်ရန်—

```bash
sudo groupdel developer
```

### `-aG` Meaning

```text
-a = Append
-G = Supplementary groups
```

`-aG` က လက်ရှိ supplementary groups မဖယ်ဘဲ group အသစ်ထပ်ထည့်တာဖြစ်ပါတယ်။

---
