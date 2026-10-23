### Operators Summary

| Operator | Name | Purpose |
|---|---|---|
| `>` | Output Redirection | stdout ကို File ထဲရေးသည်။ ရှိပြီးသားစာကို အစားထိုးသည် |
| `>>` | Append Redirection | stdout ကို File ၏ နောက်ဆုံးတွင် ထပ်ဖြည့်သည် |
| `<` | Input Redirection | File ထဲက အချက်အလက်ကို stdin အဖြစ် ယူသည် |
| `2>` | Error Redirection | stderr ကို File ထဲရေးသည် |
| `\|` | Pipe | ဘယ်ဘက် Command ၏ stdout ကို ညာဘက် Command ၏ stdin သို့ ပို့သည် |
| `&&` | Logical AND | ပထမ Command အောင်မြင်မှ နောက် Command ကို Run သည် |
| `\|\|` | Logical OR | ပထမ Command မအောင်မြင်မှ နောက် Command ကို Run သည် |
| `;` | Semicolon / Command Separator | ပထမ Command အောင်မြင်/မအောင်မြင် မရွေး၊ ပြီးလျှင် နောက် Command ကို Run သည် |

### အသုံးပြုပုံ ဥပမာများ

#### 1. Output Redirection — `>`

```bash
echo "Hello Linux" > notes.txt
```

- `Hello Linux` ဆိုသည့် stdout ကို `notes.txt` ထဲ ရေးသည်။
- File မရှိသေးလျှင် ဖန်တီးပေးသည်။
- File ရှိပြီးသားဆို မူလစာများကို အစားထိုးသည်။

#### 2. Append Redirection — `>>`

```bash
echo "Learning Linux" >> notes.txt
```

မူလစာများကို ထိန်းထားပြီး နောက်ဆုံးတွင် စာထပ်ဖြည့်သည်။

#### 3. Input Redirection — `<`

```bash
sort < notes.txt
```

`notes.txt` ထဲက စာကြောင်းများကို `sort` ၏ stdin အဖြစ်ပေးပြီး စီထားသည့်ရလဒ်ကို Terminal တွင် ပြသည်။ မူလ File ကို မပြင်ပါ။

#### 4. Error Redirection — `2>`

```bash
ls /folder_that_does_not_exist 2> errors.txt
```

Folder မရှိကြောင်း Error message ကို `errors.txt` ထဲ သိမ်းသည်။

#### 5. Pipe — `|`

```bash
ls /home | sort
```

- `ls /home` က ထုတ်ပေးသည့် stdout ကို `sort` ဆီ ပို့သည်။
- `sort` က အဲဒီအချက်အလက်ကို stdin အဖြစ် လက်ခံပြီး စီပေးသည်။

> Pipe သည် ပုံမှန်အားဖြင့် stdout ကိုသာ ပို့သည်။ stderr ကို အလိုအလျောက် မပို့ပါ။

#### 6. Logical AND — `&&`

```bash
mkdir demo && cd demo
```

`demo` folder ဖန်တီးခြင်း အောင်မြင်မှ `cd demo` ကို ဆက် Run သည်။

#### 7. Logical OR — `||`

```bash
cat missing.txt || echo "Cannot read file"
```

`cat missing.txt` မအောင်မြင်မှ `Cannot read file` ကို ပြသည်။

#### 8. Semicolon — `;`

```bash
pwd ; whoami
```

`pwd` ပြီးလျှင် အောင်မြင်/မအောင်မြင် မရွေး `whoami` ကို ဆက် Run သည်။

> Command ခွဲရန် Semicolon တစ်ခု `;` သုံးပါ။ `;;` သည် Bash ၏ `case` statement တွင် သုံးသည့် သီးခြားသင်္ကေတ ဖြစ်သည်။

### မှတ်မိရန်

- `>` → File ထဲ အစားထိုးရေး
- `>>` → File နောက်ဆုံးမှာ ထပ်ဖြည့်
- `<` → File မှ Input ယူ
- `2>` → Error ကို File ထဲရေး
- `|` → Output ကို နောက် Command ဆီပို့
- `&&` → အောင်မြင်မှ ဆက်လုပ်
- `||` → မအောင်မြင်မှ ဆက်လုပ်
- `;` → ပြီးလျှင် ဆက်လုပ်

### Quote မပိတ်မိလို့ `>` Prompt ပေါ်လာလျှင်

ဥပမာ Quote မပိတ်ဘဲ Enter နှိပ်မိလျှင်—

```bash
echo "Hello
>
```

ဒီနေရာက `>` သည် Redirection operator မဟုတ်ပါ။
Command မပြီးသေးလို့ Shell က ဆက်ရိုက်ရန် စောင့်နေသည့် Prompt ဖြစ်သည်။

`Ctrl + C` နှိပ်ပြီး Cancel လုပ်နိုင်သည်။

---

[Back to Home](../README.md)