# راه‌اندازی نود Network 3

## مراحل:

### ۱. ساخت حساب Network 3
- ابتدا در سایت زیر ثبت نام کنید و یک حساب ایجاد کنید. :  
  [لینک ثبت‌نام](https://account.network3.ai/register_page?rc=1198f6af)

---

### ۲. به‌روزرسانی سیستم‌عامل سرور VPS
برای به‌روزرسانی سیستم‌عامل از دستورات زیر استفاده کنید:
```bash
sudo apt update && sudo apt upgrade -y
```

---

### ۳. نصب نرم‌افزارهای ضروری
برای نصب نرم‌افزارهای مورد نیاز از این دستور استفاده کنید:
```bash
sudo apt install -y screen net-tools
```

---

### ۴. دانلود نود Network 3
- لینک دانلود را برای لینوکس از [داشبورد Network 3](https://network3.ai/download) کپی و پس از wget اضافه کنید.
- مثال:
```bash
wget https://network3.io/ubuntu-node-v2.1.0.tar
```

---

### ۵. استخراج فایل نرم‌افزار
برای استخراج فایل دانلود شده از دستور زیر استفاده کنید:
```bash
tar -xvf ubuntu-node-v2.1.0.tar
```

---

### ۶. ایجاد یک Screen
برای اجرای نود در پس‌زمینه، یک Screen جدید بسازید:
```bash
screen -S network3
```

---

### ۷. ورود به دایرکتوری نرم‌افزار
برای ورود به دایرکتوری استخراج شده نرم‌افزار، از دستور زیر استفاده کنید:
```bash
cd ubuntu-node
```

---

### ۸. راه‌اندازی نرم‌افزار نود
برای راه‌اندازی نود Network 3 از دستور زیر استفاده کنید:
```bash
sudo bash manager.sh up
```

---

### ۹. دریافت کلید مخفی نود
برای دریافت کلید مخفی نود خود، از دستور زیر استفاده کنید:
```bash
sudo bash manager.sh key
```
- کلید مخفی را در جایی امن ذخیره کنید.

---

### ۱۰. اتصال نود به حساب Network 3
1. وارد داشبورد حساب خود شوید.
2. آدرس زیر را در مرورگر خود وارد کنید (IP سرور خود را جایگزین xx.xx.xx.xx کنید):
   ```bash
   https://account.network3.ai/main?o=xx.xx.xx.xx:8080
   ```
3. بر روی دکمه «+» کلیک کنید و کلید مخفی را وارد کنید.

![image](https://github.com/user-attachments/assets/7e247680-d7bf-49a8-87bd-87f61f09fc45)

---

### ۱۱. مدیریت جلسه Screen
برای مدیریت جلسات Screen:
- برای خروج از screen:
  - `Ctrl + A` سپس `D`.
- برای بازگشت به screen:
```bash
screen -r network3
```

---

## تبریک!
راه‌اندازی نود Network3 شما با موفقیت انجام شد. به زودی پاداش‌ها را در داشبورد مشاهده خواهید کرد.
