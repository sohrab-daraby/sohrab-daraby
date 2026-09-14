# 🚀 راهنمای راه‌اندازی و انتشار پروفایل روی گیت‌هاب (Setup Guide)

این پکیج یک سیستم کامل و فوق‌پیشرفته برای ساخت پروفایل متحرک (Animated Profile README) به سبک **Cyberpunk Hologram & Cloud Architecture** است.

---

## ۱. ساخت مخزن اختصاصی پروفایل در گیت‌هاب (Special Profile Repo)

1. وارد اکانت گیت‌هاب خود شوید.
2. یک مخزن (Repository) جدید با **دقیقاً همان نام کاربری (Username) گیت‌هاب خود** بسازید:
   - برای مثال اگر یوزرنیم شما `sohrabdarabi` است، نام مخزن باید دقیقاً `sohrabdarabi` باشد.
3. تیک **Public** را حتماً بزنید (پروفایل‌های خصوصی نمایش داده نمی‌شوند).
4. تیک **Add a README file** را هم فعال کنید و سپس دکمه **Create repository** را بزنید.

---

## ۲. انتقال فایل‌ها به مخزن گیت‌هاب

فایل‌های تولیدشده در این فولدر را داخل مخزن جدید خود آپلود کنید یا با دستورات زیر پوش کنید:

```bash
# در پوشه جاری همین پروژه:
git init
git add .
git commit -m "feat: setup next-gen cyberpunk animated profile"
git branch -M main
git remote add origin https://github.com/<YOUR_USERNAME>/<YOUR_USERNAME>.git
git push -u origin main --force
```

> [!NOTE]
> حتماً پوشه پنهان `.github/workflows/snake.yml` و پوشه `assets/` همراه فایل `README.md` منتقل شوند.

---

## ۳. شخصی‌سازی اطلاعات و لینک‌ها (Personalization)

در فایل `README.md`:
1. اگر یوزرنیم گیت‌هاب شما چیزی به جز `sohrabdarabi` است، در فایل `README.md` با فشردن `Ctrl+H`، عبارت `sohrabdarabi` را با یوزرنیم واقعی خود جایگزین کنید تا ویجت‌های لایو گیت‌هاب آمار دقیق اکانت شما را نشان دهند.
2. لینک‌های شبکه‌های اجتماعی (لینکدین، تلگرام، ایمیل) را در بخش `CYBER HUD BADGES` مطابق با آدرس‌های خودتان به‌روز کنید.

---

## ۴. فعال‌سازی اکشن خودکار بازی مار (Snake Animation Workflow)

برای اینکه انیمیشن متحرک مار گیت‌هاب فعال شود و هر ۱۲ ساعت مشارکت‌های شما را بخورد:

1. در صفحه مخزن خود در گیت‌هاب، به تب **Settings** بروید.
2. از منوی سمت چپ، روی **Actions** و سپس **General** کلیک کنید.
3. در انتهای صفحه، بخش **Workflow permissions** را روی گزینه:
   - **Read and write permissions** قرار دهید و دکمه **Save** را بزنید.
4. سپس به تب **Actions** بالای مخزن رفته، ورک‌فلو **Generate Snake Contribution Animation** را انتخاب کرده و دکمه **Run workflow** را بزنید تا شاخه `output` و تصویر انیمیشنی ساخته شود.

---

## ساختار فایل‌های این پکیج:
- 📁 `assets/hero-banner.svg`: بنر سینمایی عریض با گرید سه‌بعدی، امواج صوتی زنده و پالس‌های مدار
- 📁 `assets/terminal-bio.svg`: کنسول ترمینال لینوکس با انیمیشن تایپ زنده و آرت رک‌های سرور
- 📁 `assets/cloud-telemetry.svg`: رادار متحرک ۳۶۰ درجه میکروسرویس‌ها و تلمتری ابری
- 📁 `assets/skills-matrix.svg`: دک تراشه‌ای مهارت‌ها و معماری سیستم بک‌اند و دوآپس
- 📁 `.github/workflows/snake.yml`: اکشن خودکار گیت‌هاب برای جنریت انیمیشن مار مشارکت‌ها
- 📄 `README.md`: فایل آماده و نهایی برای نمایش روی صفحه اول پروفایل شما
