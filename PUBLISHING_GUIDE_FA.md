# راهنمای انتشار ESPFlight Hardware Reference v1.0

## GitHub Repository

ریپازیتوری Hardware Reference را Public نگه دارید و فایل‌های این بسته را در ریشه Repository قرار دهید.

ساختار پیشنهادی:

```text
README.md
LICENSE
NOTICE.md
RELEASE_NOTES.md
EASYEDA_DESCRIPTION.txt
CHECKSUMS.sha256

docs/
└── ASSEMBLY_NOTES.md

fabrication/
├── gerber/
│   └── ESPFlight_Hardware_Reference_v1.0_Gerber.zip
├── bom/
│   └── ESPFlight_Hardware_Reference_v1.0_BOM.csv
└── pick-and-place/
    └── ESPFlight_Hardware_Reference_v1.0_PickAndPlace.csv
```

اگر فایل Editable پروژه EasyEDA را نیز Export می‌کنید، آن را در پوشه `design/` قرار دهید. پروژه عمومی EasyEDA باید منبع اصلی قابل ویرایش محسوب شود.

## GitHub Release

در GitHub به بخش Releases بروید و یک Release جدید ایجاد کنید:

- Tag: `hardware-v1.0`
- Release title: `ESPFlight Hardware Reference v1.0`
- Target: شاخه اصلی Repository
- وضعیت: Latest release

متن `RELEASE_NOTES.md` را برای توضیحات Release استفاده کنید.

سه فایل fabrication را می‌توانید علاوه بر حضور در Repository، به‌صورت Asset هم به Release اضافه کنید تا دانلود مستقیم برای کاربران ساده باشد.

## EasyEDA

در پروژه EasyEDA:

- Title: `ESPFlight Hardware Reference v1.0`
- Version/Revision: `v1.0`
- Description: محتوای `EASYEDA_DESCRIPTION.txt`
- License: `CERN-OHL-P-2.0`
- لینک Firmware: `https://github.com/espflight/firmware`
- لینک Website: `https://espflight.com`

Gerber عمومی EasyEDA باید با Gerber موجود در این Release یکسان باشد.

## Freeze

بعد از انتشار v1.0، فایل‌های ساخت همین Revision را بدون تغییر جایگزین نکنید. اگر PCB یا مقدار/پارت قطعه‌ای تغییر کرد، Revision جدید مانند `v1.1` منتشر کنید.
