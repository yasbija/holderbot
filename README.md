![Example Image](holderbotcover.png)


# هولدربات بتا چیه؟ (ورژن 4.0.2)
هولدر بات یه ربات سریع و ساده‌ست که برای حل مشکل عدم وجود گزینه `شروع تایمر پس از اولین اتصال` در رابط کاربری "پنل مرزبان" ساخته شده. با استفاده از رابط‌های برنامه نویسی `پنل مرزبان`، هولدر بات بهت این امکان رو می‌ده که به راحتی از این قابلیت در تلگرام استفاده کنید. ولی بعد از آپدیت 3.0 هولدربات قضیه یکمی متفاوت تر شد و هولدربات امکانات خاصی برای کاربران عرضه کرد که این قابلیت ها در نسخه های بعد از 4 به اوج رسید. هم اکنون هولدربات یک دستیار حرفه ای برای مرزبانی ها می باشد. برای اطلاعات بیشتر به قسمت بروزرسانی ها مراجعه کنید و یا در کانال [@ErfjabHolderbot](https://t.me/ErfjabHolderbot) عضو شوید ، نصب کنید و لذت ببرید.

# چجوری نصب/آپدیت کنیم؟
برای آپدیت ابتدا توکن بات را revoke کنید. سپس برای نصب فقط کافیه دستورات زیر را در سرور ابونتوی خود وارد کنید.
```
cd && cd .. && rm installbeta.sh*
```

```
sudo apt install && sudo apt-get install libjpeg-dev && wget https://raw.githubusercontent.com/erfjab/holderbot/main/installbeta.sh && chmod +x installbeta.sh && ./installbeta.sh
```
حالا که همه پیش‌نیازها نصب شدن، برای استارت زدن ربات اطلاعات زیر رو بهش بدید.



| اطلاعات | توضیحات |
| --- | --- |
| شناسه کاربری ادمین | شناسه کاربری تلگرامی شخصی که می‌خواهد از ربات استفاده کند. می‌توانید این اطلاعات را از این ربات بدست آورید. [@userinfobot](https://t.me/userinfobot) |
| اسم | یک اسم الکی وارد کنید. |
| توکن ربات تلگرام | توکن بات تلگرامی خود را میتوانید از طریق [@BotFather](https://t.me/botfather) بدست آورید. |
| نام کاربری پنل | می‌توانید نام کاربری مدیر اصلی را وارد کنید. |
| رمز عبور پنل | می‌توانید رمز عبور مدیر اصلی را وارد کنید. |
| دامنه پنل | ساب دامنه پنل خود را وارد کنید، بدون 'https://' ولی با پورت ، مانند: sub.domain.com:port |

اگر اطلاعاتتون رو به درستی وارد کرده باشید، یک پیامی به این شکل دریافت خواهید کرد.

![Example Image](nohupshot.png)

**صفحه را همانطور که هست نگه دارید و اکنون ربات را تست کنید. اگر اطلاعات شما صحیح باشد، ربات برای شما کاربر ایجاد می کند و اگر صحیح نباشد، کاربر ایجاد نمی کند.**
اگر ربات برای شما کاربر ایجاد نکرد، به صفحه بازگردید و دستور زیر را اجرا کنید.
```
Ctrl C
```
سپس دوباره از ابتدا مراحل نصب را طی کنید، فقط در تکمیل اطلاعات خود دقت کنید.

**اکنون، اگر این بار کاربر ربات ساخته است، پس لذت ببرید.** (سرور رو بدون دستوری ببندید.)

# بروزرسانی و امکانات جدید ؟

<details  markdown="1"> <summary>نسخه‌ی 1.0</summary>

  - تولد هولدربات و امکان دریافت ساخت یوزر با قابلیت شروع تایم بعد اولین اتصال. 

</details>

<details  markdown="1"> <summary>نسخه‌ی 2.0</summary>

  - امکان ساخت دسته جمعی یوزر. 

</details>

<details  markdown="1"> <summary>نسخه‌ی 3.0</summary>

  - امکان مانیتورینگ لحظه ای نود ها
  - ارسال نوتیف هنگام قطع شدن نودها
  - امکان انتخاب اینباند‌ هنگام ساخت یوزر
  - امکان دریافت آمار کلی کاربران پنل تعداد و لیست‌شون 
  - (مخصوصا کاربران آنلاین و آفلاین در 24 ساعت اخیر)
  - امکان دریافت آمار تکی کاربر با اسم یا لینک ساب 
  - (مخصوصا آخرین تایم آپدیت ساب و آنلاینی)
  - امکان دریافت آمار با لینک ساب توسط کاربر از بات
  - رفع باگ اذیت کننده‌ی credentials
</details>

<details  markdown="1"> <summary>نسخه‌ی 4.0</summary>
    
- امکان مدیریت ادمین‌های پنل (تغییر رمز و یا sudo)
- امکان حذف و اضافه ادمین برای پنل
- امکان تعیین ضریب مصرف نود
- امکان مدیریت‌ نودها (غیرفعال‌سازی/فعال‌سازی/ری‌کانکت)
- امکان مانیتورینگ و اطلاع‌رسانی قطعی نودها
- امکان غیرفعالسازی/فعالسازی مانیتورینگ
- امکان تغییر تایمر مانیتورینگ نودها
- امکان ساخت کاربر به صورت گروهی/تکی (on_hold)
- امکان ساخت کاربر از طریق تمپلیت‌ها
- امکان ساخت تمپلیت‌ها (حجم، زمان، اینباندها)
- امکان دریافت لیست کاربران آنلاین/آفلاین (از 1 دقیقه تا 60 روز اخیر به صورت جدول و PDF)
- امکان دریافت لیست کاربران آپدیت‌شده/نشده ساب (از 1 دقیقه تا 60 روز اخیر به صورت جدول و PDF)
- امکان دریافت آخرین‌تایم آنلاینی، آپدیت‌ساب کاربر (تکی)
- امکان دریافت مستقیم بارکد و متن لینک‌ساب یا حذف کاربر
- امکان دریافت نرم‌افزار مورد استفاده‌ی کاربر
- امکان دریافت بارکد لینک ارسالی دلخواه
- امکان سرچ و دریافت کاربرهای مشابه (مثل Did you Mean گوگل)
- رابط کاربری ساده و شیک جدید

</details>


# چجوری استفاده کنیم؟ 

چنل [@ErfjabHolderbot](https://t.me/ErfjabHolderbot) جهت ارائه آموزش ها ، اطلاع رسانی های آپدیت ها ، نظرسنجی ها برای اضافه شدن ویژگی های جدید و از این قبیل تشکیل شده است.

<p align="center">
  <a target="_blank" href="https://t.me/ErfjabHolderbot">
    <img alt="Telegram Badge" src="https://img.shields.io/badge/holderbotchanel-Telegramlink?style=for-the-badge&logo=telegram&logoColor=white&color=blue&link=https%3A%2F%2Ft.me%2FErfjabHolderbot&link=https%3A%2F%2Ft.me%2FErfjabHolderbot">
  </a>
</p>

