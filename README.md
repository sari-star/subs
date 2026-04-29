<DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>اشتراكات شات الأقصى | Al-Aqsa Chat</title>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;500;700;900&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold-gradient: linear-gradient(135deg, #bf953f, #fcf6ba, #b38728, #fbf5b7, #aa771c);
            --dark-bg: #0d0d0d;
            --card-bg: #1a1a1a;
            --accent-gold: #d4af37;
            --text-main: #ffffff;
            --text-muted: #a0a0a0;
        }

        * {
            box-sizing: border-box;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            margin: 0;
            padding: 0;
            background-color: var(--dark-bg);
            color: var(--text-main);
            font-family: 'Tajawal', sans-serif;
            overflow-x: hidden;
        }

        /* ✨ هيدر عصري */
        .hero-section {
            position: relative;
            height: 450px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: linear-gradient(rgba(0,0,0,0.8), rgba(13,13,13,1)), 
                        url('https://images.unsplash.com/photo-1590076215667-873d3950ef31?q=80&w=2070&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
            padding: 20px;
        }

        .hero-section::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: var(--gold-gradient);
        }

        h1 {
            font-size: clamp(2.5rem, 8vw, 4.5rem);
            font-weight: 900;
            margin: 0;
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            filter: drop-shadow(0 5px 15px rgba(212, 175, 55, 0.2));
        }

        .subtitle {
            font-size: 1.3rem;
            color: var(--text-muted);
            margin-top: 15px;
            letter-spacing: 1px;
        }

        /* 📊 جدول الاشتراك الاحترافي */
        .container {
            max-width: 1100px;
            margin: -60px auto 60px auto;
            padding: 0 20px;
            position: relative;
            z-index: 10;
        }

        .table-responsive {
            background: var(--card-bg);
            border-radius: 24px;
            padding: 10px;
            box-shadow: 0 25px 50px rgba(0,0,0,0.5);
            border: 1px solid rgba(255,255,255,0.05);
            overflow-x: auto; /* يجعل الجدول يسحب لليمين واليسار في الجوال */
        }

        table {
            width: 100%;
            border-collapse: collapse;
            min-width: 600px; /* يمنع الجدول من الانضغاط بشكل قبيح */
        }

        th {
            padding: 25px 15px;
            text-align: center;
            font-size: 1.2rem;
            color: var(--accent-gold);
            border-bottom: 2px solid #2a2a2a;
        }

        td {
            padding: 20px 15px;
            text-align: center;
            border-bottom: 1px solid #252525;
            color: #d1d1d1;
            font-weight: 500;
        }

        tr:last-child td { border-bottom: none; }

        tr:hover td {
            background-color: rgba(255,255,255,0.02);
        }

        /* أيقونات التميز */
        .check { color: #00ff88; font-size: 1.4rem; filter: drop-shadow(0 0 5px rgba(0,255,136,0.3)); }
        .cross { color: #ff4b2b; font-size: 1.4rem; opacity: 0.5; }

        .price-label {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--accent-gold);
        }

        /* 📱 بطاقة التواصل */
        .contact-container {
            margin-top: 50px;
            text-align: center;
            padding: 60px 30px;
            background: radial-gradient(circle at center, #1f1f1f 0%, #161616 100%);
            border-radius: 30px;
            border: 1px solid rgba(212, 175, 55, 0.2);
        }

        .btn-premium {
            display: inline-block;
            padding: 18px 50px;
            background: var(--gold-gradient);
            color: #000;
            text-decoration: none;
            border-radius: 100px;
            font-weight: 800;
            font-size: 1.2rem;
            transition: all 0.3s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.3);
            margin-top: 25px;
        }

        .btn-premium:hover {
            transform: scale(1.05) translateY(-5px);
            box-shadow: 0 15px 40px rgba(212, 175, 55, 0.5);
        }

        .footer-note {
            margin-top: 30px;
            font-size: 0.9rem;
            color: var(--text-muted);
        }

        /* 📱 تعديلات الشاشات الصغيرة */
        @media (max-width: 768px) {
            .hero-section { height: 350px; }
            h1 { font-size: 2.8rem; }
            .container { margin-top: -40px; }
            .table-responsive { border-radius: 15px; }
            th, td { padding: 15px 10px; font-size: 0.95rem; }
            .btn-premium { width: 100%; padding: 15px 20px; }
        }

        /* تجميل شريط التمرير */
        .table-responsive::-webkit-scrollbar {
            height: 6px;
        }
        .table-responsive::-webkit-scrollbar-thumb {
            background: var(--accent-gold);
            border-radius: 10px;
        }
    </style>
</head>
<body>

    <header class="hero-section">
        <h1>شات الأقصى</h1>
        <div class="subtitle">فخامة الحوار.. وجمال اللقاء</div>
    </header>

    <main class="container">
        <div class="table-responsive">
            <table>
                <thead>
                    <tr>
                        <th style="text-align: right; padding-right: 30px;">المميزات الملكية</th>
                        <th>الذهبي</th>
                        <th>الفضي</th>
                        <th>البرونزي</th>
                    </tr>
                </thead>
                <tbody>
                    <tr><td style="text-align: right; padding-right: 30px;">صلاحيات الطرد والحظر</td><td class="check">✦</td><td class="check">✦</td><td class="check">✦</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">إدارة الصور والمحتوى</td><td class="check">✦</td><td class="check">✦</td><td class="check">✦</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">نظام الهدايا الحصري</td><td class="check">✦</td><td class="check">✦</td><td class="check">✦</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">زخرفة النك نيم المتقدمة</td><td class="check">✦</td><td class="check">✦</td><td class="check">✦</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">الخصوصية والمحادثات</td><td class="check">✦</td><td class="check">✦</td><td class="check">✦</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">كشف المتخفين</td><td class="check">✦</td><td class="check">✦</td><td class="check">✦</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">الترقية لرتبة مراقب</td><td class="check">✦</td><td class="check">✦</td><td class="cross">✕</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">إنشاء غرف خاصة مستقلة</td><td class="check">✦</td><td class="cross">✕</td><td class="cross">✕</td></tr>
                    <tr><td style="text-align: right; padding-right: 30px;">مدة الصلاحية</td><td>60 يوم</td><td>60 يوم</td><td>60 يوم</td></tr>
                    <tr style="background: rgba(212, 175, 55, 0.05);">
                        <td style="text-align: right; padding-right: 30px; font-weight: bold; color: var(--accent-gold);">قيمة الاستثمار</td>
                        <td class="price-label">300 ريال</td>
                        <td class="price-label">250 ريال</td>
                        <td class="price-label">200 ريال</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <section class="contact-container">
            <h3 style="font-size: 2rem; margin-bottom: 10px;">هل أنت مستعد لتكون مميزاً؟</h3>
            <p style="color: var(--text-muted); max-width: 600px; margin: 0 auto;">انضم إلى نخبة الأعضاء في شات الأقصى وتمتع بصلاحيات لا حدود لها.</p>
            
            <a href="https://storied-llama-c463e0.netlify.app/" class="btn-premium">تواصل مع الإدارة الآن</a>
            
            <div class="footer-note">
                <p>⚠️ سيتم توجيهك مباشرة لمركز الدعم الفني</p>
                <p style="opacity: 0.6; font-size: 0.8rem;">* ملاحظة: الرسوم المدفوعة غير قابلة للاسترداد بعد تفعيل الخدمة.</p>
            </div>
        </section>
    </main>

</body>
</html>
