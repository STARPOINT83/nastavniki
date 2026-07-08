# nastavniki
да
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Наставник колледжа — Поп-арт</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,600;14..32,700;14..32,900&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: #C8FF19;
            background-image:
                radial-gradient(circle at 20% 20%, rgba(255,255,255,.18) 0 8%, transparent 9%),
                radial-gradient(circle at 80% 70%, rgba(255,255,255,.15) 0 7%, transparent 8%),
                radial-gradient(circle at 60% 40%, rgba(255,255,255,.12) 0 6%, transparent 7%);
            padding: 40px;
            min-height: 100vh;
            overflow-x: hidden;
        }

        .bg-decor {
            position: fixed;
            inset: 0;
            pointer-events: none;
            overflow: hidden;
            z-index: 0;
        }

        .blob {
            position: absolute;
            border: 5px solid #000;
            filter: drop-shadow(10px 10px 0 #000);
            animation: float 8s ease-in-out infinite;
        }
        .blob1 {
            width: 220px;
            height: 220px;
            background: #00E7FF;
            border-radius: 53% 47% 63% 37%;
            left: -70px;
            top: -50px;
        }
        .blob2 {
            width: 180px;
            height: 180px;
            background: #FFEF00;
            right: -50px;
            top: 180px;
            animation-delay: 2s;
            border-radius: 60% 40% 50% 50%;
        }
        .blob3 {
            width: 260px;
            height: 260px;
            background: #FF4FC7;
            bottom: -100px;
            right: -100px;
            border-radius: 45% 55% 55% 45%;
            animation-delay: 4s;
        }

        .star {
            position: absolute;
            font-size: 60px;
            font-weight: bold;
            color: #000;
            animation: spinStar 12s linear infinite;
        }
        .s1 { top: 90px; right: 140px; }
        .s2 { bottom: 130px; left: 80px; font-size: 45px; }
        .s3 { left: 40%; top: 40px; font-size: 70px; }

        .circle {
            position: absolute;
            border: 5px solid #000;
            border-radius: 50%;
        }
        .c1 { width: 50px; height: 50px; background: #fff; top: 200px; left: 100px; }
        .c2 { width: 70px; height: 70px; background: #ff4fc7; right: 120px; bottom: 140px; }
        .c3 { width: 40px; height: 40px; background: #00e7ff; left: 70%; top: 80%; }

        .zigzag {
            position: absolute;
            width: 120px;
            height: 12px;
            background: repeating-linear-gradient(45deg, #000 0 8px, transparent 8px 16px);
        }
        .z1 { top: 320px; right: 40px; transform: rotate(25deg); }
        .z2 { bottom: 100px; left: 30px; transform: rotate(-25deg); }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-18px) rotate(4deg); }
        }
        @keyframes spinStar {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        .left-hand,
        .right-hand {
            position: fixed;
            font-size: 260px;
            z-index: 1;
            filter: drop-shadow(8px 8px 0 #000);
            animation: handMove 5s ease-in-out infinite;
            user-select: none;
            pointer-events: none;
        }
        .left-hand {
            left: -60px;
            top: 80px;
            transform: rotate(-25deg);
        }
        .right-hand {
            right: -60px;
            bottom: 60px;
            transform: rotate(35deg);
            animation-delay: 2s;
        }

        .sticker {
            position: fixed;
            padding: 12px 22px;
            background: #fff;
            border: 4px solid #000;
            font-weight: 900;
            font-size: 28px;
            box-shadow: 8px 8px 0 #000;
            transform: rotate(-8deg);
            z-index: 3;
        }
        .sticker1 {
            background: #FFE500;
            top: 50px;
            right: 90px;
        }
        .sticker2 {
            background: #00E7FF;
            left: 80px;
            bottom: 120px;
            transform: rotate(10deg);
        }
        .sticker3 {
            background: #FF4FC7;
            right: 250px;
            bottom: 80px;
            width: 70px;
            height: 70px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
        }

        @keyframes handMove {
            0% { transform: translateY(0) scale(1); }
            50% { transform: translateY(-20px) scale(1.03); }
            100% { transform: translateY(0) scale(1); }
        }

        .form-card {
            max-width: 760px;
            width: 100%;
            margin: auto;
            position: relative;
            z-index: 5;
            background: linear-gradient(145deg, #ff6dd5, #ff3db8);
            border: 6px solid #000;
            border-radius: 28px;
            padding: 35px;
            box-shadow: 20px 20px 0 #000, 0 0 50px rgba(255, 0, 180, 0.4);
        }

        h1 {
            color: #000;
            font-size: 2.2rem;
            font-weight: 900;
            letter-spacing: 1px;
            text-transform: uppercase;
            margin-bottom: 15px;
        }

        .badge {
            background: #000;
            color: #C8FF19;
            border-radius: 0;
            padding: 8px 18px;
            font-size: .8rem;
            display: inline-block;
            margin-top: 10px;
        }

        .subhead {
            margin-top: 20px;
            margin-bottom: 30px;
            background: #fff;
            border: 4px solid #000;
            padding: 20px;
            border-radius: 18px;
            color: #000;
            line-height: 1.7;
            font-weight: 600;
        }

        .form-group {
            margin-bottom: 20px;
        }

        label {
            display: block;
            font-weight: 800;
            color: #000;
            margin-bottom: 8px;
        }

        input,
        select,
        textarea {
            width: 100%;
            padding: 16px;
            border: 4px solid #000;
            border-radius: 18px;
            background: #fff;
            color: #000;
            font-size: 16px;
            font-weight: 600;
            box-shadow: 8px 8px 0 #000;
            transition: .2s;
            font-family: 'Inter', sans-serif;
        }

        input:focus,
        textarea:focus,
        select:focus {
            outline: none;
            border-color: #ff0088;
            transform: translate(-2px, -2px);
            box-shadow: 12px 12px 0 #000;
        }

        textarea {
            min-height: 130px;
            resize: vertical;
        }

        .inline-group,
        .form-row {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }

        .inline-group .form-group,
        .form-row .form-group {
            flex: 1;
        }

        .checkbox-group,
        .radio-group {
            background: #00E7FF;
            border: 4px solid #000;
            border-radius: 20px;
            padding: 18px;
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
        }

        .checkbox-item,
        .radio-item {
            font-weight: 700;
            color: #000;
            display: flex;
            align-items: center;
            gap: 10px;
            cursor: pointer;
        }

        input[type="checkbox"],
        input[type="radio"] {
            width: 22px;
            height: 22px;
            accent-color: #ff0088;
            box-shadow: none;
            flex-shrink: 0;
        }

        .file-upload {
            background: #fff;
            border: 4px dashed #000;
            border-radius: 20px;
            padding: 25px;
            text-align: center;
            cursor: pointer;
            transition: .2s;
            font-weight: 700;
            color: #000;
        }

        .file-upload:hover {
            background: #C8FF19;
            transform: rotate(-1deg);
        }

        .file-upload .file-label {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 6px;
            cursor: pointer;
        }

        .file-upload .file-icon {
            font-size: 2rem;
        }

        .file-upload input {
            display: none;
        }

        .btn-submit {
            width: 100%;
            padding: 18px;
            margin-top: 25px;
            background: #000;
            color: #C8FF19;
            border: 4px solid #000;
            border-radius: 18px;
            font-size: 20px;
            font-weight: 900;
            text-transform: uppercase;
            cursor: pointer;
            box-shadow: 10px 10px 0 #ff4fc7;
            transition: .2s;
            font-family: 'Inter', sans-serif;
        }

        .btn-submit:hover {
            background: #ff4fc7;
            color: #000;
            transform: translate(-4px, -4px);
            box-shadow: 16px 16px 0 #000;
        }

        .btn-submit:active {
            transform: translate(5px, 5px);
            box-shadow: 4px 4px 0 #000;
        }

        .btn-submit:disabled {
            opacity: 0.6;
            cursor: not-allowed;
            transform: none !important;
            box-shadow: 10px 10px 0 #ff4fc7;
        }

        .footer-note {
            margin-top: 30px;
            text-align: center;
            font-weight: 700;
            color: #000;
        }

        .loading-spinner {
            display: inline-block;
            width: 20px;
            height: 20px;
            border: 3px solid rgba(255,255,255,.3);
            border-top-color: #fff;
            border-radius: 50%;
            animation: spin .7s linear infinite;
        }

        @keyframes spin {
            to { transform: rotate(360deg); }
        }

        .debug-info {
            margin-top: 20px;
            padding: 15px;
            background: #fff;
            border: 4px solid #000;
            border-radius: 18px;
            display: none;
            font-weight: 600;
            white-space: pre-wrap;
            word-break: break-all;
            max-height: 300px;
            overflow-y: auto;
        }

        .debug-info.show {
            display: block;
        }
        .debug-info .error {
            color: #dc3545;
        }
        .debug-info .success {
            color: #28a745;
        }

        @media (max-width: 700px) {
            .inline-group,
            .form-row {
                flex-direction: column;
            }
            .form-card {
                padding: 20px;
            }
            h1 {
                font-size: 32px;
            }
            .left-hand,
            .right-hand {
                font-size: 120px;
            }
            .left-hand {
                left: -30px;
                top: 40px;
            }
            .right-hand {
                right: -30px;
                bottom: 30px;
            }
            .sticker {
                font-size: 18px;
                padding: 8px 14px;
            }
            .sticker1 { top: 20px; right: 20px; }
            .sticker2 { left: 20px; bottom: 60px; }
            .sticker3 { right: 20px; bottom: 40px; width: 50px; height: 50px; }
            .blob1, .blob2, .blob3 {
                display: none;
            }
            .star, .circle, .zigzag {
                display: none;
            }
        }
    </style>
</head>
<body>

    <!-- ============= ДЕКОР ============= -->
    <div class="bg-decor">
        <div class="blob blob1"></div>
        <div class="blob blob2"></div>
        <div class="blob blob3"></div>
        <div class="star s1">✦</div>
        <div class="star s2">✦</div>
        <div class="star s3">✦</div>
        <div class="circle c1"></div>
        <div class="circle c2"></div>
        <div class="circle c3"></div>
        <div class="zigzag z1"></div>
        <div class="zigzag z2"></div>
    </div>

    <!-- ============= РУКИ ============= -->
    <div class="left-hand">✋</div>
    <div class="right-hand">✋</div>

    <!-- ============= СТИКЕРЫ ============= -->
    <div class="sticker sticker1">WOW!</div>
    <div class="sticker sticker2">GO!</div>
    <div class="sticker sticker3">★</div>

    <!-- ============= ФОРМА ============= -->
    <div class="form-card">
        <h1>
            🧑‍🏫 Наставник<br>для первокурсников
            <span class="badge">Колледж → Старшие помогают</span>
        </h1>

        <div class="subhead">
            Ты учишься на <strong>2–4 курсе</strong> колледжа? Помоги первокурсникам освоиться, поделись опытом и стань частью команды наставников.<br>
            <strong style="color: #ff0088;">Заполни анкету — и мы свяжемся с тобой!</strong>
        </div>

        <form id="mentorForm" onsubmit="submitForm(event)">
            <!-- ФИО -->
            <div class="form-group">
                <label for="fullname">ФИО <span style="font-weight:400;">(полностью)</span></label>
                <input type="text" id="fullname" placeholder="Петров Алексей Сергеевич" required>
            </div>

            <!-- Контакты -->
            <div class="form-row">
                <div class="form-group">
                    <label for="phone">Телефон</label>
                    <input type="tel" id="phone" placeholder="+7 (999) 123-45-67" required>
                </div>
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" placeholder="alexey@college.ru" required>
                </div>
            </div>

            <!-- Курс и специальность -->
            <div class="inline-group">
                <div class="form-group">
                    <label for="course">Твой курс</label>
                    <select id="course" required>
                        <option value="">— выбери —</option>
                        <option value="2">2-й курс</option>
                        <option value="3">3-й курс</option>
                        <option value="4">4-й курс</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="specialty">Твоя специальность</label>
                    <input type="text" id="specialty" placeholder="Например: Сварочное производство" required>
                </div>
            </div>

            <!-- Группа первокурсников -->
            <div class="form-group">
                <label for="groupType">С какой группой первокурсников готов работать?</label>
                <select id="groupType" required>
                    <option value="">— выбери направление —</option>
                    <option value="Физическая культура">Физическая культура</option>
                    <option value="Дизайн">Дизайн</option>
                    <option value="Сварочное производство">Сварочное производство</option>
                    <option value="Операционная деятельность в логистике">Операционная деятельность в логистике</option>
                    <option value="Эксплуатация и обслуживание электрического и электромеханического оборудования">Эксплуатация и обслуживание электрического и электромеханического оборудования</option>
                    <option value="Оператор-наладчик металлообрабатывающих станков">Оператор-наладчик металлообрабатывающих станков</option>
                    <option value="Мастер слесарных работ">Мастер слесарных работ</option>
                    <option value="Электромонтер по ремонту и обслуживанию электрооборудования">Электромонтер по ремонту и обслуживанию электрооборудования</option>
                    <option value="Мастер отделочных строительных и декоративных работ">Мастер отделочных строительных и декоративных работ</option>
                    <option value="Мастер по ремонту и обслуживанию автомобилей">Мастер по ремонту и обслуживанию автомобилей</option>
                    <option value="Сварщик">Сварщик</option>
                    <option value="Строительство и эксплуатация зданий и сооружений">Строительство и эксплуатация зданий и сооружений</option>
                    <option value="Туризм и гостеприимство">Туризм и гостеприимство</option>
                    <option value="Конструирование, моделирование и технология изготовления изделий легкой промышленности">Конструирование, моделирование и технология изготовления изделий легкой промышленности</option>
                    <option value="Технология машиностроения">Технология машиностроения</option>
                </select>
            </div>

            <!-- Опыт наставничества -->
            <div class="form-group">
                <label>Был ли ты наставником раньше?</label>
                <div class="radio-group">
                    <label class="radio-item">
                        <input type="radio" name="experience" value="Да, был" required> Да, был
                    </label>
                    <label class="radio-item">
                        <input type="radio" name="experience" value="Нет, но хочу попробовать" required> Нет, но хочу попробовать
                    </label>
                    <label class="radio-item">
                        <input type="radio" name="experience" value="Помогал неформально" required> Помогал неформально
                    </label>
                </div>
            </div>

            <!-- Навыки -->
            <div class="form-group">
                <label>Чем можешь помочь первокурсникам? <span style="font-weight:400;">(выбери несколько)</span></label>
                <div class="checkbox-group">
                    <label class="checkbox-item">
                        <input type="checkbox" name="skills" value="Практические занятия / лабораторные"> Практические занятия / лабораторные
                    </label>
                    <label class="checkbox-item">
                        <input type="checkbox" name="skills" value="Теория / подготовка к экзаменам"> Теория / подготовка к экзаменам
                    </label>
                    <label class="checkbox-item">
                        <input type="checkbox" name="skills" value="Курсовые и проектные работы"> Курсовые и проектные работы
                    </label>
                    <label class="checkbox-item">
                        <input type="checkbox" name="skills" value="Адаптация в колледже"> Адаптация в колледже (расписание, традиции)
                    </label>
                    <label class="checkbox-item">
                        <input type="checkbox" name="skills" value="Профориентация / практика"> Профориентация / практика / стажировки
                    </label>
                    <label class="checkbox-item">
                        <input type="checkbox" name="skills" value="Бытовые вопросы"> Бытовые вопросы (общежитие, стипендия)
                    </label>
                </div>
            </div>

            <!-- Мотивация -->
            <div class="form-group">
                <label for="motivation">Почему ты хочешь стать наставником?</label>
                <textarea id="motivation" placeholder="Расскажи, что тебя вдохновляет, какой опыт у тебя есть, и почему первокурсникам будет полезно с тобой..." required></textarea>
            </div>

            <!-- Дополнительно -->
            <div class="form-row">
                <div class="form-group">
                    <label for="additional">Дополнительно <span style="font-weight:400;">(соцсети, портфолио)</span></label>
                    <input type="text" id="additional" placeholder="https://t.me/yourprofile">
                </div>
                <div class="form-group">
                    <label>Загрузить файл <span style="font-weight:400;">(необязательно)</span></label>
                    <div class="file-upload" onclick="document.getElementById('fileInput').click()">
                        <div class="file-label">
                            <span class="file-icon">📎</span>
                            <span>Нажми, чтобы выбрать файл</span>
                            <span style="font-size: 0.75rem; opacity: 0.7;">PNG, JPG, PDF до 5 МБ</span>
                        </div>
                        <input type="file" id="fileInput" accept=".png,.jpg,.jpeg,.pdf">
                    </div>
                </div>
            </div>

            <!-- Согласие -->
            <div class="form-group" style="margin-top: 10px;">
                <label class="checkbox-item" style="gap: 12px; padding: 6px 0; background: transparent; border: none;">
                    <input type="checkbox" id="consent" required style="width: 22px; height: 22px;">
                    <span>Я согласен(на) на обработку персональных данных и готов(а) помогать первокурсникам 💪</span>
                </label>
            </div>

            <button type="submit" class="btn-submit" id="submitBtn">
                <span>📩</span> Отправить заявку
            </button>

            <div class="footer-note">
                <span>#НаставникКолледжа</span> — после отправки с тобой свяжется руководитель программы в течение 2–3 дней.
            </div>
        </form>

        <!-- Отладка -->
        <div class="debug-info" id="debugInfo">
            <strong>📋 Отладка:</strong>
            <div id="debugContent"></div>
        </div>
    </div>

    <script>
        // ✅ Ваш бот
        const BOT_TOKEN = '8824496618:AAHzosvv01ob30FIGvHTKl72uVhv_yVl2ds';
        
        // ✅ ДВА получателя: ваш ID и новый ID
        const CHAT_IDS = ['8251845054', '1366550195'];

        function getSafeValue(value, defaultValue = 'не указано') {
            if (value === null || value === undefined || value === '') {
                return defaultValue;
            }
            return value;
        }

        async function sendToTelegram(chatId, message, file) {
            const response = await fetch(`https://api.telegram.org/bot${BOT_TOKEN}/sendMessage`, {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify({
                    chat_id: chatId,
                    text: message,
                    parse_mode: 'HTML'
                })
            });
            const result = await response.json();
            
            if (!result.ok) {
                throw new Error(`Ошибка отправки для ID ${chatId}: ${result.description}`);
            }

            if (file) {
                const fileData = new FormData();
                fileData.append('chat_id', chatId);
                fileData.append('document', file);
                await fetch(`https://api.telegram.org/bot${BOT_TOKEN}/sendDocument`, {
                    method: 'POST',
                    body: fileData
                });
            }
            
            return result;
        }

        async function submitForm(e) {
            e.preventDefault();

            const form = document.getElementById('mentorForm');
            const submitBtn = document.getElementById('submitBtn');
            const debugInfo = document.getElementById('debugInfo');
            const debugContent = document.getElementById('debugContent');

            debugInfo.classList.add('show');
            debugContent.innerHTML = '⏳ Отправка...';

            submitBtn.disabled = true;
            submitBtn.innerHTML = '<span class="loading-spinner"></span> Отправка...';

            try {
                const formData = new FormData(form);

                const fullname = getSafeValue(formData.get('fullname'));
                const phone = getSafeValue(formData.get('phone'));
                const email = getSafeValue(formData.get('email'));
                const course = getSafeValue(formData.get('course'), 'не выбран');
                const specialty = getSafeValue(formData.get('specialty'), 'не указана');
                const groupType = getSafeValue(formData.get('groupType'), 'не выбрано');
                const experience = getSafeValue(
                    document.querySelector('input[name="experience"]:checked')?.value,
                    'не выбрано'
                );

                const skills = [];
                document.querySelectorAll('input[name="skills"]:checked').forEach(cb => {
                    skills.push(cb.value);
                });
                const skillsText = skills.length ? skills.map(s => `  • ${s}`).join('\n') : '  • не выбрано';

                const motivation = getSafeValue(formData.get('motivation'));
                const additional = getSafeValue(formData.get('additional'));

                const fileInput = document.getElementById('fileInput');
                const file = fileInput.files[0] || null;
                const fileName = file ? file.name : 'не загружен';

                const message = `🎓 НОВАЯ ЗАЯВКА НА НАСТАВНИКА

👤 ФИО: ${fullname}
📞 Телефон: ${phone}
📧 Email: ${email}

📚 Курс: ${course}
🔧 Специальность: ${specialty}
📋 Группа первокурсников: ${groupType}

⭐ Опыт наставничества: ${experience}

🛠 Навыки:
${skillsText}

💬 Мотивация:
${motivation}

🔗 Дополнительно: ${additional}
📎 Файл: ${fileName}

📅 Дата: ${new Date().toLocaleString('ru-RU')}`;

                debugContent.innerHTML = '📤 Отправка в Telegram...';

                const testResponse = await fetch(`https://api.telegram.org/bot${BOT_TOKEN}/getMe`);
                const testData = await testResponse.json();

                if (!testData.ok) {
                    throw new Error('❌ Бот не активен! Проверьте токен.');
                }
                debugContent.innerHTML += `\n✅ Бот активен: @${testData.result.username}`;

                let successCount = 0;
                let errors = [];

                for (const chatId of CHAT_IDS) {
                    try {
                        debugContent.innerHTML += `\n📨 Отправка для ID ${chatId}...`;
                        await sendToTelegram(chatId, message, file);
                        successCount++;
                        debugContent.innerHTML += ` ✅`;
                    } catch (err) {
                        errors.push(`ID ${chatId}: ${err.message}`);
                        debugContent.innerHTML += ` ❌`;
                    }
                }

                if (successCount > 0) {
                    debugContent.innerHTML += `\n✅ УСПЕШНО ОТПРАВЛЕНО ${successCount} из ${CHAT_IDS.length} получателей!`;
                    alert(`✅ Заявка успешно отправлена! (${successCount} из ${CHAT_IDS.length} получателей)`);
                    form.reset();
                    document.querySelector('.file-upload .file-label span:nth-child(2)').innerText = 'Нажми, чтобы выбрать файл';
                } else {
                    throw new Error(`Не удалось отправить ни одному получателю: ${errors.join('; ')}`);
                }

            } catch (error) {
                console.error('Ошибка:', error);
                debugContent.innerHTML += `\n❌ Ошибка: ${error.message}`;
                alert(`❌ Ошибка: ${error.message}\n\nПроверьте отладку внизу страницы.`);
            } finally {
                submitBtn.disabled = false;
                submitBtn.innerHTML = '<span>📩</span> Отправить заявку';
            }
        }

        document.getElementById('fileInput')?.addEventListener('change', function(e) {
            const fileName = this.files[0]?.name;
            if (fileName) {
                const label = this.closest('.file-upload').querySelector('.file-label span:nth-child(2)');
                if (label) label.innerText = `📄 ${fileName}`;
            }
        });
    </script>

</body>
</html>

---

## 📋 Поля формы

| Поле | Описание |
|------|----------|
| ФИО | Полное имя кандидата |
| Телефон | Контактный номер |
| Email | Электронная почта |
| Курс | 2-й, 3-й или 4-й курс |
| Специальность | Направление обучения |
| Группа первокурсников | С какой группой готов работать |
| Опыт наставничества | Был ли наставником раньше |
| Навыки | Чем может помочь (множественный выбор) |
| Мотивация | Почему хочет стать наставником |
| Дополнительно | Соцсети, портфолио |
| Файл | Резюме или фото (необязательно) |

---

## 🤖 Telegram

Заявки отправляются в Telegram-бота:

- **Бот:** @Technulikbot
- **Получатели:** ID `8251845054` и `1366550195`

---

## 🛠️ Технологии

- HTML5
- CSS3 (поп-арт стиль)
- JavaScript (отправка в Telegram API)

---

## 📄 Лицензия

MIT License — свободно используйте и изменяйте!

---

## 🙌 Автор

Сделано для колледжа — старшие помогают младшим!
