# جنگو چیست؟

جنگو (جَنگو) یک فریم ورک تحت وب رایگان و open source است که با زبان پایتون نوشته شده است. یک فریم ورک تحت وب, دارای مجموعه ای است که به شما کمک می کنند تا یک وب سایت را سریع تر و راحت تر توسعه دهید.

هنگامی که در حال ساخت یک وب سایت هستید، شما همیشه به مجموعه ای از اجزای مشابه نیاز دارید. به شرح زیر: یک روش برای کنترل کردن احراز هویت کاربر (ثبت نام ، ورود به حساب کاربری ، خروج از حساب کاربری) ، یک پنل مدیریت برای وب سایت خود ، فرم ها ، روشی برای آپلود فایل ها و غیره.

خوشبختانه خیلی وقت پیش، افرادی متوجه این موضوع شدند که هنگام ساختن یک سایت جدید، توسعه دهندگان وب با مشکلات مشابهی روبرو می شوند، بنابراین آن ها تیمی را تشکیل دادند که به راحتی اجزای کار را در اختیار شما قرار می دهد که شما بتوانید به راحتی از انها استفاده کنید ودر نهایت فریم ورک ها را ساختند (جنگو یکی از آن هاست).

فریم ورکها به این دلیل به وجود آمده اند که دیگر نیازی نباشد شما از اول چرخ را بسازید و به شما کمک می کند تا به راحتی سایت خود را بسازید.

## چرا شما به یک فریم ورک نیاز دارید؟

برای درک بهترچگونگی عملکرد جنگو نگاه دقیق تری به سرور می اندازیم. اولین چیزی که سرور نیاز دارد که بداند این است که شما می خواهید سرور برای شما یک وب پیج را راه اندازی کند.

حالا میل باکس را تصور کنید که برای دریافت نامه ها ( requests) چه کارهایی را انجام می دهد. این کار توسط وب سرور انجام خواهد گرفت. وب سرور نامه را خوانده و پاسخ مربوطه را به وب پیج می فرستد. اما هنگامی که شما میخواهید چیزی را ارسال کنید, شما به برخی مطالب نیاز دارید. و جنگو همونی است که به شما برای ایجاد محتوا کمک می کند.

## زمانی که فردی یک درخواست از وب سایت به سرور شما می کند، چه اتفاقی می افتد؟

هنگامی که درخواست به وب سرور فرستاده می شود آن درخواست به جنگو انتقال داده می شود در این هنگام جنگو در تلاش برای فهمیدن درخواست می باشد. در ابتدا آدرس وب پیج را میگیرد و سعی در فهمیدن عملکرد می کند. این بخش توسط **urlresolver** جنگو انجام میگیرد (توجه داشته باشید که website address یوآرال را صدا میزند – Uniform Resource Locator– به این دلیل *urlresolver* نامیده می شود). یک لیست از الگوها را میگیرد و سعی برای مطابقت با آدرس می کند (خیلی منطقی نیست). جانگو الگوها را از بالا به پایین بررسی می کند و اگر چیزی هماهنگ باشد، جانگو درخواست را به تابع مرتبط (که * نمایش </ 0> نامیده می شود) می گذارد.</p> 

تصور کنید یک حامل نامه با یک نامه. او در خیابان راه می رود و هر شماره خانه را در مقابل نامه ای قرار می دهد. اگر مطابقت داشته باشد، نامه را در آنجا می گذارد. این است که چگونه حل کننده آدرس اینترنتی کار می کند!

در عملکرد * مشاهده </ 0>، تمام چیزهای جالب انجام می شود: ما می توانیم به یک پایگاه داده نگاه کنیم تا اطلاعاتی را جستجو کنیم. شاید کاربر درخواست تغییر در داده را داشته باشد؟ مثل یک نامه گفت: "لطفا توضیح کار من را تغییر دهید." * مشاهده </ 0> می توانید بررسی کنید که آیا شما مجاز به انجام این کار هستید، و سپس شرح شغل را برای شما به روز رسانی کرده و یک پیام را ارسال کنید: "انجام شد!" سپس نمایش * یک پاسخ ایجاد می کند و جنگجو می تواند آن را به مرورگر وب کاربر ارسال کند.</p> 

البته توضیح بالا کمی ساده شده است، اما نیازی به دانستن همه چیزهای فنی نیست. ایده کلی این است که کافی باشد.

بنابراین به جای غواصی بیش از حد به جزئیات، ما به سادگی شروع به ایجاد چیزی با جانگو و ما تمام بخش های مهم را در طول راه یاد بگیریم!