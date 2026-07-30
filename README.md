# 🕵️ BingDork Pro - Dork Collection

**781 Premium Dork Queries** ready for [BingDork Pro](https://github.com/mmojoj101-del/bingdork-pro-termux)

## 📂 Categories

| # | Category | Dorks | Description |
|---|----------|-------|-------------|
| 1 | SQL Injection | 26 | Find SQLi vulnerable parameters |
| 2 | XSS | 24 | Cross-Site Scripting vectors |
| 3 | LFI/RFI | 16 | File inclusion vulnerabilities |
| 4 | RCE | 15 | Remote code execution |
| 5 | Path Traversal | 10 | Directory traversal |
| 6 | Information Disclosure | 51 | Exposed directories |
| 7 | Sensitive Files | 58 | Passwords, configs, dumps |
| 8 | Admin Panels | 20 | Login pages |
| 9 | Exposed Databases | 15 | phpMyAdmin, Adminer |
| 10 | Backup Files | 30 | Old/backup files |
| 11 | Configuration Files | 20 | Server configs |
| 12 | Directory Listing | 45 | Open indexes |
| 13 | Open Redirects | 28 | Redirect parameters |
| 14 | Server Status | 30 | Error pages, debug |
| 15 | API Endpoints | 50 | REST, GraphQL, Swagger |
| 16 | Cloud/DevOps | 55 | AWS, Azure, GCP, Docker |
| 17 | IoT Cameras | 40 | Webcams, DVRs, IP cameras |
| 18 | WordPress | 32 | WP-specific |
| 19 | Joomla | 30 | Joomla-specific |
| 20 | Generic Vulns | 186 | Broad scanning |

## 🚀 Usage with BingDork Pro

```bash
# Install/Termux
cd ~/bingdork-pro-termux
git pull
make build

# Scan all dorks with thunder mode (20 workers)
./bingdork batch -f dorks.txt -p auto -w 20 -t txt -o results.txt

# Scan specific category
grep "^inurl:" dorks.txt > sqli.txt
./bingdork batch -f sqli.txt -p auto -w 10 -m 50 -t json -o sqli_results.json

# Scan with delay (stealth mode)
./bingdork batch -f dorks.txt -p bing -w 3 -d 2 -t txt -o stealth.txt
```

## 🎯 Tips

- Use `-w 20` for maximum speed (20 concurrent workers)
- Use `-m 50` to get 50 results per query
- Use `-p auto` to rotate between Bing/Google/DuckDuckGo/Brave
- Filter results with `grep` for specific domains

## 📦 Download

```bash
git clone https://github.com/mmojoj101-del/bingdork-pro-dorks.git
```

## ⚠️ Legal

For authorized security testing and bug bounty research only.
