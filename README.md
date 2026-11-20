<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>بوابة النشاط التفاعلي للطلاب</title>
  <style>
    :root {
      --bg: #f4f7fb;
      --card: #ffffff;
      --primary: #1d4ed8;
      --primary-hover: #1e40af;
      --accent: #0f766e;
      --text: #0f172a;
      --muted: #475569;
      --border: #e2e8f0;
      --success-bg: #ecfdf5;
      --success-border: #10b981;
      --success-text: #065f46;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: "Segoe UI", Tahoma, Arial, sans-serif;
      background: var(--bg);
      color: var(--text);
      line-height: 1.7;
    }

    .container {
      max-width: 960px;
      margin: 0 auto;
      padding: 24px 16px 48px;
    }

    .hero {
      background: linear-gradient(135deg, #1d4ed8, #0f766e);
      color: #fff;
      border-radius: 18px;
      padding: 28px 24px;
      box-shadow: 0 10px 25px rgba(15, 23, 42, 0.1);
      margin-bottom: 24px;
    }

    .badge {
      display: inline-block;
      background: rgba(255, 255, 255, 0.18);
      padding: 4px 12px;
      border-radius: 999px;
      font-size: 0.85rem;
      margin-bottom: 10px;
    }

    .hero h1 {
      margin: 0 0 10px;
      font-size: 1.8rem;
    }

    .hero p {
      margin: 0;
      opacity: 0.95;
      font-size: 1.02rem;
    }

    .grid {
      display: grid;
      grid-template-columns: 1fr;
      gap: 20px;
    }

    @media (min-width: 768px) {
      .grid-2 {
        grid-template-columns: 1.1fr 0.9fr;
      }
    }

    .card {
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 22px;
      box-shadow: 0 4px 14px rgba(15, 23, 42, 0.04);
      margin-bottom: 20px;
    }

    .card h2 {
      margin: 0 0 12px;
      font-size: 1.25rem;
      color: var(--primary);
    }

    ol.steps {
      margin: 0;
      padding-right: 20px;
    }

    ol.steps li {
      margin-bottom: 8px;
      color: var(--text);
    }

    .link-box {
      background: #f8fafc;
      border: 1px dashed #94a3b8;
      border-radius: 12px;
      padding: 12px;
      font-size: 0.9rem;
      word-break: break-all;
      color: var(--muted);
      margin-bottom: 14px;
    }

    .btn-row {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    button, a.btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 8px;
      padding: 11px 18px;
      border-radius: 10px;
      border: none;
      font-size: 0.95rem;
      font-weight: 600;
      cursor: pointer;
      text-decoration: none;
      transition: 0.2s ease;
    }

    .btn-primary {
      background: var(--primary);
      color: #fff;
    }

    .btn-primary:hover {
      background: var(--primary-hover);
    }

    .btn-secondary {
      background: #e2e8f0;
      color: var(--text);
    }

    .btn-secondary:hover {
      background: #cbd5e1;
    }

    .embed-wrapper {
      border: 1px solid var(--border);
      border-radius: 14px;
      overflow: hidden;
      background: #fff;
      margin-top: 12px;
    }

    iframe {
      width: 100%;
      height: 540px;
      border: 0;
      display: block;
    }

    .notice {
      font-size: 0.88rem;
      color: var(--muted);
      background: #f1f5f9;
      padding: 10px 14px;
      border-radius: 10px;
      margin-top: 10px;
    }

    .form-group {
      margin-bottom: 14px;
    }

    label {
      display: block;
      font-weight: 600;
      margin-bottom: 6px;
      font-size: 0.95rem;
    }

    input[type="text"],
    textarea {
      width: 100%;
      padding: 10px 12px;
      border: 1px solid #cbd5e1;
      border-radius: 10px;
      font-family: inherit;
      font-size: 0.95rem;
      background: #fff;
    }

    input[type="text"]:focus,
    textarea:focus {
      outline: none;
      border-color: var(--primary);
      box-shadow: 0 0 0 3px rgba(29, 78, 216, 0.12);
    }

    textarea {
      min-height: 100px;
      resize: vertical;
    }

    .feedback {
      display: none;
      margin-top: 14px;
      padding: 14px;
      border-radius: 12px;
      background: var(--success-bg);
      border: 1px solid var(--success-border);
      color: var(--success-text);
      font-size: 0.92rem;
    }

    .submissions-list {
      margin-top: 16px;
      display: grid;
      gap: 10px;
    }

    .submission-item {
      border: 1px solid var(--border);
      background: #f8fafc;
      border-radius: 10px;
      padding: 12px;
      font-size: 0.9rem;
    }

    .submission-meta {
      font-weight: 700;
      color: var(--primary);
      margin-bottom: 4px;
    }
  </style>
</head>
<body>
  <div class="container">
    <header class="hero">
      <div class="badge">نشاط تعليمي تفاعلي</div>
      <h1>مرحباً بكم في النشاط التفاعلي</h1>
      <p>اطّلع على التعليمات، افتح النشاط التعليمي، ثم سجّل ملخص مشاركتك أو إجابتك في الأسفل.</p>
    </header>

    <div class="grid grid-2">
      <section class="card">
        <h2>تعليمات الطالب</h2>
        <ol class="steps">
          <li>اضغط على زر <strong>«فتح النشاط في نافذة جديدة»</strong> أو تفاعل معه مباشرة في الإطار أدناه.</li>
          <li>اقرأ محتوى النشاط بعناية وأكمل المطلوب خطوة بخطوة.</li>
          <li>بعد الانتهاء، اكتب اسمك وملخص ما تعلمته أو إجابتك في نموذج التسليم.</li>
          <li>انسخ ملخص الإجابة وأرسله لمعلمك عبر قناة الصف المعتمدة إذا طُلب منك ذلك.</li>
        </ol>
      </section>

      <section class="card">
        <h2>الوصول السريع للنشاط</h2>
        <div class="link-box" id="activityUrlText">
          https://claude.ai/artifact/QZFbwsBSEo6qGbdXYkebAr
        </div>
        <div class="btn-row">
          <a
            id="openActivityBtn"
            href="https://claude.ai/artifact/QZFbwsBSEo6qGbdXYkebAr"
            target="_blank"
            rel="noopener noreferrer"
            class="btn btn-primary"
          >
            فتح النشاط في نافذة جديدة
          </a>
          <button type="button" id="copyLinkBtn" class="btn btn-secondary">
            نسخ الرابط
          </button>
        </div>
        <div class="notice">
          إذا لم يظهر المحتوى داخل الإطار المدمج بسبب إعدادات الأمان في متصفحك أو في موقع المصدر، فاستخدم زر <strong>«فتح النشاط في نافذة جديدة»</strong>.
        </div>
      </section>
    </div>

    <section class="card">
      <h2>نافذة النشاط التفاعلي</h2>
      <div class="embed-wrapper">
        <iframe
          id="activityFrame"
          src="https://claude.ai/artifact/QZFbwsBSEo6qGbdXYkebAr"
          title="النشاط التفاعلي للطلاب"
          loading="lazy"
          allow="clipboard-write"
        ></iframe>
      </div>
    </section>

    <section class="card">
      <h2>تسجيل مشاركة الطالب</h2>
      <form id="studentForm">
        <div class="form-group">
          <label for="studentName">الاسم الثلاثي للطالب</label>
          <input type="text" id="studentName" placeholder="مثال: أحمد محمد السالم" required />
        </div>

        <div class="form-group">
          <label for="studentClass">الصف / المجموعة (اختياري)</label>
          <input type="text" id="studentClass" placeholder="مثال: أول ثانوي - أ" />
        </div>

        <div class="form-group">
          <label for="studentNote">إجابتك أو ملخص ما استفدته من النشاط</label>
          <textarea
            id="studentNote"
            placeholder="اكتب إجابتك أو الفكرة الرئيسية التي توصلت إليها..."
            required
          ></textarea>
        </div>

        <div class="btn-row">
          <button type="submit" class="btn btn-primary">حفظ وتوليد ملخص التسليم</button>
          <button type="button" id="copySummaryBtn" class="btn btn-secondary">نسخ ملخص التسليم</button>
        </div>
      </form>

      <div class="feedback" id="feedbackBox"></div>
      <div class="submissions-list" id="submissionsList"></div>
    </section>
  </div>

  <script>
    const ACTIVITY_URL = "https://claude.ai/artifact/QZFbwsBSEo6qGbdXYkebAr";
    const STORAGE_KEY = "student_activity_submissions_v1";

    const copyLinkBtn = document.getElementById("copyLinkBtn");
    const studentForm = document.getElementById("studentForm");
    const feedbackBox = document.getElementById("feedbackBox");
    const submissionsList = document.getElementById("submissionsList");
    const copySummaryBtn = document.getElementById("copySummaryBtn");

    let lastSummaryText = "";

    copyLinkBtn.addEventListener("click", async () => {
      try {
        await navigator.clipboard.writeText(ACTIVITY_URL);
        copyLinkBtn.textContent = "تم نسخ الرابط ✓";
        setTimeout(() => {
          copyLinkBtn.textContent = "نسخ الرابط";
        }, 2000);
      } catch {
        alert("انسخ الرابط يدوياً: " + ACTIVITY_URL);
      }
    });

    function loadSubmissions() {
      try {
        return JSON.parse(localStorage.getItem(STORAGE_KEY) || "[]");
      } catch {
        return [];
      }
    }

    function saveSubmissions(items) {
      localStorage.setItem(STORAGE_KEY, JSON.stringify(items));
    }

    function renderSubmissions() {
      const items = loadSubmissions();
      submissionsList.innerHTML = "";
      if (!items.length) return;

      items.slice().reverse().forEach((item) => {
        const div = document.createElement("div");
        div.className = "submission-item";
        div.innerHTML = `
          <div class="submission-meta">${escapeHtml(item.name)}${item.group ? " — " + escapeHtml(item.group) : ""}</div>
          <div>${escapeHtml(item.note)}</div>
        `;
        submissionsList.appendChild(div);
      });
    }

    function escapeHtml(str) {
      return str
        .replace(/&/g, "&amp;")
        .replace(/</g, "&lt;")
        .replace(/>/g, "&gt;")
        .replace(/"/g, "&quot;");
    }

    studentForm.addEventListener("submit", (e) => {
      e.preventDefault();
      const name = document.getElementById("studentName").value.trim();
      const group = document.getElementById("studentClass").value.trim();
      const note = document.getElementById("studentNote").value.trim();

      if (!name || !note) return;

      const entry = {
        name,
        group,
        note,
        time: new Date().toLocaleString("ar-SA")
      };

      const items = loadSubmissions();
      items.push(entry);
      saveSubmissions(items);
      renderSubmissions();

      lastSummaryText =
        `الاسم: ${name}\n` +
        (group ? `الصف/المجموعة: ${group}\n` : "") +
        `النشاط: ${ACTIVITY_URL}\n` +
        `المشاركة/الإجابة: ${note}`;

      feedbackBox.style.display = "block";
      feedbackBox.innerHTML =
        `<strong>تم حفظ مشاركتك بنجاح!</strong> يمكنك الآن الضغط على <strong>«نسخ ملخص التسليم»</strong> وإرساله لمعلمك.`;

      studentForm.reset();
    });

    copySummaryBtn.addEventListener("click", async () => {
      if (!lastSummaryText) {
        alert("يرجى تعبئة النموذج والضغط على «حفظ وتوليد ملخص التسليم» أولاً.");
        return;
      }
      try {
        await navigator.clipboard.writeText(lastSummaryText);
        copySummaryBtn.textContent = "تم نسخ الملخص ✓";
        setTimeout(() => {
          copySummaryBtn.textContent = "نسخ ملخص التسليم";
        }, 2000);
      } catch {
        alert(lastSummaryText);
      }
    });

    renderSubmissions();
  </script>
</body>
</html>
