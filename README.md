# Pokitro
صفحاتي الرسمية 
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pokitro - كيرلس عفت</title>
    <!-- Font Awesome للأيقونات -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- خط Tajawal العصرى من Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700;900&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --bg-color: #0b0f19;
            --card-bg: rgba(22, 31, 48, 0.7);
            --accent-color: #00f2fe;
            --accent-gradient: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
            --hover-gradient: linear-gradient(135deg, #00f2fe 0%, #4facfe 100%);
            --text-color: #ffffff;
            --subtext-color: #94a3b8;
            --border-color: rgba(255, 255, 255, 0.08);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Tajawal', sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            background-image: 
                radial-gradient(circle at 15% 15%, rgba(0, 242, 254, 0.12) 0%, transparent 40%),
                radial-gradient(circle at 85% 85%, rgba(79, 172, 254, 0.12) 0%, transparent 40%);
        }

        .container {
            width: 100%;
            max-width: 420px;
            text-align: center;
        }

        .profile-card {
            background: var(--card-bg);
            backdrop-filter: blur(12px);
            border: 1px solid var(--border-color);
            border-radius: 24px;
            padding: 40px 24px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4);
        }

        .avatar {
            width: 96px;
            height: 96px;
            border-radius: 50%;
            background: var(--accent-gradient);
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto 20px auto;
            font-size: 40px;
            color: #000;
            box-shadow: 0 0 25px rgba(0, 242, 254, 0.4);
        }

        h1 {
            font-size: 26px;
            font-weight: 900;
            margin-bottom: 6px;
            letter-spacing: 0.5px;
        }

        .bio {
            color: var(--subtext-color);
            font-size: 15px;
            margin-bottom: 32px;
            font-weight: 400;
        }

        .links-container {
            display: flex;
            flex-direction: column;
            gap: 16px;
        }

        .link-card {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 16px 20px;
            border-radius: 16px;
            background: rgba(255, 255, 255, 0.03);
            border: 1px solid var(--border-color);
            color: var(--text-color);
            text-decoration: none;
            font-size: 16px;
            font-weight: 700;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .link-card i.icon {
            font-size: 22px;
            width: 30px;
            text-align: center;
        }

        .link-card .arrow {
            font-size: 14px;
            color: var(--subtext-color);
            transition: transform 0.3s ease;
        }

        .link-card:hover {
            transform: translateY(-3px);
            border-color: rgba(0, 242, 254, 0.5);
            background: rgba(0, 242, 254, 0.08);
            box-shadow: 0 8px 20px rgba(0, 242, 254, 0.15);
        }

        .link-card:hover .arrow {
            transform: translateX(-4px);
            color: var(--accent-color);
        }

        .facebook:hover i.icon { color: #1877f2; }
        .whatsapp:hover i.icon { color: #25d366; }

        footer {
            margin-top: 32px;
            font-size: 13px;
            color: var(--subtext-color);
            opacity: 0.7;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="profile-card">
            <!-- الشعار أو الصورة الشخصية -->
            <div class="avatar">
                <i class="fa-solid fa-bolt"></i>
            </div>

            <!-- الاسم والـ Bio -->
            <h1>Pokitro</h1>
            <p class="bio">كيرلس عفت</p>

            <!-- الأزرار والروابط -->
            <div class="links-container">
                <a href="https://facebook.com" target="_blank" class="link-card facebook">
                    <i class="fa-brands fa-facebook-f icon"></i>
                    <span>فيسبوك</span>
                    <i class="fa-solid fa-chevron-left arrow"></i>
                </a>

                <a href="https://wa.me/" target="_blank" class="link-card whatsapp">
                    <i class="fa-brands fa-whatsapp icon"></i>
                    <span>واتساب</span>
                    <i class="fa-solid fa-chevron-left arrow"></i>
                </a>
            </div>

            <footer>
                &copy; Pokitro. جميع الحقوق محفوظة
            </footer>
        </div>
    </div>

</body>
</html>
