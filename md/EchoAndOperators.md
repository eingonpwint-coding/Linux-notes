## 5. Echo and Operators

Text ပြရန်—

```bash
echo "Hello Linux"
```

### `>` — Overwrite

```bash
echo "Hello" > notes.txt
```

File ရှိပြီးသားဆိုရင် အရင် contents ကိုဖျက်ပြီး အသစ်ရေးပါတယ်။

### `>>` — Append

```bash
echo "Second line" >> notes.txt
```

ရှိပြီးသားစာရဲ့အောက်မှာ ထပ်ထည့်ပါတယ်။

### `|` — Pipe

ပထမ command ရဲ့ output ကို နောက် command ဆီပို့ပါတယ်။

```bash
cat /etc/passwd | grep testuser
```

### `&&` — Success ဖြစ်မှဆက်လုပ်

```bash
mkdir test && cd test
```

### `||` — Fail ဖြစ်မှဆက်လုပ်

```bash
cd test || echo "Directory not found"
```

### `;` — Success/Fail မစဉ်းစားဘဲဆက်လုပ်

```bash
pwd; ls
```

### Operators Summary

| Operator | Purpose |
|---|---|
| `>` | Replace/overwrite |
| `>>` | အောက်မှာထပ်ထည့် |
| `\|` | Output ကိုနောက် command ဆီပို့ |
| `&&` | ပထမ command success ဖြစ်မှဆက် |
| `\|\|` | ပထမ command fail ဖြစ်မှဆက် |
| `;` | ဘာဖြစ်ဖြစ်ဆက်လုပ် |

Quote မပိတ်မိလို့ `>` prompt ပေါ်လာလျှင်—

```text
Ctrl + C
```

နှိပ်ပြီး cancel လုပ်ပါ။

---
