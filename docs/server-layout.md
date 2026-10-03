# Server layout (file locations)

Everything lives in a tidy, predictable layout. You can also see this any time
from **Manage → File Locations** in the CLI.

| Path | What |
|------|------|
| `/root/BackSpeed` | The release bundle and downloaded archives. |
| `/root/BackSpeed/backups` | [Backup](backup-restore.md) `.tar.gz` files. |
| `/etc/backspeed` | Tunnel configs (one `.toml` per tunnel) and runtime state. |
| `/usr/local/bin/backspeed` | The binary itself. |
| `backspeed-<name>.service` | A systemd unit per tunnel. |
| `backspeed-monitor.service` | The [monitor service](monitor-service.md). |

The install directory is recorded in `/etc/backspeed/install_path`, which is what
the uninstaller reads to know what to remove.

---

<div dir="rtl">

## خلاصهٔ فارسی

همه‌چیز در یک ساختار مرتب و قابل‌پیش‌بینی است. همین را هر وقت خواستی از
`Manage → File Locations` در CLI هم می‌بینی.

`‎/root/BackSpeed` بستهٔ ریلیز و آرشیوهای دانلودشده ·
`‎/root/BackSpeed/backups` فایل‌های [پشتیبان](backup-restore.md) ·
`‎/etc/backspeed` کانفیگ تونل‌ها (برای هر تونل یک فایل `.toml`) و وضعیت اجرا ·
`‎/usr/local/bin/backspeed` خودِ باینری ·
`backspeed-<name>.service` یک یونیت systemd به‌ازای هر تونل ·
`backspeed-monitor.service` [سرویس مانیتور](monitor-service.md).

مسیر نصب در `/etc/backspeed/install_path` ثبت می‌شود و حذف‌کنندهٔ داخلی از روی
همان می‌فهمد چه چیزی را پاک کند.

</div>

---
[← Back to the docs index](README.md)

---

*Last verified against BackSpeed v1.8.5.*
