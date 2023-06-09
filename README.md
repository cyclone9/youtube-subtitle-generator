## ساخت زیرنویس برای ویدیوهای یوتیوب با دادن لینک

با توجه به اهمیت استفاده از محتوای یوتیوب برای یادگیری مطالب گوناگون و موجود نبودن زیرنویس فارسی برای بعضی از ویدیو ها یا کیفیت پایین این زیر نویس ها تصمیم به ساخت سرور شخصی برای ساخت زیرنویس با استفاده از کتابخانه ها و api های موجود گرفتم.
با توجه به تجریه ترجمه کتاب با استفاده از کد نویسی و ضعیف بودن تکنولوژی ها برای ترجمه با کیفیت، در مدت دو هفته گذشته راه های بسیاری را امتحان کردم و به این نتیجه رسیدم بهترین ترجمه ای که میتوان از هوش مصنوعی گرفت استفاده همزمان از سرور google translate و chatgpt با یکدیگر است.
روند کار به این صورت است که وقتی متن وارد سرور می شود یک بار به وسیله google translate ترجمه می شود و وقتی جواب آماده شد، متن فارسی یک بار دیگر به وسیله chatgpt به کمک پرامت بازنویسی انجام میشود.

### نحوه عملکرد

در این ریپو به دلیل متن باز بودن و راحتی استفاده برنامه نویسان از زیرنویس یوتیوب از api شرکت گوگل استفاده کرده ام اما شما می توانید برای بالا بردن کیفیت ترجمه اقدام به خرید سرویس های معتبر و جاگذاری api key با گوگل کنید.

<p align="center">
    <img src="./demo.gif" width="600"/>
</p>

### How to install ?

- Clone This repo
- Cd youtube-subtitle-generator
- Change env.local to env
- To install all modules `yarn`
- To run developer server `yarn dev`
- You can install pm2 globally before deploying. `npm i pm2 -g`
- Then run `pm2 start /src/index.js`
