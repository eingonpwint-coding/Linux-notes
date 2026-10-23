## 4. File and Directory Operations

| Task | Command |
|---|---|
| Empty file ဖန်တီးရန် | `touch notes.txt` |
| File ဖန်တီးပြီး စာရေးရန် / ရှိပြီးသား File ပြင်ရန် | `vi notes.txt` |
| Directory ဖန်တီးရန် | `mkdir project` |
| File ဖတ်ရန် | `cat notes.txt` |
| File copy ကူးရန် | `cp file1.txt file2.txt` |
| Directory copy ကူးရန် | `cp -r dir1 dir2` |
| File rename လုပ်ရန် | `mv old.txt new.txt` |
| File move လုပ်ရန် | `mv file.txt directory/` |
| File ဖျက်ရန် | `rm file.txt` |
| Empty directory ဖျက်ရန် | `rmdir directory` |
| Directory နှင့် contents ဖျက်ရန် | `rm -r directory` |

> `rm -r` သုံးရာတွင် target directory ကို သေချာစစ်ပါ။ ဖျက်ထားတာကို ပုံမှန်အားဖြင့် Trash ထဲမှာပြန်မတွေ့နိုင်ပါ။

---


### vi ဖြင့် File ဖန်တီးပြီး စာရေးနည်း

1. `vi notes.txt` ရိုက်ပြီး Enter နှိပ်ပါ။
2. `i` နှိပ်ပြီး စာရေးပါ။
3. ရေးပြီးလျှင် `Esc` နှိပ်ပါ။
4. `:wq` ရိုက်ပြီး Enter နှိပ်ပါ။ သိမ်းပြီး ထွက်ပါမည်။

> File မရှိသေးလျှင် သိမ်းသည့်အချိန် အသစ်ဖန်တီးပေးမည်။ ရှိပြီးသားဆိုလျှင် ဖွင့်ပြင်နိုင်သည်။

| Command | Purpose |
|---------|---------|
| `i` | Insert mode ဝင်ပြီး စာရေးရန် |
| `Esc` | Normal mode သို့ ပြန်ဝင်ရန် |
| `:w` | သိမ်းရန် |
| `:wq` | သိမ်းပြီး ထွက်ရန် |
| `:q!` | ယခု ပြင်ထားသည်များကို မသိမ်းဘဲ ထွက်ရန် |

> `:w`, `:wq`, `:q!` ကို အသုံးမပြုမီ `Esc` အရင်နှိပ်ပါ။

[Back to Home](../README.md)