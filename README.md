<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>سعرها - بالسعر الأصلي</title>

    <!-- إعدادات التغليف (PWA) والهوية -->
    <link rel="manifest" href="manifest.json">
    <meta name="theme-color" content="#f97316">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <meta name="apple-mobile-web-app-title" content="سعرها">
    
    <style>
        body {
            font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background-color: #fdfdfd;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            text-align: center;
        }
        .logo-container img {
            width: 140px;
            height: 140px;
            object-fit: contain;
            border-radius: 28px;
            box-shadow: 0 10px 25px rgba(249, 115, 22, 0.2);
        }
        h1 {
            color: #f97316;
            font-size: 28px;
            margin: 10px 0 5px;
        }
        p.slogan {
            color: #666;
            font-size: 16px;
            font-weight: bold;
            margin-bottom: 30px;
        }
        .content-box {
            background: #ffffff;
            padding: 24px;
            border-radius: 16px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.05);
            max-width: 90%;
            width: 400px;
        }
    </style>
</head>
<body>

    <div class="logo-container">
        <img src="https://cdn-icons-png.flaticon.com/512/1069/1069102.png" alt="شعار سعرها">
    </div>

    <h1>سعرها</h1>
    <p class="slogan">بالسعر الأصلي</p>

    <div class="content-box">
        <p>مرحباً بكِ في تطبيق <strong>سعرها</strong> لمقارنة الأسعار والعروض بكل سهولة!</p>
        <p style="font-size: 14px; color: #888;">الموقع جاهز الآن ليعمل كتطبيق مستقل على جوالكِ.</p>
    </div>

    <!-- كود إشعار وتنبيه التثبيت للشاشة الرئيسية في الجوال -->
    <script>
      window.addEventListener('DOMContentLoaded', () => {
        const isStandalone = window.navigator.standalone || window.matchMedia('(display-mode: standalone)').matches;

        if (!isStandalone) {
          const banner = document.createElement('div');
          banner.style.cssText = 'position:fixed; bottom:15px; left:15px; right:15px; background:#111; color:#fff; padding:12px 16px; border-radius:12px; text-align:center; z-index:99999; font-size:13px; box-shadow:0 4px 15px rgba(0,0,0,0.4); font-family:sans-serif; line-height:1.5;';
          banner.innerHTML = '📲 لتثبيت تطبيق <b>سعرها</b> على شاشتك الرئيسية:<br>اضغط زر <b>مشاركة (Share)</b> ثم <b>إضافة إلى الشاشة الرئيسية (Add to Home Screen)</b> <span style="display:block; margin-top:6px; font-size:11px; color:#aaa; cursor:pointer;" onclick="this.parentNode.style.display=\'none\'">إخفاء</span>';
          document.body.appendChild(banner);
        }
      });
    </script>
</body>
</html>
