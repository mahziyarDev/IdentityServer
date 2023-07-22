# IdentityServer

<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
</head>
<body>
    <div>
        <strong>این پروژه صرفا جهت تمرین بوده و مواردی که بیشترین نقش را در مبحث Identity server دارد را شامل می شود. </strong>
    </div>
    <div>
        <h2>
            برای اجرای این پروژه دوتا update-database میزنید:
        </h2>
        <ul>
            <ol>1.Update-Database init -Context PersistedGrantDbContext</ol>
            <ol>2.Update-Database init -Context ConfigurationDbContext</ol>
        </ul>
</div>
<div>
    <h2>
        در صورت نیاز دستورات migration :
    </h2>
    <ul>
        <ol>1.Add-Migration init -Context PersistedGrantDbContext -o Data/Config</ol>
        <ol>2.Add-Migration init -Context ConfigurationDbContext -o Data/Config2</ol>
    </ul>
</div>

<div>
    <h2>
        نحوه run  کردن پروژه :
    </h2>
    <p>
        پروزه Api رو به صورت run without debuging و سپس پروژه identity server  و در آخر هم پروژه ui  . بعد از run شدن پروژه ui برای احراز هویت به یک url  هدایت شده سپس شما با نام کاربر و رمز عبور یکسان alice لاگین می نمایید.
سپس در آدرس https://localhost:7002/weatherforcast می توانید دیتا هایی را مشاهده کنید.
    </p>
</div>
</body>
</html>
