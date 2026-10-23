## 16. Shell Scripts

ဥပမာ `hello.sh`—

```bash
#!/bin/bash
echo "Hello Linux"
```

Bash နဲ့ run ရန်—

```bash
bash hello.sh
```

Directly run ရန် execute permission အရင်ပေးပါ။

```bash
chmod +x hello.sh
./hello.sh
```

`./` ဆိုတာ current directory ထဲက file ကိုဆိုလိုပါတယ်။

`Permission denied` ဖြစ်ရင်—

```bash
ls -l hello.sh
chmod +x hello.sh
```

နဲ့စစ်ပါ။

---

[Back to Home](../README.md)
