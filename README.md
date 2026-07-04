<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>د. مصطفى درويش - مستشار قانوني</title>
    <!-- استيراد خطوط متناسقة وعريضة لتناسب التصميم القانوني الفخم -->
    <link rel="preconnect" href="https://googleapis.com">
    <link rel="preconnect" href="https://gstatic.com" crossorigin>
    <link href="https://googleapis.com/css2?family=Cairo:wght@700;900&family=Montserrat:wght@700;900&display=swap" rel="stylesheet">
    <!-- أيقونات مبسطة للعنوان والواتساب -->
    <link rel="stylesheet" href="https://cloudflare.com">
    
    <style>
        /* إعدادات الخلفية السوداء العامة والتصفير */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            background-color: #000000;
            color: #ffffff;
            font-family: 'Cairo', sans-serif;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: flex-start;
            padding: 40px 20px;
            overflow-x: hidden;
        }

        /* حاوية المحتوى الرئيسي المتمركز في المنتصف */
        .container {
            max-width: 600px;
            width: 100%;
            text-align: center;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* العناوين الرئيسية بحجم عريض بولد */
        .title-ar {
            font-size: 24px;
            font-weight: 900;
            color: #D4AF37; /* ذهبي كلاسيكي فخم */
            margin-bottom: 5px;
            text-shadow: 0 2px 4px rgba(212, 175, 55, 0.2);
        }
        .title-en {
            font-family: 'Montserrat', sans-serif;
            font-size: 20px;
            font-weight: 900;
            /* تأثير الفضي البراق */
            color: #E5E4E2;
            background: linear-gradient(135deg, #f0f0f0 0%, #b0b0b0 50%, #f5f5f5 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 25px;
            text-shadow: 0 2px 4px rgba(255,255,255,0.1);
        }

        /* البرواز الذهبي ذو الإطار المزخرف النحيف المخصص للصور */
        .photo-frame {
            width: 260px;
            height: 340px;
            border: 3px double #D4AF37; /* إطار مزدوج مزخرف نحيف */
            padding: 6px;
            background-color: #000000;
            box-shadow: 0 0 15px rgba(212, 175, 55, 0.3);
            margin-bottom: 30px;
            position: relative;
            overflow: hidden;
            border-radius: 4px;
        }

        /* إعدادات متحكم الشرائح التلقائي للصور الثلاث */
        .slider {
            width: 100%;
            height: 100%;
            position: relative;
        }
        .slider img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            position: absolute;
            top: 0;
            left: 0;
            opacity: 0;
            transition: opacity 0.8s ease-in-out;
        }
        /* تفعيل ظهور الصورة الأولى بشكل مبدئي */
        .slider img.active {
            opacity: 1;
        }

        /* إعدادات المقاطع البراجرافات بحجم متناسق */
        .paragraph-section {
            width: 100%;
            margin-bottom: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .text-gold {
            font-size: 16px;
            font-weight: 700;
            color: #D4AF37;
            line-height: 1.6;
            margin-bottom: 8px;
        }
        .text-silver {
            font-size: 14px;
            font-weight: 700;
            color: #C0C0C0;
            line-height: 1.5;
            margin-bottom: 15px;
        }
        /* الخطوط الفاصلة الذهبية الناعمة في نهاية كل برأجراف */
        .gold-divider {
            width: 60%;
            height: 1px;
            background: linear-gradient(90deg, transparent, #D4AF37, transparent);
            margin-top: 5px;
        }

        /* إعدادات التفاعل والروابط للخرائط والواتساب */
        .info-link {
            text-decoration: none;
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 100%;
        }
        .info-link:hover .text-gold {
            color: #fff;
            text-shadow: 0 0 5px #D4AF37;
        }
        .map-icon {
            font-size: 18px;
            color: #D4AF37;
            margin-bottom: 5px;
        }
        .whatsapp-container {
            margin-top: 15px;
            width: 100%;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .whatsapp-btn {
            background-color: #128C7E;
            color: #ffffff;
            padding: 10px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 700;
            font-size: 14px;
            margin-top: 15px;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            box-shadow: 0 4px 10px rgba(18, 140, 126, 0.4);
            transition: transform 0.2s;
        }
        .whatsapp-btn:hover {
            transform: scale(1.05);
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- العنوان الرئيسي -->
        <h1 class="title-ar">د.مصطفي درويش</h1>
        <h2 class="title-en">Dr. Moustafa Darwish</h2>

        <!-- برواز الصور المزخرف الذهبي والشرائح -->
        <div class="photo-frame">
            <div class="slider">
                <img src="https://githubusercontent.com" class="active" alt="د. مصطفى درويش 1" id="img1">
                <img src="" alt="د. مصطفى درويش 2" id="img2">
                <img src="" alt="د. مصطفى درويش 3" id="img3">
            </div>
        </div>

        <!-- المقطع الأول: التخصص الاستشاري والقانوني -->
        <div class="paragraph-section">
            <p class="text-gold">مستشار قانوني متخصص في قضايا البنوك  و التسويات البنكيه و إعادة جدولة المديونيات المتعثرة 
            داخل مصر و دول الخليج العربي </p>
            <p class="text-silver" dir="ltr">Legal Consultant specializing in banking finance, debt settlements, and non-performing loans (NPLs) restructuring</p>
            <div class="gold-divider"></div>
        </div>

        <!-- المقطع الثاني: المؤهل العلمي والشهادات -->
        <div class="paragraph-section">
            <p class="text-gold">دكتوراه في التنميه البشريه و تطوير الاعمال</p>
            <p class="text-silver" dir="ltr">PhD in Human Development and Business Development</p>
            <div class="gold-divider"></div>
        </div>

        <!-- المقطع الثالث: المحاضر المعتمد في المملكة المتحدة -->
        <div class="paragraph-section">
            <p class="text-gold">محاضر معتمد من أكاديميه التدريب الدولية بالمملكة المتحده</p>
            <p class="text-silver" dir="ltr">Certified instructor from the International Training Academy - UK</p>
            <div class="gold-divider"></div>
        </div>

        <!-- المقطع الرابع والأخير: الخرائط والعنوان والتواصل وحجز المواعيد -->
        <div class="paragraph-section">
            <!-- رابط تفاعلي يفتح الخريطة للإسكندرية مباشرة عند الضغط عليه -->
            <a href="https://google.com" target="_blank" class="info-link">
                <i class="fa-solid fa-location-dot map-icon"></i>
                <p class="text-gold">٥٢ شارع توت عنخ أمون ابراج سيدي جابر ، الإسكندرية</p>
                <p class="text-silver" dir="ltr">52 Tutankhamun Street, Sidi Gaber Towers, Alexandria</p>
            </a>
            <div class="gold-divider"></div>
            
            <!-- تم تصحيح الفقرة المكاملة هنا لتظهر اللغة العربية كاملة وتحتها الترجمة الإنجليزية -->
            <div class="whatsapp-container">
                <p class="text-gold">حجز المواعيد برساله على الواتس ٠٠٢٠١٠٠٨٠٧٠٠٨٧</p>
                <p class="text-silver" dir="ltr">Book appointments by sending a message to WhatsApp number +201008070087</p>
            </div>
            
            <!-- زر تفاعلي للاتصال السريع والمباشر بالواتساب فوراً برقمك المكتوب -->
            <a href="https://wa.me،%20أود%20حجز%20موعد%20إستشارة" target="_blank" class="whatsapp-btn">
                <i class="fa-brands fa-whatsapp" style="font-size: 18px;"></i>
                <span>٠٠٢٠١٠٠٨٠٧٠٠٨٧ | Book Now</span>
            </a>
        </div>
    </div>

    <!-- كود التحويل التلقائي للشرائح كل 4 ثوانٍ وسحب روابط صورك المرفوعة -->
    <script>
        const username = "dr-moustafa71";
        const repo = "Profile";
        
        document.getElementById('img1').src = `https://githubusercontent.com{username}/${repo}/main/dr-moustafa-darwish-v2.html`; 
        document.getElementById('img2').src = `https://githubusercontent.com{username}/${repo}/main/dr-moustafa-darwish-v2.html`; 
        document.getElementById('img3').src = `https://githubusercontent.com{username}/${repo}/main/dr-moustafa-darwish-v2.html`;

        const images = document.querySelectorAll('.slider img');
        let currentIndex = 0;

        setInterval(() => {
            images[currentIndex].classList.remove('active');
            currentIndex = (currentIndex + 1) % images.length;
            images[currentIndex].classList.add('active');
        }, 4000);
    </script>
</body>
</html>
# 👋 أهلاً بك في بروفايل د. مصطفى للاستشارات القانونية | Dr. Moustafa Legal Firm

<p align="center">
  <img src="https://shields.io" alt="Status">
  <img src="https://shields.io" alt="Focus">
</p>

## ⚖️ نبذة عنّا
مرحباً بك في صفحة البروفاايل الخاص بنا نحن نقدم خدمات تدريبيه واستشارات قانونية متكاملة تهدف إلى حماية أعمالكم وتوفير الحلول القانونية المبتكرة والذكية لتلبية احتياجات الشركات والأفراد.

## 🛠️ مجالات التخصص والخدمات
* 🏛️ **الاستشارات القانونية:** تقديم الدعم القانوني للشركات والأفراد.
* 📝 **صياغة العقود:** إعداد ومراجعة الاتفاقيات والعقود التجارية والمدنية.
* 💼 **تدريب وتطوير الكوادر:** يبدأ الأمان الحقيقى من اللحظه الفعليه من إدراك القائم بالاعمال بطبيعة أدواته و قوتها و طريقة الأستفاده القصوى من الأمكانيات و الصلاحيات التى تمنحها له هذه الأدوات.
* 🌐 **التكنولوجيا والقانون:** صياغة سياسات الخصوصية وشروط الاستخدام للمواقع والتطبيقات.

## 🤝 تواصل معنا
يسعدنا دائماً استقبال استفساراتكم وبناء شراكات عمل مثمرة:
* 📧 **البريد الإلكتروني:** [اmoustafa.mzd@gmail.com]
* 🌐 **الموقع الإلكتروني:** [رابط موقعك إن وجد]
