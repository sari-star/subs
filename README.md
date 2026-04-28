<DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اشتراكات شات الأقصى</title>
    <link href="https://fonts.googleapis.com/css2?family=Changa:wght@400;700&family=Tajawal:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-gold: #d4af37;
            --secondary-blue: #1a5f7a;
            --dark-bg: #0a0a0a;
            --card-bg: #161616;
            --text-color: #e0e0e0;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: var(--dark-bg);
            color: var(--text-color);
            font-family: 'Changa', sans-serif;
            line-height: 1.6;
        }

        /* ✨ البنر العلوي */
        .hero-section {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(10,10,10,1)), 
                        url('https://images.unsplash.com/photo-1590076215667-873d3950ef31?q=80&w=2070&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
            height: 350px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            border-bottom: 3px solid var(--primary-gold);
        }

        h1 {
            font-size: clamp(2.2rem, 6vw, 4rem);
            color: var(--primary-gold);
            margin: 0;
            text-shadow: 0 4px 15px rgba(212, 175, 55, 0.3);
            font-weight: 700;
        }

        .subtitle {
            font-family: 'Tajawal', sans-serif;
            font-size: 1.2rem;
            color: #bbb;
            margin-top: 10px;
        }

        /* 📊 الحاوية والجدول */
        .container {
            max-width: 1000px;
            margin: -50px auto 50px auto;
            padding: 0 20px;
        }

        .table-wrapper {
            background: var(--card-bg);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0,0,0,0.6);
            border: 1px solid #333;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            text-align: center;
        }

        th {
            padding: 22px;
            background-color: #1a1a1a;
            font-size: 1.2rem;
            color: var(--primary-gold);
            border-bottom: 2px solid #333;
        }

        td {
            padding: 16px;
            border-bottom: 1px solid #252525;
            font-size: 1.1rem;
            transition: 0.3s;
        }

        tr:hover td {
            background-color: #1d1d1d;
        }

        .check { color: #2ecc71; font-weight: bold; font-size: 1.3rem; }
        .cross { color: #e74c3c; font-weight: bold; font-size: 1.3rem; }

        .price-row {
            background-color: rgba(212, 175, 55, 0.08);
            font-weight: bold;
            color: var(--primary-gold);
            font-size: 1.3rem;
        }

        /* 📱 قسم التواصل والزر المحدث */
        .contact-card {
            margin-top: 40px;
            background: linear-gradient(145deg, #161616, #1f1f1f);
            padding: 40px 20px;
            border-radius: 20px;
            border: 1px solid #2a2a2a;
            box-shadow: 0 10px 25px rgba(0,0,0,0.3);
            text-align: center;
        }

        .contact-card h3 {
            margin-top: 0;
            color: var(--primary-gold);
            font-size: 1.8rem;
        }

        .btn-contact {
            display: inline-block;
            margin-top: 20px;
            padding: 15px 45px;
            background: linear-gradient(45deg, var(--primary-gold), #b8860b);
            color: #000;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            font-size: 1.2rem;
            box-shadow: 0 4px 15px rgba(212, 175, 55, 0.4);
            transition: all 0.4s ease;
        }

        .btn-contact:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(212, 175, 55, 0.6);
            filter: brightness(1.1);
        }

        .note {
            font-size: 0.9rem;
            color: #777;
            margin-top: 25px;
            font-family: 'Tajawal', sans-serif;
        }

        /* الهواتف الذكية */
        @media (max-width: 600px) {
            th, td { padding: 12px 5px; font-size: 0.9rem; }
            .hero-section { height: 280px; }
            .btn-contact { width: 80%; padding: 12px 20px; }
        }
    </style>
</head>
<body>

    <section class="hero-section">
        <h1>شات الأقصى</h1>
        <div class="subtitle">فخامة الحوار.. وجمال اللقاء</div>
    </section>

    <div class="container">
        <div class="table-wrapper">
            <table>
                <thead>
                    <tr>
                        <th>الميزة</th>
                        <th>ذهبي</th>
                        <th>فضي</th>
                        <th>برونزي</th>
                    </tr>
                </thead>
                <tbody>
                    <tr><td>الطرد والحظر</td><td class="check">✔</td><td class="check">✔</td><td class="check">✔</td></tr>
                    <tr><td>حذف الصور المخالفة</td><td class="check">✔</td><td class="check">✔</td><td class="check">✔</td></tr>
                    <tr><td>إرسال الهدايا</td><td class="check">✔</td><td class="check">✔</td><td class="check">✔</td></tr>
                    <tr><td>تغيير زخرفة النك</td><td class="check">✔</td><td class="check">✔</td><td class="check">✔</td></tr>
                    <tr><td>فتح المحادثات الخاصة</td><td class="check">✔</td><td class="check">✔</td><td class="check">✔</td></tr>
                    <tr><td>كشف النكات المخفية</td><td class="check">✔</td><td class="check">✔</td><td class="check">✔</td></tr>
                    <tr><td>الترقية لمراقب</td><td class="check">✔</td><td class="check">✔</td><td class="cross">✘</td></tr>
                    <tr><td>إنشاء غرفة خاصة</td><td class="check">✔</td><td class="cross">✘</td><td class="cross">✘</td></tr>
                    <tr><td>مدة الاشتراك</td><td>60 يوم</td><td>60 يوم</td><td>60 يوم</td></tr>
                    <tr class="price-row">
                        <td>السعر</td>
                        <td>300 ريال</td>
                        <td>250 ريال</td>
                        <td>200 ريال</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <div class="contact-card">
            <h3>جاهز للتميز؟</h3>
            <p>اختر باقتك المفضلة وتواصل مع الإدارة لتفعيل عضويتك فوراً</p>
            
            <a href="https://storied-llama-c463e0.netlify.app/" class="btn-contact">تواصل مع الإدارة الآن</a>
            
            <div class="note">سيتم توجيهك لصفحة الدعم الفني الخاصة بشات الأقصى</div>
            <div class="note" style="color: #555; font-size: 0.8rem; margin-top: 5px;">* لا يمكن استرداد المبلغ بعد تفعيل الاشتراك.</div>
        </div>
    </div>

</body>
</html>
