# Spring Edge Worker

راه‌اندازی در یک کلیک 🚀

[![Deploy to Cloudflare Workers](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/eipro/spring)
---

## استفاده سریع برای کاربر نهایی

1. روی دکمه **Deploy to Cloudflare Workers** کلیک کن.
2. وارد Cloudflare شو (اگر لاگین نیستی).
3. Cloudflare به‌صورت خودکار پروژه را ایمپورت و Deploy می‌کند.
4. بعد از Deploy، فقط مقدار `UUID` را در Variables ست کن.

---

## Environment Variables

- `UUID` (ضروری)
- `PROXYIP` (اختیاری)
- `SOCKS5_ENABLED` (اختیاری: `true/false`)
- `SOCKS5_ADDRESS` (اختیاری: فرمت `[user:pass@]host:port`)
- `SOCKS5` (اختیاری، حالت قدیمی: اگر `true/false` باشد مثل فلگ رفتار می‌کند، اگر آدرس باشد به‌عنوان `SOCKS5_ADDRESS` در نظر گرفته می‌شود)
- `SOCKS5_RELAY` (اختیاری)
- `SCAMALYTICS_USERNAME` (اختیاری)
- `SCAMALYTICS_API_KEY` (اختیاری)
- `SCAMALYTICS_BASEURL` (اختیاری)

---

## مسیرهای اصلی

- `/<UUID>`
- `/xray/<UUID>`
- `/sb/<UUID>`
- `/scamalytics-lookup?ip=1.1.1.1`
