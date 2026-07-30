# 🕵️ BingDork Pro - 100K Premium Dork Collection

**100,000 unique, validated search queries** for [BingDork Pro](https://github.com/mmojoj101-del/bingdork-pro-termux)

## 📊 Stats
- **Total**: 100,000 queries
- **Generated**: via combinatoric wordlist expansion
- **Categories**: 10 curated sets (10K-15K each)
- **Size**: ~3.5MB compressed

## 🚀 Quick Start

```bash
# Clone the dorks
git clone https://github.com/mmojoj101-del/bingdork-pro-dorks.git
cd bingdork-pro-dorks

# Install bingdork
cd ~/bingdork-pro-termux
git pull && make build

# Scan ALL 100K dorks with Thunder mode ⚡
cd ~/bingdork-pro-dorks
~/bingdork-pro-termux/build/bingdork batch \
  -f dorks.txt -p auto -w 20 -t txt -o results.txt

# Or scan specific categories
~/bingdork-pro-termux/build/bingdork batch \
  -f categories/04-sensitive.txt -p auto -w 15 -m 50 -t json -o sensitive.json

# Stealth mode (slow, undetected)
~/bingdork-pro-termux/build/bingdork batch \
  -f categories/02-filetype.txt -p bing -w 1 -d 3 -t txt -o stealth.txt
```

## 📁 Structure

```
dorks.txt            ← All 100K dorks (one per line)
categories/
├── 01-inurl.txt          (15K) - URL parameter injections
├── 02-filetype.txt       (15K) - File type searches
├── 03-intitle.txt        (15K) - Title searches
├── 04-sensitive.txt      (10K) - Passwords, keys, secrets
├── 05-admin.txt          (10K) - Admin panels, login pages
├── 06-database.txt       (10K) - SQL, database files
├── 07-technologies.txt   (10K) - PHP, ASP, CMS specific
├── 08-backup.txt         (10K) - Backup & old files
├── 09-top-tlds.txt       (10K) - .com, .net, .org, .edu
└── 10-config.txt         (10K) - Config & setup files
```

## ⚙️ Best Practices

| Goal | Workers | Delay | Provider | File |
|------|---------|-------|----------|------|
| 🔥 Maximum speed | `-w 20` | `-d 0` | `auto` | `dorks.txt` |
| ⚡ Fast scan | `-w 10` | `-d 0` | `auto` | `categories/*.txt` |
| 🐢 Stealth | `-w 1` | `-d 3` | `bing` | `small files` |
| 🎯 Targeted | `-w 5` | `-d 1` | `auto` | Single category |

## 🔗 Related Repos
- [BingDork Pro (Termux)](https://github.com/mmojoj101-del/bingdork-pro-termux)
- [BingDork Pro (Desktop)](https://github.com/mmojoj101-del/bingdork-pro-desktop)

## ⚠️ Legal
For authorized security testing and bug bounty research only.
