# IdentityServer
این پروژه صرفا جهت تمرین بوده و مواردی که بیشترین نقش را در مبحث Identity server دارد را شامل می شود.

برای اجرای این پروژه دوتا update-database میزنید:
1.Update-Database init -Context PersistedGrantDbContext
2.Update-Database init -Context ConfigurationDbContext
در صورت نیاز دستورات migration :

1.Add-Migration init -Context PersistedGrantDbContext -o Data/Config
2.Add-Migration init -Context ConfigurationDbContext -o Data/Config2

نحوه run  کردن پروژه :
پروزه Api رو به صورت run without debuging و سپس پروژه identity server  و در آخر هم پروژه ui  . بعد از run شدن پروژه ui برای احراز هویت به یک url  هدایت شده سپس شما با نام کاربر و رمز عبور یکسان alice لاگین می نمایید.
سپس در آدرس https://localhost:7002/weatherforcast می توانید دیتا هایی را مشاهده کنید.
