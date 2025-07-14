# pdlx-release

**pdlx-release** یک بسته برندینگ رسمی برای توزیع [PdLinuXOS](https://pdlx.ir) است که فایل‌های شناسایی سیستم، لوگو، و پیکربندی پوسته Nushell و Fastfetch را فراهم می‌کند.

---

## 📦 محتویات پکیج

| فایل | مسیر نصب | توضیح |
|------|-----------|--------|
| `os-release` | `/etc/os-release` | اطلاعات استاندارد سیستم |
| `lsb-release` | `/etc/lsb-release` | اطلاعات برای `lsb_release -a` |
| `issue` | `/etc/issue` | نمایش لوگو و پیام هنگام ورود به tty |
| `pdlinuxos.txt` | `/usr/share/neofetch/ascii/` | لوگوی ASCII برای neofetch |
| `pdlinuxos.png` | `/usr/share/pixmaps/` | لوگوی تصویری سیستم (برای SDDM, Calamares, درباره سیستم و...) |
| `config.nu` | `/etc/skel/.config/nushell/` | اجرای خودکار `fastfetch` در ترمینال Nushell |
| `.bash_profile` | `/etc/skel/` | اجرای Nushell به‌صورت پیش‌فرض برای کاربران جدید |

---

## 🧱 وابستگی‌ها

این بسته به صورت خودکار پکیج‌های زیر را نصب می‌کند:

- [`fastfetch`](https://archlinux.org/packages/community/x86_64/fastfetch/)
- [`nushell`](https://archlinux.org/packages/community/x86_64/nushell/)

---

## ⚙️ نصب

برای ساخت و نصب پکیج:

```bash
git clone https://github.com/pdlinux/pdlx-release.git
cd pdlx-release
makepkg -si
