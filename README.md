# 👻 TorForTerminal

> A minimalist, privacy-focused terminal web viewer powered by Tor.
> **Kodlayan:** [Padros](https://github.com/Padrosum)

![Bash](https://img.shields.io/badge/Language-Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Tor](https://img.shields.io/badge/Network-Tor-7D4698?style=for-the-badge&logo=tor-browser&logoColor=white)
![Privacy](https://img.shields.io/badge/Focus-Privacy-000000?style=for-the-badge)

---

## 📖 Nedir?

**TorForTerminal**, terminalinizden çıkmadan web sitelerini **anonim**, **reklamsız** ve **JavaScript olmadan** okumanızı sağlayan basit bir Bash scriptidir.

Tüm trafiği `torsocks` aracılığıyla **Tor Ağı** üzerinden geçirir. `curl` ile veriyi çeker ve `w3m` ile terminalde render eder.

### ✨ Özellikler

* 🛡️ **Tam Anonimlik:** Tüm istekler Tor çıkış düğümleri (exit nodes) üzerinden yapılır.
* 🕵️ **User-Agent Spoofing:** Kendini standart bir Windows/Firefox kullanıcısı olarak gizler, böylece "bot" korumalarına takılmaz.
* 🚫 **No-JS:** JavaScript çalıştırmaz. İzleyiciler (trackers), reklamlar ve kötü amaçlı scriptler engellenir.
* 🚀 **Hız:** Görselleri ve ağır CSS dosyalarını yoksayar, sadece saf bilgiye odaklanır.

---

## ⚠️ Yasal Uyarı (Disclaimer)

Bu yazılım **yalnızca eğitim amaçlı** ve **kişisel gizlilik araştırmaları** için geliştirilmiştir.

* Bu script, **Tor Browser'ın sunduğu tam kapsamlı güvenliği ve anonimliği (OpSec) garanti etmez.**
* Kullanıcı, bu aracı kullanarak gerçekleştirdiği tüm eylemlerden yasal ve teknik olarak **tek başına sorumludur.**
* Geliştirici (**Padros**), bu aracın kötü amaçlı kullanımından veya doğabilecek herhangi bir zarardan sorumlu tutulamaz.

---

## 🛠️ Gereksinimler (Dependencies)

Bu aracı kullanabilmek için aşağıdaki paketlerin sisteminizde yüklü olması gerekir:

* `tor` (Servis olarak çalışıyor olmalı)
* `torsocks`
* `curl`
* `w3m`

**Arch Kurulum:**
```bash
sudo pacman -S tor torsocks curl w3m
sudo systemctl start tor
