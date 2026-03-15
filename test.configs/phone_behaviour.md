# Phone Behaviour with Hiddify & REALITY

## رفتار گوشی با هیدیفای و REALITY | Phone Behaviour Guide

This document covers common phone behaviour patterns and troubleshooting steps when using Hiddify with the REALITY protocol.

این سند رفتارهای رایج گوشی و مراحل عیب‌یابی هنگام استفاده از هیدیفای با پروتکل REALITY را پوشش می‌دهد.

---

## Common Phone Behaviour Issues / مشکلات رایج رفتار گوشی

### 1. Connection Drops / قطع شدن اتصال

**Symptoms / علائم:**
- VPN disconnects after a few hours of use
- پس از چند ساعت استفاده، VPN قطع می‌شود

**Possible Causes / دلایل احتمالی:**
- Battery optimisation killing the Hiddify app in the background
- بهینه‌سازی باتری که برنامه هیدیفای را در پس‌زمینه می‌بندد
- Mobile data switching to WiFi or vice versa
- تغییر از اینترنت موبایل به وای‌فای یا برعکس

**Solutions / راه‌حل‌ها:**
1. Disable battery optimisation for Hiddify in your phone settings
   غیرفعال کردن بهینه‌سازی باتری برای هیدیفای در تنظیمات گوشی
2. Enable "Always On VPN" in system settings (Android)
   فعال کردن «VPN همیشه روشن» در تنظیمات سیستم (اندروید)

---

### 2. Slow Speeds After a Few Hours / سرعت کم بعد از چند ساعت

**Symptoms / علائم:**
- Connection speed degrades noticeably after several hours
- سرعت اتصال بعد از چند ساعت به‌طور قابل توجهی کاهش می‌یابد

**Solutions / راه‌حل‌ها:**
1. Reconnect to refresh the REALITY session
   برای تازه‌سازی جلسه REALITY دوباره متصل شوید
2. Update the subscription profile (profile-update-interval is set to 24 hours in the snippet)
   پروفایل اشتراک را به‌روز کنید (فاصله به‌روزرسانی پروفایل در اسنیپت روی ۲۴ ساعت تنظیم شده است)

---

### 3. App Behaves Unexpectedly / رفتار غیرمنتظره برنامه

**Symptoms / علائم:**
- Hiddify shows connected but traffic is not routed through VPN
- هیدیفای متصل نشان می‌دهد اما ترافیک از طریق VPN هدایت نمی‌شود
- Certain apps bypass the VPN
- برخی برنامه‌ها از VPN عبور می‌کنند

**Solutions / راه‌حل‌ها:**
1. Check "Per-App Proxy" settings in Hiddify to ensure all required apps route through the VPN
   تنظیمات «پراکسی برای هر برنامه» در هیدیفای را بررسی کنید تا مطمئن شوید همه برنامه‌های مورد نیاز از طریق VPN هدایت می‌شوند
2. Restart Hiddify and reconnect
   هیدیفای را ری‌استارت کرده و مجدداً متصل شوید
3. Check if the profile is up to date via the refresh button
   با دکمه رفرش بررسی کنید که آیا پروفایل به‌روز است

---

### 4. Phone Battery Drain / مصرف باتری گوشی

**Symptoms / علائم:**
- Noticeably higher battery drain while Hiddify is running
- مصرف باتری به‌طور قابل توجهی هنگام اجرای هیدیفای بیشتر است

**Solutions / راه‌حل‌ها:**
1. Use the `warp` profile with fragment enabled (see `hiddify_snippet`) for lighter processing
   از پروفایل `warp` با فعال‌سازی فرگمنت استفاده کنید (به `hiddify_snippet` مراجعه کنید)
2. Reduce the update interval if frequent profile checks are draining the battery
   اگر بررسی‌های مکرر پروفایل باعث تخلیه باتری می‌شود، فاصله به‌روزرسانی را کاهش دهید

---

## Diagnostic Steps / مراحل عیب‌یابی

If you experience unexpected phone behaviour in the last few hours, follow these steps:

اگر رفتار غیرمنتظره‌ای در چند ساعت گذشته داشتید، این مراحل را دنبال کنید:

1. **Check Hiddify logs** – Open Hiddify → Settings → Logs to see recent connection events
   **بررسی لاگ‌های هیدیفای** – هیدیفای → تنظیمات → لاگ‌ها را باز کنید

2. **Verify the active profile** – Ensure your profile has not expired (check `subscription-userinfo`)
   **تأیید پروفایل فعال** – مطمئن شوید پروفایل شما منقضی نشده است

3. **Re-import the snippet** – Use the link below to get a fresh copy of the snippet:
   **وارد کردن مجدد اسنیپت** – از لینک زیر برای دریافت نسخه جدید استفاده کنید:
   ```
   https://raw.githubusercontent.com/hiddify/hiddify-app/refs/heads/main/test.configs/hiddify_snippet
   ```

4. **Check for app updates** – Make sure Hiddify is up to date from [app.hiddify.com](https://app.hiddify.com)
   **بررسی به‌روزرسانی برنامه** – مطمئن شوید هیدیفای از [app.hiddify.com](https://app.hiddify.com) به‌روز است

---

## Support / پشتیبانی

- Telegram: [t.me/hiddify](https://t.me/hiddify)
- Website: [hiddify.com](https://hiddify.com)
