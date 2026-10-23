## 17. Hard Link and Soft Link

### Hard Link

```bash
ln original.txt hardlink.txt
```

### Soft Link

```bash
ln -s original.txt softlink.txt
```

| Point | Hard Link | Soft Link |
|---|---|---|
| Command | `ln` | `ln -s` |
| Inode | တူ | မတူ |
| Original file ဖျက်လျှင် | အလုပ်လုပ်ဆဲ | Broken link |
| Directory link | ပုံမှန်အားဖြင့်မလုပ် | လုပ်နိုင် |
| Filesystem ကျော်နိုင် | မရ | ရ |
| Easy meaning | File ရဲ့နာမည်နောက်တစ်ခု | Shortcut |

Inode စစ်ရန်—

```bash
ls -li
```

---

[Back to Home](../README.md)

