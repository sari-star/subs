<DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>الاشتراكات | شات الاقصى</title>
    <meta name="description" content="اختر باقة الاشتراك المناسبة واستمتع بمزايا حصرية في اشتراكات شات الاقصى للجوال">
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #2563eb;
            --primary-light: #3b82f6;
            --primary-dark: #1e40af;
            --secondary: #f97316;
            --secondary-light: #fb923c;
            --accent: #ef4444;
            --accent-light: #f87171;
            --success: #10b981;
            --success-light: #34d399;
            --warning: #f59e0b;
            --warning-light: #fbbf24;
            --bg: #fafafa;
            --card: #ffffff;
            --text: #1f2937;
            --text-light: #6b7280;
            --border: #e5e7eb;
            --featured: #10b981;
            --shadow: rgba(37, 99, 235, 0.1);
        }

        body {
            -webkit-user-select: none;
            -moz-user-select: none;
            -ms-user-select: none;
            user-select: none;
            font-family: 'Tajawal', 'Segoe UI', Tahoma, sans-serif;
            background: linear-gradient(135deg, #f8fafc 0%, #f1f5f9 100%);
            color: var(--text);
            line-height: 1.8;
            padding: 20px;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .back-btn {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: white;
            color: var(--primary);
            padding: 12px 25px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            margin-bottom: 30px;
            transition: all 0.3s ease;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
            border: 1px solid var(--border);
        }

        .back-btn:hover {
            background: var(--primary);
            color: white;
            transform: translateX(-5px);
        }

        .hero-section {
            background: linear-gradient(135deg, var(--primary-dark) 0%, #1e3a8a 100%);
            color: white;
            padding: 60px 40px;
            border-radius: 30px;
            text-align: center;
            margin-bottom: 50px;
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
        }

        .hero-section h1 {
            font-size: 2.8em;
            margin-bottom: 15px;
            font-weight: 800;
        }

        .card {
            background: var(--card);
            border-radius: 24px;
            padding: 40px;
            margin-bottom: 40px;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.05);
            border: 1px solid var(--border);
        }

        .section-title {
            color: var(--text);
            font-size: 1.8em;
            margin-bottom: 30px;
            padding-right: 20px;
            border-right: 6px solid var(--primary);
            font-weight: 800;
        }

        .tiers-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
            margin: 30px 0;
        }

        .tier-card {
            background: white;
            padding: 35px 25px;
            border-radius: 24px;
            text-align: center;
            transition: all 0.4s ease;
            border: 2px solid var(--border);
            position: relative;
        }

        .tier-card:hover {
            transform: translateY(-10px);
            border-color: var(--primary-light);
            box-shadow: 0 15px 30px rgba(0,0,0,0.1);
        }

        .tier-card.featured {
            border-color: var(--featured);
            background: linear-gradient(to bottom, #ffffff, #f0fdf4);
        }

        .featured-badge {
            position: absolute;
            top: -15px;
            left: 50%;
            transform: translateX(-50%);
            background: var(--featured);
            color: white;
            padding: 6px 20px;
            border-radius: 50px;
            font-size: 0.85em;
            font-weight: 700;
        }

        .tier-name {
            font-weight: 800;
            font-size: 1.4em;
            margin-bottom: 10px;
        }

        .tier-price {
            font-size: 3em;
            color: var(--primary);
            font-weight: 900;
            margin: 10px 0;
        }

        .tier-price span {
            font-size: 0.4em;
            color: var(--text-light);
        }

        .tier-duration {
            color: var(--text-light);
            font-weight: 500;
        }

        .table-wrapper {
            width: 100%;
            overflow-x: auto;
            margin: 30px 0;
            border-radius: 20px;
            border: 1px solid var(--border);
        }

        .permissions-table {
            width: 100%;
            border-collapse: collapse;
            background: white;
            min-width: 1000px;
        }

        .permissions-table th, .permissions-table td {
            padding: 18px;
            text-align: center;
            border-bottom: 1px solid var(--border);
        }

        .permissions-table th {
            background: #f8fafc;
            font-weight: 800;
        }

        .permission-name {
            text-align: right !important;
            font-weight: 700;
            background: #fdfdfd;
            position: sticky;
            right: 0;
            z-index: 2;
            border-left: 2px solid var(--border);
        }

        .tier-check { color: var(--success); font-size: 1.4em; font-weight: bold; }
        .tier-cross { color: #d1d5db; font-size: 1.2em; }

        .info-box {
            background: #eff6ff;
            padding: 25px;
            border-radius: 20px;
            border-right: 6px solid var(--primary);
            margin-top: 20px;
        }

        .payment-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .payment-card {
            background: #f8fafc;
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            border: 1px dashed var(--border);
        }

        .payment-card .icon { font-size: 2em; margin-bottom: 10px; }

        .warning-box {
            background: #fff1f2;
            padding: 20px;
            border-radius: 15px;
            border-right: 6px solid var(--accent);
            margin-top: 25px;
        }

        /* تنسيقات الأقسام الجديدة */
        .response-time-box {
            background: linear-gradient(135deg, #1e2937 0%, #374151 100%);
            color: white;
            padding: 30px;
            border-radius: 20px;
            margin-bottom: 40px;
            display: flex;
            align-items: center;
            gap: 20px;
            border-right: 8px solid var(--warning);
        }

        .response-time-box h3 { color: var(--warning); margin-bottom: 10px; }

        .steps-list { list-style: none; counter-reset: my-counter; }
        .steps-list li {
            padding: 15px 45px 15px 15px;
            margin-bottom: 10px;
            background: #f9fafb;
            border-radius: 12px;
            position: relative;
            font-weight: 600;
        }
        .steps-list li::before {
            content: counter(my-counter);
            counter-increment: my-counter;
            position: absolute;
            right: 15px;
            top: 50%;
            transform: translateY(-50%);
            width: 25px;
            height: 25px;
            background: var(--primary);
            color: white;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.8em;
        }

        .advantages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }
        .adv-item {
            background: #f0fdf4;
            padding: 15px;
            border-radius: 12px;
            color: #166534;
            font-weight: 600;
            border-right: 4px solid var(--success);
        }

        .elite-gift {
            background: #fffbeb;
            padding: 15px;
            border-radius: 12px;
            margin-bottom: 10px;
            border: 1px solid #fde68a;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .terms-box {
            background: #f8fafc;
            padding: 30px;
            border-radius: 20px;
            border: 1px solid var(--border);
        }
        .terms-list { padding-right: 20px; }
        .terms-list li { margin-bottom: 12px; position: relative; list-style: none; padding-right: 20px; }
        .terms-list li::before {
            content: "•";
            position: absolute;
            right: 0;
            color: var(--primary);
            font-weight: bold;
        }

        .note-tag {
            background: #fef2f2;
            color: #991b1b;
            padding: 15px;
            border-radius: 12px;
            margin-top: 20px;
            border-right: 5px solid var(--accent);
            font-weight: 700;
        }

        .footer {
            text-align: center;
            padding: 60px 20px;
            border-top: 1px solid var(--border);
        }

        @media (max-width: 768px) {
            .hero-section h1 { font-size: 2em; }
            .card { padding: 20px; }
            .response-time-box { flex-direction: column; text-align: center; }
        }
    </style>
</head>
<body oncontextmenu="return false;">

    <div class="container">
        <a href="https://www.chat-jawwal.com" class="back-btn">
            <span>←</span> العودة إلى الشات الرئيسي
        </a>

        <div class="hero-section">
            <h1>💎 الاشتراكات المميزة</h1>
            <p>اختر الباقة المناسبة واستمتع بمزايا حصرية لا مثيل لها في شات الاقصى</p>
        </div>

        <div class="card">
            <h2 class="section-title">📦 الباقات المتاحة</h2>
            <div class="tiers-grid">
                <div class="tier-card featured">
                    <div class="featured-badge">الأكثر طلباً ⭐</div>
                    <div class="tier-name">💎 عضوية النخبة</div>
                    <div class="tier-price">600 <span>﷼</span></div>
                    <div class="tier-duration">لمدة 6 شهور</div>
                </div>
                <div class="tier-card">
                    <div class="tier-name">👑 التاج الملكي</div>
                    <div class="tier-price">500 <span>﷼</span></div>
                    <div class="tier-duration">لمدة 5 شهور</div>
                </div>
                <div class="tier-card">
                    <div class="tier-name">⚜️ عضوية التميز</div>
                    <div class="tier-price">400 <span>﷼</span></div>
                    <div class="tier-duration">لمدة 4 شهور</div>
                </div>
                <div class="tier-card">
                    <div class="tier-name">🌟 عضوية الكريستال</div>
                    <div class="tier-price">300 <span>﷼</span></div>
                    <div class="tier-duration">لمدة 4 شهور</div>
                </div>
                <div class="tier-card">
                    <div class="tier-name">⭐ النجمة الذهبية</div>
                    <div class="tier-price">200 <span>﷼</span></div>
                    <div class="tier-duration">لمدة 4 شهور</div>
                </div>
                <div class="tier-card">
                    <div class="tier-name">🌑 النجمة السوداء</div>
                    <div class="tier-price">150 <span>﷼</span></div>
                    <div class="tier-duration">لمدة 4 شهور</div>
                </div>
            </div>
        </div>

        <div class="card">
            <h2 class="section-title">🔧 جدول الصلاحيات</h2>
            <div class="table-wrapper">
                <table class="permissions-table">
                    <thead>
                        <tr>
                            <th class="permission-name">الميزة / الصلاحية</th>
                            <th>💎 النخبة</th>
                            <th>👑 الملكي</th>
                            <th>⚜️ التميز</th>
                            <th>🌟 الكريستال</th>
                            <th>⭐ الذهبية</th>
                            <th>🌑 السوداء</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td class="permission-name">طرد مستخدم</td>
                            <td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-cross">✗</td>
                        </tr>
                        <tr>
                            <td class="permission-name">الباند / الحظر / التشفير</td>
                            <td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-cross">✗</td><td class="tier-cross">✗</td>
                        </tr>
                        <tr>
                            <td class="permission-name">سحب المايك</td>
                            <td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td><td class="tier-check">✓</td>
                        </tr>
                        <tr>
                            <td class="permission-name">لوحة التحكم الكاملة</td>
                            <td class="tier-check">✓</td><td class="tier-cross">✗</td><td class="tier-cross">✗</td><td class="tier-cross">✗</td><td class="tier-cross">✗</td><td class="tier-cross">✗</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>

        <div class="card">
            <h2 class="section-title">💳 طرق الدفع المتاحة</h2>
            <div class="payment-grid">
                <div class="payment-card"><div class="icon">🏦</div><div>التحويل البنكي</div></div>
                <div class="payment-card"><div class="icon">💻</div><div>STC Pay</div></div>
                <div class="payment-card"><div class="icon">📱</div><div>Apple Pay</div></div>
                <div class="payment-card"><div class="icon">💳</div><div>بطاقات الائتمان</div></div>
            </div>
        </div>

        <div class="response-time-box">
            <div style="font-size: 3em;">⏰</div>
            <div>
                <h3>أوقات الاستجابة:</h3>
                <p>نحن متواجدون لخدمتك على مدار الساعة. متوسط وقت الاستجابة خلال <strong>15 دقيقة</strong> في الأوقات العادية. للحالات العاجلة، نستجيب فوراً!</p>
            </div>
        </div>

        <div class="card">
            <h2 class="section-title">💡 إرشادات الاشتراك</h2>
            <div style="margin-bottom: 30px;">
                <h3 style="margin-bottom: 15px; color: var(--primary);">📝 خطوات الاشتراك السهلة:</h3>
                <ul class="steps-list">
                    <li>اختر الباقة المناسبة لاحتياجاتك من الجدول أعلاه</li>
                    <li>تواصل معنا عبر إحدى قنوات التواصل المتاحة</li>
                    <li>اذكر اسم المستخدم الخاص بك بوضوح</li>
                    <li>اختر طريقة الدفع المناسبة لك</li>
                    <li>قم بالتحويل وأرسل إيصال الدفع</li>
                    <li>انتظر التفعيل خلال دقائق معدودة</li>
                </ul>
            </div>

            <div style="margin-bottom: 30px;">
                <h3 style="margin-bottom: 15px; color: var(--success);">✨ مزايا إضافية:</h3>
                <div class="advantages-grid">
                    <div class="adv-item">✓ تفعيل فوري بعد تأكيد الدفع</div>
                    <div class="adv-item">✓ دعم فني متواصل طوال فترة الاشتراك</div>
                    <div class="adv-item">✓ إشعار قبل انتهاء الاشتراك بوقت كافٍ</div>
                    <div class="adv-item">✓ ضمان استمرار الاشتراك</div>
                </div>
            </div>

            <div>
                <h3 style="margin-bottom: 15px; color: var(--warning-light);">🎁 مزايا عضوية النخبة الحصرية:</h3>
                <div class="elite-gift">🎁 غرفة خاصة مجانية مع الاشتراك</div>
                <div class="elite-gift">🎁 سوبر مجاني هدية لأي صديق تختاره</div>
                <div class="elite-gift">🎁 بانر خاص باسمك أو أيقونة خاصة</div>
            </div>
        </div>

        <div class="card">
            <h2 class="section-title">📜 شروط اشتراكات السوبر</h2>
            <div class="terms-box">
                <h4 style="margin-bottom: 20px; color: var(--text);">📋 عرض الشروط الكاملة:</h4>
                <ul class="terms-list">
                    <li>يجب إحضار إيصال التحويل حتى يتم قبول الاشتراك</li>
                    <li>لن يتم استرجاع المبلغ بعد التحويل لأي سبب كان</li>
                    <li>يُمنع الطرد أو الحظر إلا في حال وجود إثبات واضح على مخالفة قوانين الشات (السب، الشتم، السياسة، الدين)</li>
                    <li>يُمنع التلاعب بالصلاحيات أو استخدامها بطريقة غير مخصصة لها</li>
                    <li>يجب احترام جميع الأعضاء والإدارة وعدم استخدام ألفاظ خارجة عن الأدب</li>
                    <li>يُمنع استخدام الإعلانات لأغراض شخصية أو الترويج لحسابات خاصة</li>
                    <li>يُمنع منح العضوية لشخص آخر أو مشاركتها</li>
                    <li>الالتزام بنظام اللايكات (500 لايك للأعضاء الجدد كحد أقصى)</li>
                    <li>يُمنع نقل الرتب أو تغيير الأسماء أو منح الهدايا دون إذن</li>
                    <li>يُمنع استخدام صلاحية الطرد في الغرف العامة</li>
                    <li>يُمنع استخدام المخفي لأغراض التجسس في الغرف الخاصة</li>
                </ul>
                <div class="note-tag">
                    🔸 تنويه: في حال ارتكاب أي مخالفة، يحق للإدارة سحب صلاحية السوبر أو إيقاف العضوية مؤقتاً أو بشكل دائم.
                </div>
            </div>
        </div>

        <div class="footer">
            <p>جميع الحقوق محفوظة © 2026 <strong>شات الاقصى للجوال</strong></p>
        </div>
    </div>

    <script>
        document.addEventListener('contextmenu', e => e.preventDefault());
        document.onkeydown = function(e) {
            if (e.keyCode == 123 || (e.ctrlKey && (e.keyCode == 85 || e.keyCode == 73 || e.keyCode == 83))) return false;
        };
        setInterval(function() { debugger; }, 1000);
    </script>
</body>
</html>
