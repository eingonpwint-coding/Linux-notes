## 13. Sudo and Sudoers

`sudo` က command ကို administrator/root permission နဲ့ run ပေးပါတယ်။

```bash
sudo useradd testuser
sudo chmod 755 directory
sudo apt update
```

Sudo configuration files—

```text
/etc/sudoers
/etc/sudoers.d/
```

Sudoers ကို လုံခြုံစွာပြင်ရန်—

```bash
sudo visudo
```

### Sudoers Rule

```sudoers
%sudo ALL=(ALL:ALL) ALL
```

| Part | Meaning |
|---|---|
| `%sudo` | `sudo` group members |
| First `ALL` | All hosts |
| `(ALL:ALL)` | Run as any user and group |
| Last `ALL` | All commands |

### Easy Memory

```text
sudo group → Every host → Any user/group → Every command
```

User ကို sudo group ထဲထည့်ရန်—

```bash
sudo usermod -aG sudo thura
```

ပြီးနောက် logout/login ပြန်လုပ်ပါ။

အောက်က error—

```text
thura is not in the sudoers file
```

ဆိုတာ `thura` မှာ sudo permission မရှိတာဖြစ်ပါတယ်။

---

[Back to Home](../README.md)