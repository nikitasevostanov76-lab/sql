<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SQL Академия</title>
<style>
  :root {
    --bg: #0f1117;
    --bg2: #1a1d27;
    --bg3: #22263a;
    --card: #1e2235;
    --border: #2e3354;
    --accent: #4f8ef7;
    --accent2: #7c5cfc;
    --green: #22c97a;
    --red: #f75f5f;
    --amber: #f7c948;
    --text: #e8eaf6;
    --muted: #8b90b0;
    --code-bg: #12141f;
    --radius: 12px;
    --radius-sm: 8px;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; }
  html { font-size: 16px; }
  body { background: var(--bg); color: var(--text); font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; line-height: 1.6; min-height: 100vh; }

  /* ---- NAV ---- */
  .nav { position: sticky; top: 0; z-index: 100; background: rgba(15,17,23,0.95); backdrop-filter: blur(10px); border-bottom: 1px solid var(--border); display: flex; align-items: center; gap: 12px; padding: 12px 16px; }
  .nav-logo { font-size: 17px; font-weight: 700; background: linear-gradient(90deg, var(--accent), var(--accent2)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; flex-shrink: 0; }
  .nav-progress-wrap { flex: 1; background: var(--bg3); border-radius: 4px; height: 6px; }
  .nav-progress-bar { height: 6px; border-radius: 4px; background: linear-gradient(90deg, var(--accent), var(--green)); transition: width 0.5s; }
  .nav-pct { font-size: 13px; color: var(--muted); min-width: 36px; text-align: right; }

  /* ---- LAYOUT ---- */
  .shell { display: flex; min-height: calc(100vh - 53px); }
  .sidebar { width: 260px; flex-shrink: 0; border-right: 1px solid var(--border); background: var(--bg2); display: flex; flex-direction: column; position: sticky; top: 53px; height: calc(100vh - 53px); overflow-y: auto; }
  .main { flex: 1; min-width: 0; padding: 0; }

  /* ---- SIDEBAR ---- */
  .sb-section { padding: 16px 12px 8px; font-size: 11px; text-transform: uppercase; letter-spacing: 1px; color: var(--muted); }
  .sb-item { display: flex; align-items: center; gap: 10px; padding: 10px 14px; cursor: pointer; border-radius: var(--radius-sm); margin: 2px 8px; transition: background 0.15s; text-decoration: none; color: inherit; }
  .sb-item:hover { background: var(--bg3); }
  .sb-item.active { background: rgba(79,142,247,0.15); color: var(--accent); }
  .sb-item.done .sb-dot { background: var(--green); }
  .sb-dot { width: 8px; height: 8px; border-radius: 50%; background: var(--border); flex-shrink: 0; transition: background 0.3s; }
  .sb-item.active .sb-dot { background: var(--accent); }
  .sb-label { font-size: 13px; flex: 1; line-height: 1.3; }
  .sb-check { font-size: 11px; color: var(--green); }
  .sb-stats { margin: auto 0 0; padding: 16px; border-top: 1px solid var(--border); display: grid; grid-template-columns: 1fr 1fr; gap: 8px; }
  .sb-stat { background: var(--bg3); border-radius: var(--radius-sm); padding: 10px; text-align: center; }
  .sb-stat-val { font-size: 20px; font-weight: 700; color: var(--accent); }
  .sb-stat-label { font-size: 11px; color: var(--muted); margin-top: 2px; }

  /* ---- PAGES ---- */
  .page { display: none; }
  .page.active { display: block; }

  /* ---- HOME ---- */
  .hero { padding: 48px 40px 32px; max-width: 680px; }
  .hero h1 { font-size: 32px; font-weight: 800; line-height: 1.2; margin-bottom: 12px; background: linear-gradient(135deg, #fff 0%, var(--accent) 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent; }
  .hero p { color: var(--muted); font-size: 16px; margin-bottom: 28px; }
  .hero-cards { display: grid; grid-template-columns: repeat(auto-fit, minmax(160px, 1fr)); gap: 12px; max-width: 640px; margin-bottom: 32px; }
  .hero-card { background: var(--card); border: 1px solid var(--border); border-radius: var(--radius); padding: 18px 16px; }
  .hero-card-icon { font-size: 24px; margin-bottom: 8px; }
  .hero-card-title { font-size: 14px; font-weight: 600; margin-bottom: 4px; }
  .hero-card-sub { font-size: 12px; color: var(--muted); }
  .btn { display: inline-flex; align-items: center; gap: 8px; padding: 12px 24px; border-radius: var(--radius-sm); font-size: 14px; font-weight: 600; cursor: pointer; border: none; transition: all 0.15s; }
  .btn-primary { background: var(--accent); color: #fff; }
  .btn-primary:hover { background: #3a7be8; transform: translateY(-1px); }
  .btn-outline { background: transparent; border: 1px solid var(--border); color: var(--text); }
  .btn-outline:hover { background: var(--bg3); }

  /* ---- MODULE PAGE ---- */
  .module-page { max-width: 720px; padding: 32px 32px 64px; }
  .module-header { margin-bottom: 28px; }
  .module-tag { display: inline-block; background: rgba(79,142,247,0.15); color: var(--accent); font-size: 11px; font-weight: 600; padding: 4px 12px; border-radius: 20px; text-transform: uppercase; letter-spacing: 0.5px; margin-bottom: 12px; }
  .module-title { font-size: 26px; font-weight: 800; margin-bottom: 8px; }
  .module-desc { color: var(--muted); font-size: 15px; }
  .module-meta-row { display: flex; gap: 16px; margin-top: 12px; flex-wrap: wrap; }
  .meta-chip { font-size: 12px; color: var(--muted); display: flex; align-items: center; gap: 5px; }

  /* ---- LECTURE ---- */
  .lecture { margin-bottom: 32px; }
  .lecture h2 { font-size: 20px; font-weight: 700; margin: 28px 0 10px; color: var(--text); }
  .lecture h3 { font-size: 16px; font-weight: 600; margin: 20px 0 8px; color: var(--accent); }
  .lecture p { color: #c5c9e0; font-size: 15px; line-height: 1.75; margin-bottom: 12px; }
  .lecture ul, .lecture ol { padding-left: 20px; margin-bottom: 12px; }
  .lecture li { color: #c5c9e0; font-size: 15px; line-height: 1.75; margin-bottom: 4px; }
  .lecture strong { color: var(--text); font-weight: 600; }
  .tip { background: rgba(79,142,247,0.08); border-left: 3px solid var(--accent); border-radius: 0 var(--radius-sm) var(--radius-sm) 0; padding: 12px 16px; margin: 16px 0; }
  .tip-label { font-size: 11px; font-weight: 700; text-transform: uppercase; letter-spacing: 0.5px; color: var(--accent); margin-bottom: 4px; }
  .tip p { margin: 0; font-size: 14px; color: #c5c9e0; }
  .warn { background: rgba(247,201,72,0.08); border-left: 3px solid var(--amber); border-radius: 0 var(--radius-sm) var(--radius-sm) 0; padding: 12px 16px; margin: 16px 0; }
  .warn .tip-label { color: var(--amber); }
  .warn p { margin: 0; font-size: 14px; color: #c5c9e0; }
  pre { background: var(--code-bg); border: 1px solid var(--border); border-radius: var(--radius-sm); padding: 16px; overflow-x: auto; margin: 12px 0; }
  code { font-family: 'JetBrains Mono', 'Fira Code', monospace; font-size: 13px; color: #a8d8f0; }
  pre code { color: #a8d8f0; }
  .kw { color: #c792ea; }
  .fn { color: #82aaff; }
  .str { color: #c3e88d; }
  .cm { color: #546e7a; font-style: italic; }
  .num { color: #f78c6c; }
  .table-demo { width: 100%; border-collapse: collapse; margin: 16px 0; font-size: 13px; }
  .table-demo th { background: var(--bg3); color: var(--muted); text-align: left; padding: 8px 12px; font-weight: 600; border: 1px solid var(--border); }
  .table-demo td { padding: 8px 12px; border: 1px solid var(--border); color: #c5c9e0; }
  .table-demo tr:nth-child(even) td { background: rgba(255,255,255,0.02); }

  /* ---- CHECKLIST ---- */
  .checklist { margin: 24px 0; display: flex; flex-direction: column; gap: 8px; }
  .check-item { display: flex; align-items: flex-start; gap: 12px; background: var(--card); border: 1px solid var(--border); border-radius: var(--radius-sm); padding: 12px 14px; cursor: pointer; transition: all 0.15s; user-select: none; }
  .check-item:hover { border-color: var(--accent); }
  .check-item.checked { background: rgba(34,201,122,0.07); border-color: rgba(34,201,122,0.3); }
  .check-box { width: 20px; height: 20px; border-radius: 50%; border: 2px solid var(--border); flex-shrink: 0; margin-top: 1px; display: flex; align-items: center; justify-content: center; font-size: 11px; transition: all 0.2s; }
  .check-item.checked .check-box { background: var(--green); border-color: var(--green); color: #fff; }
  .check-text { flex: 1; }
  .check-title { font-size: 14px; font-weight: 600; }
  .check-sub { font-size: 12px; color: var(--muted); margin-top: 2px; }

  /* ---- QUIZ ---- */
  .quiz-section { background: var(--card); border: 1px solid var(--border); border-radius: var(--radius); padding: 24px; margin-top: 32px; }
  .quiz-header { display: flex; align-items: center; justify-content: space-between; margin-bottom: 20px; }
  .quiz-title { font-size: 16px; font-weight: 700; }
  .quiz-counter { font-size: 13px; color: var(--muted); }
  .quiz-q { font-size: 15px; font-weight: 600; margin-bottom: 12px; line-height: 1.5; }
  .quiz-code { background: var(--code-bg); border: 1px solid var(--border); border-radius: var(--radius-sm); padding: 14px; font-family: monospace; font-size: 13px; color: #a8d8f0; margin-bottom: 14px; overflow-x: auto; white-space: pre; }
  .quiz-opts { display: flex; flex-direction: column; gap: 8px; }
  .quiz-opt { padding: 12px 16px; border: 1px solid var(--border); border-radius: var(--radius-sm); font-size: 14px; cursor: pointer; background: var(--bg3); color: var(--text); text-align: left; transition: all 0.15s; }
  .quiz-opt:hover:not(:disabled) { border-color: var(--accent); background: rgba(79,142,247,0.1); }
  .quiz-opt.correct { background: rgba(34,201,122,0.12); border-color: var(--green); color: var(--green); }
  .quiz-opt.wrong { background: rgba(247,95,95,0.12); border-color: var(--red); color: var(--red); }
  .quiz-opt:disabled { cursor: default; }
  .quiz-feedback { margin-top: 14px; padding: 12px 16px; border-radius: var(--radius-sm); font-size: 14px; display: none; }
  .quiz-feedback.ok { background: rgba(34,201,122,0.1); color: #5de8a0; border: 1px solid rgba(34,201,122,0.2); display: block; }
  .quiz-feedback.bad { background: rgba(247,95,95,0.1); color: #f97f7f; border: 1px solid rgba(247,95,95,0.2); display: block; }
  .quiz-nav { display: flex; align-items: center; justify-content: space-between; margin-top: 16px; }
  .quiz-result { text-align: center; padding: 20px 0; }
  .quiz-result-score { font-size: 40px; font-weight: 800; margin-bottom: 8px; }
  .quiz-result-sub { color: var(--muted); font-size: 14px; margin-bottom: 20px; }

  /* ---- DIVIDER ---- */
  .divider { height: 1px; background: var(--border); margin: 32px 0; }

  /* ---- MOBILE ---- */
  .mob-nav { display: none; position: fixed; bottom: 0; left: 0; right: 0; background: var(--bg2); border-top: 1px solid var(--border); z-index: 200; padding: 8px 0 max(8px, env(safe-area-inset-bottom)); }
  .mob-nav-inner { display: flex; justify-content: space-around; }
  .mob-btn { display: flex; flex-direction: column; align-items: center; gap: 3px; background: none; border: none; color: var(--muted); font-size: 10px; cursor: pointer; padding: 4px 12px; }
  .mob-btn.active { color: var(--accent); }
  .mob-btn-icon { font-size: 20px; }

  @media (max-width: 700px) {
    .sidebar { display: none; }
    .hero { padding: 24px 16px 20px; }
    .hero h1 { font-size: 24px; }
    .module-page { padding: 20px 16px 100px; }
    .mob-nav { display: block; }
    .quiz-section { padding: 16px; }
  }
</style>
</head>
<body>

<nav class="nav">
  <div class="nav-logo">SQL Academy</div>
  <div class="nav-progress-wrap"><div class="nav-progress-bar" id="navBar" style="width:0%"></div></div>
  <div class="nav-pct" id="navPct">0%</div>
</nav>

<div class="shell">
  <!-- SIDEBAR -->
  <aside class="sidebar" id="sidebar">
    <div class="sb-section">Модули</div>
    <a class="sb-item active" onclick="showPage('home')" href="#">
      <div class="sb-dot" style="background:var(--accent2)"></div>
      <span class="sb-label">🏠 Главная</span>
    </a>
    <div id="sbModules"></div>
    <div class="sb-stats">
      <div class="sb-stat"><div class="sb-stat-val" id="stTopics">0</div><div class="sb-stat-label">Тем</div></div>
      <div class="sb-stat"><div class="sb-stat-val" id="stQuiz">0%</div><div class="sb-stat-label">Тесты</div></div>
    </div>
  </aside>

  <!-- MAIN -->
  <main class="main">
    <!-- HOME -->
    <div class="page active" id="page-home">
      <div class="hero">
        <h1>SQL с нуля до уверенного уровня</h1>
        <p>Лекции, примеры, интерактивные тесты. Открывай с любого устройства — прогресс сохраняется.</p>
        <div class="hero-cards">
          <div class="hero-card"><div class="hero-card-icon">📖</div><div class="hero-card-title">6 модулей</div><div class="hero-card-sub">От SELECT до оконных функций</div></div>
          <div class="hero-card"><div class="hero-card-icon">✅</div><div class="hero-card-title">30 тем</div><div class="hero-card-sub">С чеклистом прогресса</div></div>
          <div class="hero-card"><div class="hero-card-icon">🧪</div><div class="hero-card-title">12 тестов</div><div class="hero-card-sub">С разбором ответов</div></div>
          <div class="hero-card"><div class="hero-card-icon">📱</div><div class="hero-card-title">Mobile</div><div class="hero-card-sub">Работает на телефоне</div></div>
        </div>
        <button class="btn btn-primary" onclick="showPage('m0')">Начать с модуля 1 →</button>
      </div>
    </div>

    <!-- MODULE PAGES will be injected here -->
    <div id="modulePages"></div>
  </main>
</div>

<!-- MOBILE BOTTOM NAV -->
<div class="mob-nav">
  <div class="mob-nav-inner">
    <button class="mob-btn active" id="mob-home" onclick="showPage('home')"><span class="mob-btn-icon">🏠</span>Главная</button>
    <button class="mob-btn" id="mob-modules" onclick="showMobModules()"><span class="mob-btn-icon">📚</span>Модули</button>
    <button class="mob-btn" id="mob-progress" onclick="showPage('progress')"><span class="mob-btn-icon">📊</span>Прогресс</button>
  </div>
</div>

<script>
// ============================================================
// DATA
// ============================================================
const MODULES = [
{
  title: "Основы SQL и SELECT",
  tag: "Модуль 1",
  desc: "Что такое реляционная база данных, как выбирать данные, фильтровать и сортировать.",
  time: "3–4 дня",
  topics: [
    { title: "Реляционная БД и таблицы", sub: "Строки, столбцы, первичный ключ" },
    { title: "SELECT: выборка данных", sub: "SELECT *, SELECT col1, col2" },
    { title: "WHERE: фильтрация строк", sub: "=, !=, >, <, BETWEEN, IN, LIKE" },
    { title: "ORDER BY и LIMIT", sub: "Сортировка и ограничение результата" },
    { title: "NULL и IS NULL", sub: "Работа с пустыми значениями" },
  ],
  lecture: `
<h2>Что такое реляционная база данных?</h2>
<p>База данных — это организованное хранилище данных. <strong>Реляционная</strong> база хранит данные в виде таблиц, связанных между собой. Каждая таблица — это как лист Excel: строки (записи) и столбцы (поля).</p>
<p>Например, таблица <strong>users</strong>:</p>
<table class="table-demo"><thead><tr><th>id</th><th>name</th><th>age</th><th>city</th></tr></thead><tbody>
<tr><td>1</td><td>Алёша</td><td>25</td><td>Москва</td></tr>
<tr><td>2</td><td>Маша</td><td>30</td><td>Питер</td></tr>
<tr><td>3</td><td>Игорь</td><td>22</td><td>Москва</td></tr>
</tbody></table>
<p><strong>id</strong> — это первичный ключ (PRIMARY KEY): уникальный идентификатор каждой строки.</p>
<div class="tip"><div class="tip-label">💡 Аналогия</div><p>Таблица = Excel-лист. База данных = Excel-книга с несколькими листами, связанными друг с другом.</p></div>

<h2>SELECT — выборка данных</h2>
<p>Основная команда SQL. Синтаксис:</p>
<pre><code><span class="kw">SELECT</span> * <span class="kw">FROM</span> users;           <span class="cm">-- все столбцы, все строки</span>
<span class="kw">SELECT</span> name, age <span class="kw">FROM</span> users;   <span class="cm">-- только name и age</span>
<span class="kw">SELECT</span> name <span class="kw">AS</span> имя <span class="kw">FROM</span> users; <span class="cm">-- переименовать столбец</span></code></pre>
<div class="warn"><div class="tip-label">⚠️ Привычка</div><p>Не пиши SELECT * в продакшене — это медленно и читается хуже. Всегда указывай нужные столбцы.</p></div>

<h2>WHERE — фильтрация</h2>
<p>WHERE отбирает строки по условию. Операторы:</p>
<pre><code><span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> age > <span class="num">18</span>;
<span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> city = <span class="str">'Москва'</span>;
<span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> age <span class="kw">BETWEEN</span> <span class="num">20</span> <span class="kw">AND</span> <span class="num">30</span>;
<span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> city <span class="kw">IN</span> (<span class="str">'Москва'</span>, <span class="str">'Питер'</span>);
<span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> name <span class="kw">LIKE</span> <span class="str">'А%'</span>; <span class="cm">-- начинается на А</span>
<span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> name <span class="kw">LIKE</span> <span class="str">'%ов'</span>; <span class="cm">-- заканчивается на ов</span></code></pre>
<p>Комбинируй условия через <strong>AND</strong> / <strong>OR</strong> / <strong>NOT</strong>:</p>
<pre><code><span class="kw">SELECT</span> * <span class="kw">FROM</span> users
<span class="kw">WHERE</span> age > <span class="num">18</span> <span class="kw">AND</span> city = <span class="str">'Москва'</span>;</code></pre>

<h2>ORDER BY и LIMIT</h2>
<pre><code><span class="kw">SELECT</span> name, age <span class="kw">FROM</span> users <span class="kw">ORDER BY</span> age;           <span class="cm">-- ASC по умолчанию</span>
<span class="kw">SELECT</span> name, age <span class="kw">FROM</span> users <span class="kw">ORDER BY</span> age <span class="kw">DESC</span>;      <span class="cm">-- от большего</span>
<span class="kw">SELECT</span> name, age <span class="kw">FROM</span> users <span class="kw">ORDER BY</span> age <span class="kw">DESC LIMIT</span> <span class="num">5</span>; <span class="cm">-- топ-5</span></code></pre>

<h2>NULL — пустое значение</h2>
<p><strong>NULL</strong> — это не 0 и не пустая строка. Это отсутствие значения. Сравнивать NULL через = нельзя!</p>
<pre><code><span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> phone <span class="kw">IS NULL</span>;     <span class="cm">-- нет телефона</span>
<span class="kw">SELECT</span> * <span class="kw">FROM</span> users <span class="kw">WHERE</span> phone <span class="kw">IS NOT NULL</span>; <span class="cm">-- есть телефон</span>
<span class="cm">-- WRONG: WHERE phone = NULL  (всегда пусто!)</span></code></pre>
`,
  quizzes: [
    { q: "Какой запрос вернёт пользователей из Москвы старше 25 лет?", code: null,
      opts: ["SELECT * FROM users WHERE city = 'Москва' AND age > 25", "SELECT * FROM users WHERE city = 'Москва' OR age > 25", "SELECT * FROM users IF city = 'Москва' AND age > 25", "FILTER users WHERE city = 'Москва' AND age > 25"],
      correct: 0, explain: "AND объединяет оба условия — оба должны быть истинны. OR подойдёт, если достаточно выполнения хотя бы одного." },
    { q: "Что вернёт этот запрос?", code: "SELECT name FROM users\nORDER BY age DESC\nLIMIT 3;",
      opts: ["3 самых молодых пользователя", "3 самых старших пользователя", "Всех пользователей, отсортированных по имени", "Ошибку"],
      correct: 1, explain: "DESC — по убыванию (от большего к меньшему). LIMIT 3 берёт первые 3 строки результата — то есть 3 самых старших." },
  ]
},
{
  title: "Агрегация и GROUP BY",
  tag: "Модуль 2",
  desc: "Считаем суммы, средние, группируем данные. Это 80% аналитических запросов.",
  time: "3–4 дня",
  topics: [
    { title: "COUNT, SUM, AVG, MIN, MAX", sub: "Агрегатные функции" },
    { title: "GROUP BY: группировка", sub: "Что можно в SELECT при GROUP BY" },
    { title: "HAVING: фильтр по группам", sub: "Отличие от WHERE" },
    { title: "DISTINCT: уникальные значения", sub: "COUNT(DISTINCT col)" },
    { title: "ROUND и другие функции", sub: "Форматирование чисел" },
  ],
  lecture: `
<h2>Агрегатные функции</h2>
<p>Агрегатные функции сворачивают много строк в одно число:</p>
<pre><code><span class="kw">SELECT</span>
  <span class="fn">COUNT</span>(*),          <span class="cm">-- количество строк</span>
  <span class="fn">COUNT</span>(phone),      <span class="cm">-- строки, где phone IS NOT NULL</span>
  <span class="fn">SUM</span>(amount),       <span class="cm">-- сумма</span>
  <span class="fn">AVG</span>(age),          <span class="cm">-- среднее</span>
  <span class="fn">MIN</span>(price),        <span class="cm">-- минимум</span>
  <span class="fn">MAX</span>(price)         <span class="cm">-- максимум</span>
<span class="kw">FROM</span> orders;</code></pre>

<h2>GROUP BY — группировка</h2>
<p>GROUP BY разбивает строки на группы и применяет агрегацию к каждой группе.</p>
<pre><code><span class="cm">-- Количество пользователей по городам:</span>
<span class="kw">SELECT</span> city, <span class="fn">COUNT</span>(*) <span class="kw">AS</span> cnt
<span class="kw">FROM</span> users
<span class="kw">GROUP BY</span> city;</code></pre>
<table class="table-demo"><thead><tr><th>city</th><th>cnt</th></tr></thead><tbody>
<tr><td>Москва</td><td>3</td></tr>
<tr><td>Питер</td><td>2</td></tr>
</tbody></table>
<div class="warn"><div class="tip-label">⚠️ Правило GROUP BY</div><p>В SELECT при GROUP BY можно писать только: (1) столбцы из GROUP BY, (2) агрегатные функции. Всё остальное — ошибка.</p></div>
<pre><code><span class="cm">-- OK:</span>
<span class="kw">SELECT</span> city, <span class="fn">COUNT</span>(*), <span class="fn">AVG</span>(age) <span class="kw">FROM</span> users <span class="kw">GROUP BY</span> city;
<span class="cm">-- ОШИБКА — name не в GROUP BY:</span>
<span class="kw">SELECT</span> city, name, <span class="fn">COUNT</span>(*) <span class="kw">FROM</span> users <span class="kw">GROUP BY</span> city;</code></pre>

<h2>HAVING — фильтр после группировки</h2>
<pre><code><span class="cm">-- Города, где больше 5 пользователей:</span>
<span class="kw">SELECT</span> city, <span class="fn">COUNT</span>(*) <span class="kw">AS</span> cnt
<span class="kw">FROM</span> users
<span class="kw">GROUP BY</span> city
<span class="kw">HAVING</span> <span class="fn">COUNT</span>(*) > <span class="num">5</span>;</code></pre>
<div class="tip"><div class="tip-label">💡 WHERE vs HAVING</div><p><strong>WHERE</strong> — до группировки, фильтрует строки. <strong>HAVING</strong> — после, фильтрует группы. Можно использовать оба вместе.</p></div>
<pre><code><span class="kw">SELECT</span> city, <span class="fn">COUNT</span>(*) <span class="kw">AS</span> cnt
<span class="kw">FROM</span> users
<span class="kw">WHERE</span> age > <span class="num">18</span>            <span class="cm">-- сначала отбросим несовершеннолетних</span>
<span class="kw">GROUP BY</span> city
<span class="kw">HAVING</span> <span class="fn">COUNT</span>(*) > <span class="num">3</span>;      <span class="cm">-- затем — только крупные города</span></code></pre>

<h2>DISTINCT — уникальные значения</h2>
<pre><code><span class="kw">SELECT DISTINCT</span> city <span class="kw">FROM</span> users;         <span class="cm">-- уникальные города</span>
<span class="kw">SELECT</span> <span class="fn">COUNT</span>(<span class="kw">DISTINCT</span> city) <span class="kw">FROM</span> users;  <span class="cm">-- сколько уникальных</span></code></pre>
`,
  quizzes: [
    { q: "В чём разница WHERE и HAVING?", code: null,
      opts: ["WHERE работает после GROUP BY, HAVING — до", "WHERE фильтрует строки до группировки, HAVING — группы после", "Они взаимозаменяемы", "HAVING работает только с COUNT"],
      correct: 1, explain: "WHERE отбирает строки ДО того, как GROUP BY их сгруппирует. HAVING фильтрует уже готовые группы — поэтому в нём можно использовать агрегатные функции." },
    { q: "Что вернёт запрос?", code: "SELECT department, AVG(salary) as avg_sal\nFROM employees\nGROUP BY department\nHAVING AVG(salary) > 80000;",
      opts: ["Всех сотрудников с зарплатой > 80000", "Отделы, где средняя зарплата выше 80000", "Отделы с хотя бы одним сотрудником с з/п > 80000", "Ошибку — нельзя AVG в HAVING"],
      correct: 1, explain: "HAVING AVG(salary) > 80000 фильтрует группы (отделы) по средней зарплате внутри группы. Это классический паттерн: GROUP BY → HAVING с агрегатом." },
  ]
},
{
  title: "JOIN: объединение таблиц",
  tag: "Модуль 3",
  desc: "Ключевая тема. Без JOIN нельзя работать с реальными данными — они всегда в нескольких таблицах.",
  time: "4–5 дней",
  topics: [
    { title: "INNER JOIN", sub: "Только совпадающие строки" },
    { title: "LEFT JOIN / RIGHT JOIN", sub: "Все строки + совпадения" },
    { title: "FULL OUTER JOIN", sub: "Все строки из обеих таблиц" },
    { title: "JOIN трёх и более таблиц", sub: "Цепочка соединений" },
    { title: "Алиасы и читаемость", sub: "Таблица AS t, столбец AS col" },
  ],
  lecture: `
<h2>Зачем нужен JOIN?</h2>
<p>Данные обычно хранятся в разных таблицах. Заказы — в одной, клиенты — в другой. JOIN позволяет их соединить.</p>
<table class="table-demo"><thead><tr><th>orders.id</th><th>orders.client_id</th><th>orders.amount</th></tr></thead><tbody>
<tr><td>1</td><td>10</td><td>500</td></tr><tr><td>2</td><td>11</td><td>200</td></tr><tr><td>3</td><td>99</td><td>800</td></tr>
</tbody></table>
<table class="table-demo"><thead><tr><th>clients.id</th><th>clients.name</th></tr></thead><tbody>
<tr><td>10</td><td>Алёша</td></tr><tr><td>11</td><td>Маша</td></tr>
</tbody></table>

<h2>INNER JOIN — только совпадения</h2>
<pre><code><span class="kw">SELECT</span> o.id, c.name, o.amount
<span class="kw">FROM</span> orders o
<span class="kw">INNER JOIN</span> clients c <span class="kw">ON</span> o.client_id = c.id;</code></pre>
<p>Результат: только строки, где client_id нашёлся в обеих таблицах. Заказ #3 (client_id=99) выпадет — такого клиента нет.</p>
<table class="table-demo"><thead><tr><th>id</th><th>name</th><th>amount</th></tr></thead><tbody>
<tr><td>1</td><td>Алёша</td><td>500</td></tr><tr><td>2</td><td>Маша</td><td>200</td></tr>
</tbody></table>

<h2>LEFT JOIN — все строки из левой таблицы</h2>
<pre><code><span class="kw">SELECT</span> o.id, c.name, o.amount
<span class="kw">FROM</span> orders o
<span class="kw">LEFT JOIN</span> clients c <span class="kw">ON</span> o.client_id = c.id;</code></pre>
<p>Теперь заказ #3 тоже попадает — просто с NULL в name:</p>
<table class="table-demo"><thead><tr><th>id</th><th>name</th><th>amount</th></tr></thead><tbody>
<tr><td>1</td><td>Алёша</td><td>500</td></tr><tr><td>2</td><td>Маша</td><td>200</td></tr><tr><td>3</td><td>NULL</td><td>800</td></tr>
</tbody></table>
<div class="tip"><div class="tip-label">💡 Лайфхак</div><p>LEFT JOIN + WHERE right.id IS NULL — найти строки в левой таблице, которых НЕТ в правой. Например, клиенты без заказов.</p></div>
<pre><code><span class="cm">-- Клиенты, которые ни разу не заказывали:</span>
<span class="kw">SELECT</span> c.name
<span class="kw">FROM</span> clients c
<span class="kw">LEFT JOIN</span> orders o <span class="kw">ON</span> c.id = o.client_id
<span class="kw">WHERE</span> o.id <span class="kw">IS NULL</span>;</code></pre>

<h2>JOIN трёх таблиц</h2>
<pre><code><span class="kw">SELECT</span> o.id, c.name, p.title
<span class="kw">FROM</span> orders o
<span class="kw">JOIN</span> clients c <span class="kw">ON</span> o.client_id = c.id
<span class="kw">JOIN</span> products p <span class="kw">ON</span> o.product_id = p.id;</code></pre>
<p>Каждый новый JOIN добавляет ещё одну таблицу. Читай слева направо: начни с orders, присоедини clients, потом products.</p>
`,
  quizzes: [
    { q: "Какой JOIN вернёт ВСЕ заказы, даже если клиент не найден в таблице clients?", code: "SELECT o.id, c.name\nFROM orders o\n[???] JOIN clients c ON o.client_id = c.id",
      opts: ["INNER JOIN", "LEFT JOIN", "RIGHT JOIN", "CROSS JOIN"],
      correct: 1, explain: "LEFT JOIN берёт ВСЕ строки из левой таблицы (orders) и добавляет совпадения из правой. Нет совпадения — c.name будет NULL, но строка всё равно попадёт." },
    { q: "Сколько строк вернёт INNER JOIN, если orders — 5 строк, clients — 3, из них совпадают только 2 пары?", code: null,
      opts: ["2", "5", "3", "8"],
      correct: 0, explain: "INNER JOIN — это пересечение. Только совпадающие пары. Если их 2 — вернётся ровно 2 строки." },
  ]
},
{
  title: "Подзапросы и CTE",
  tag: "Модуль 4",
  desc: "Как писать запросы внутри запросов и почему CTE делает код читаемым.",
  time: "4 дня",
  topics: [
    { title: "Подзапросы в WHERE", sub: "IN, EXISTS, скалярное сравнение" },
    { title: "Подзапросы в FROM", sub: "Derived table — подзапрос как таблица" },
    { title: "Коррелированные подзапросы", sub: "Зависят от внешнего запроса" },
    { title: "WITH (CTE)", sub: "Именованный временный результат" },
    { title: "Несколько CTE цепочкой", sub: "WITH a AS (...), b AS (...)" },
  ],
  lecture: `
<h2>Подзапросы в WHERE</h2>
<p>Подзапрос — это запрос внутри запроса. Самое частое применение — IN и EXISTS.</p>
<pre><code><span class="cm">-- Пользователи, которые сделали хотя бы один заказ:</span>
<span class="kw">SELECT</span> name <span class="kw">FROM</span> users
<span class="kw">WHERE</span> id <span class="kw">IN</span> (
  <span class="kw">SELECT</span> user_id <span class="kw">FROM</span> orders
);</code></pre>
<pre><code><span class="cm">-- То же самое через EXISTS (быстрее на больших таблицах):</span>
<span class="kw">SELECT</span> name <span class="kw">FROM</span> users u
<span class="kw">WHERE EXISTS</span> (
  <span class="kw">SELECT</span> <span class="num">1</span> <span class="kw">FROM</span> orders o
  <span class="kw">WHERE</span> o.user_id = u.id
);</code></pre>
<div class="tip"><div class="tip-label">💡 SELECT 1</div><p>В EXISTS пишут SELECT 1 — важен сам факт наличия строк, а не их содержимое. Это стандартная практика.</p></div>

<h2>Подзапрос в FROM (Derived Table)</h2>
<pre><code><span class="cm">-- Средний размер заказа по клиентам:</span>
<span class="kw">SELECT</span> <span class="fn">AVG</span>(total) <span class="kw">FROM</span> (
  <span class="kw">SELECT</span> user_id, <span class="fn">SUM</span>(amount) <span class="kw">AS</span> total
  <span class="kw">FROM</span> orders
  <span class="kw">GROUP BY</span> user_id
) <span class="kw">AS</span> user_totals;</code></pre>

<h2>CTE — читаемый способ писать подзапросы</h2>
<p>CTE (Common Table Expression) — именованный блок, который работает как временная таблица для текущего запроса.</p>
<pre><code><span class="kw">WITH</span> high_value_users <span class="kw">AS</span> (
  <span class="kw">SELECT</span> user_id, <span class="fn">SUM</span>(amount) <span class="kw">AS</span> total
  <span class="kw">FROM</span> orders
  <span class="kw">GROUP BY</span> user_id
  <span class="kw">HAVING</span> <span class="fn">SUM</span>(amount) > <span class="num">10000</span>
)
<span class="kw">SELECT</span> u.name, hvu.total
<span class="kw">FROM</span> users u
<span class="kw">JOIN</span> high_value_users hvu <span class="kw">ON</span> u.id = hvu.user_id;</code></pre>

<h2>Несколько CTE</h2>
<pre><code><span class="kw">WITH</span>
orders_agg <span class="kw">AS</span> (
  <span class="kw">SELECT</span> user_id, <span class="fn">COUNT</span>(*) <span class="kw">AS</span> cnt, <span class="fn">SUM</span>(amount) <span class="kw">AS</span> total
  <span class="kw">FROM</span> orders <span class="kw">GROUP BY</span> user_id
),
active_users <span class="kw">AS</span> (
  <span class="kw">SELECT</span> * <span class="kw">FROM</span> orders_agg <span class="kw">WHERE</span> cnt > <span class="num">5</span>
)
<span class="kw">SELECT</span> u.name, au.total
<span class="kw">FROM</span> users u
<span class="kw">JOIN</span> active_users au <span class="kw">ON</span> u.id = au.user_id;</code></pre>
<div class="tip"><div class="tip-label">💡 Когда CTE vs подзапрос?</div><p>CTE лучше, когда: (1) результат нужен несколько раз, (2) запрос сложный и нужна читаемость, (3) хочется дать смысловое имя промежуточному результату.</p></div>
`,
  quizzes: [
    { q: "Зачем использовать CTE вместо подзапроса?", code: null,
      opts: ["CTE всегда быстрее", "CTE делает запрос читаемее и позволяет переиспользовать результат", "Подзапросы не поддерживают JOIN", "CTE только в PostgreSQL"],
      correct: 1, explain: "CTE улучшает читаемость и позволяет дать промежуточному результату имя. По скорости — зависит от СУБД, часто одинаково." },
    { q: "Что вернёт EXISTS в этом запросе?", code: "SELECT name FROM users u\nWHERE EXISTS (\n  SELECT 1 FROM orders o\n  WHERE o.user_id = u.id\n);",
      opts: ["Пользователей без заказов", "Пользователей, у которых есть хотя бы один заказ", "Количество заказов", "Ошибку"],
      correct: 1, explain: "EXISTS = TRUE если подзапрос вернул хотя бы одну строку. Здесь: существует ли заказ для этого пользователя? Если да — берём его в результат." },
  ]
},
{
  title: "Оконные функции",
  tag: "Модуль 5",
  desc: "Самый мощный инструмент SQL. Ранги, накопительные суммы, сравнение с предыдущим периодом.",
  time: "4–5 дней",
  topics: [
    { title: "OVER(): синтаксис окна", sub: "PARTITION BY, ORDER BY внутри OVER" },
    { title: "ROW_NUMBER, RANK, DENSE_RANK", sub: "Нумерация и ранжирование" },
    { title: "LAG и LEAD", sub: "Доступ к соседним строкам" },
    { title: "SUM OVER — накопительный итог", sub: "Бегущая сумма" },
    { title: "NTILE и PERCENT_RANK", sub: "Квантили и перцентили" },
  ],
  lecture: `
<h2>Что такое оконная функция?</h2>
<p>Оконная функция выполняет вычисление над набором строк, <strong>не сворачивая их в одну</strong> (в отличие от GROUP BY). Каждая строка остаётся в результате.</p>
<pre><code><span class="fn">функция</span>() <span class="kw">OVER</span> (
  <span class="kw">PARTITION BY</span> столбец   <span class="cm">-- разбить на группы (необязательно)</span>
  <span class="kw">ORDER BY</span> столбец        <span class="cm">-- порядок внутри окна (необязательно)</span>
)</code></pre>

<h2>ROW_NUMBER, RANK, DENSE_RANK</h2>
<pre><code><span class="kw">SELECT</span>
  name,
  department,
  salary,
  <span class="fn">ROW_NUMBER</span>() <span class="kw">OVER</span> (<span class="kw">PARTITION BY</span> department <span class="kw">ORDER BY</span> salary <span class="kw">DESC</span>) <span class="kw">AS</span> rn,
  <span class="fn">RANK</span>()       <span class="kw">OVER</span> (<span class="kw">PARTITION BY</span> department <span class="kw">ORDER BY</span> salary <span class="kw">DESC</span>) <span class="kw">AS</span> rnk,
  <span class="fn">DENSE_RANK</span>() <span class="kw">OVER</span> (<span class="kw">PARTITION BY</span> department <span class="kw">ORDER BY</span> salary <span class="kw">DESC</span>) <span class="kw">AS</span> drnk
<span class="kw">FROM</span> employees;</code></pre>
<table class="table-demo"><thead><tr><th>name</th><th>salary</th><th>ROW_NUMBER</th><th>RANK</th><th>DENSE_RANK</th></tr></thead><tbody>
<tr><td>Алёша</td><td>100</td><td>1</td><td>1</td><td>1</td></tr>
<tr><td>Маша</td><td>90</td><td>2</td><td>2</td><td>2</td></tr>
<tr><td>Игорь</td><td>90</td><td>3</td><td>2</td><td>2</td></tr>
<tr><td>Петя</td><td>80</td><td>4</td><td>4</td><td>3</td></tr>
</tbody></table>
<div class="tip"><div class="tip-label">💡 Разница</div><p>RANK пропускает номера после ничьей (2, 2, 4). DENSE_RANK — нет (2, 2, 3). ROW_NUMBER всегда уникален.</p></div>

<h2>Топ-N внутри группы (частая задача)</h2>
<pre><code><span class="cm">-- Топ-2 сотрудника по зарплате в каждом отделе:</span>
<span class="kw">WITH</span> ranked <span class="kw">AS</span> (
  <span class="kw">SELECT</span> *, <span class="fn">ROW_NUMBER</span>() <span class="kw">OVER</span> (
    <span class="kw">PARTITION BY</span> department
    <span class="kw">ORDER BY</span> salary <span class="kw">DESC</span>
  ) <span class="kw">AS</span> rn
  <span class="kw">FROM</span> employees
)
<span class="kw">SELECT</span> * <span class="kw">FROM</span> ranked <span class="kw">WHERE</span> rn <= <span class="num">2</span>;</code></pre>

<h2>LAG и LEAD — соседние строки</h2>
<pre><code><span class="cm">-- Сравнить продажи с предыдущим месяцем:</span>
<span class="kw">SELECT</span>
  month,
  revenue,
  <span class="fn">LAG</span>(revenue) <span class="kw">OVER</span> (<span class="kw">ORDER BY</span> month) <span class="kw">AS</span> prev_month,
  revenue - <span class="fn">LAG</span>(revenue) <span class="kw">OVER</span> (<span class="kw">ORDER BY</span> month) <span class="kw">AS</span> diff
<span class="kw">FROM</span> monthly_sales;</code></pre>

<h2>Накопительная сумма</h2>
<pre><code><span class="kw">SELECT</span>
  date,
  amount,
  <span class="fn">SUM</span>(amount) <span class="kw">OVER</span> (<span class="kw">ORDER BY</span> date) <span class="kw">AS</span> running_total
<span class="kw">FROM</span> payments;</code></pre>
`,
  quizzes: [
    { q: "Что вернёт ROW_NUMBER() OVER(PARTITION BY dept ORDER BY salary DESC)?", code: null,
      opts: ["Номер строки по всей таблице", "Порядковый номер сотрудника внутри его отдела от большей зарплаты", "Ранг отдела", "Количество сотрудников в отделе"],
      correct: 1, explain: "PARTITION BY dept = отдельное окно для каждого отдела. ORDER BY salary DESC = нумерация от большей зарплаты. Итог: 1-й — самый высокооплачиваемый в своём отделе." },
    { q: "В чём разница RANK и DENSE_RANK для зарплат 100, 90, 90, 80?", code: null,
      opts: ["Нет разницы", "RANK: 1,2,2,4 | DENSE_RANK: 1,2,2,3", "RANK: 1,2,3,4 | DENSE_RANK: 1,2,2,4", "DENSE_RANK пропускает дубли"],
      correct: 1, explain: "RANK пропускает номера после ничьей: два 2-х места — следующий 4-й. DENSE_RANK не пропускает: два 2-х — следующий 3-й." },
  ]
},
{
  title: "Практика: задачи среднего уровня",
  tag: "Модуль 6",
  desc: "Собираем всё вместе. Реальные паттерны, которые встречаются на практике и на собеседованиях.",
  time: "5–7 дней",
  topics: [
    { title: "CASE WHEN — условная логика", sub: "Категоризация, флаги, pivot" },
    { title: "Self JOIN — самосоединение", sub: "Сотрудник и менеджер в одной таблице" },
    { title: "Поиск дубликатов", sub: "GROUP BY + HAVING, ROW_NUMBER" },
    { title: "Топ-N по группам", sub: "Классическая задача с оконными функциями" },
    { title: "Когортный анализ", sub: "CTE + оконные функции" },
  ],
  lecture: `
<h2>CASE WHEN — условный столбец</h2>
<pre><code><span class="kw">SELECT</span> name,
  <span class="kw">CASE</span>
    <span class="kw">WHEN</span> age < <span class="num">18</span> <span class="kw">THEN</span> <span class="str">'junior'</span>
    <span class="kw">WHEN</span> age < <span class="num">60</span> <span class="kw">THEN</span> <span class="str">'adult'</span>
    <span class="kw">ELSE</span> <span class="str">'senior'</span>
  <span class="kw">END</span> <span class="kw">AS</span> age_group
<span class="kw">FROM</span> users;</code></pre>
<p>CASE WHEN — это не фильтр. Он создаёт новый вычисляемый столбец для каждой строки.</p>
<pre><code><span class="cm">-- Pivot-like: подсчёт по категориям в одну строку</span>
<span class="kw">SELECT</span>
  <span class="fn">SUM</span>(<span class="kw">CASE WHEN</span> status = <span class="str">'paid'</span> <span class="kw">THEN</span> <span class="num">1</span> <span class="kw">ELSE</span> <span class="num">0</span> <span class="kw">END</span>) <span class="kw">AS</span> paid_cnt,
  <span class="fn">SUM</span>(<span class="kw">CASE WHEN</span> status = <span class="str">'pending'</span> <span class="kw">THEN</span> <span class="num">1</span> <span class="kw">ELSE</span> <span class="num">0</span> <span class="kw">END</span>) <span class="kw">AS</span> pending_cnt
<span class="kw">FROM</span> orders;</code></pre>

<h2>Self JOIN — таблица с собой</h2>
<pre><code><span class="cm">-- employees: id, name, manager_id</span>
<span class="kw">SELECT</span>
  e.name <span class="kw">AS</span> employee,
  m.name <span class="kw">AS</span> manager
<span class="kw">FROM</span> employees e
<span class="kw">LEFT JOIN</span> employees m <span class="kw">ON</span> e.manager_id = m.id;</code></pre>

<h2>Поиск дубликатов</h2>
<pre><code><span class="cm">-- Метод 1: GROUP BY + HAVING</span>
<span class="kw">SELECT</span> email, <span class="fn">COUNT</span>(*) <span class="kw">AS</span> cnt
<span class="kw">FROM</span> users
<span class="kw">GROUP BY</span> email
<span class="kw">HAVING</span> <span class="fn">COUNT</span>(*) > <span class="num">1</span>;</code></pre>
<pre><code><span class="cm">-- Метод 2: ROW_NUMBER (чтобы удалить дубликаты)</span>
<span class="kw">WITH</span> dupes <span class="kw">AS</span> (
  <span class="kw">SELECT</span> *,
    <span class="fn">ROW_NUMBER</span>() <span class="kw">OVER</span> (
      <span class="kw">PARTITION BY</span> email
      <span class="kw">ORDER BY</span> created_at
    ) <span class="kw">AS</span> rn
  <span class="kw">FROM</span> users
)
<span class="kw">SELECT</span> * <span class="kw">FROM</span> dupes <span class="kw">WHERE</span> rn = <span class="num">1</span>; <span class="cm">-- только первая запись</span></code></pre>

<h2>Топ-N по группам</h2>
<pre><code><span class="cm">-- Топ-3 товара по продажам в каждой категории:</span>
<span class="kw">WITH</span> ranked <span class="kw">AS</span> (
  <span class="kw">SELECT</span>
    category, product, sales,
    <span class="fn">ROW_NUMBER</span>() <span class="kw">OVER</span> (
      <span class="kw">PARTITION BY</span> category
      <span class="kw">ORDER BY</span> sales <span class="kw">DESC</span>
    ) <span class="kw">AS</span> rn
  <span class="kw">FROM</span> products
)
<span class="kw">SELECT</span> category, product, sales
<span class="kw">FROM</span> ranked
<span class="kw">WHERE</span> rn <= <span class="num">3</span>;</code></pre>
<div class="tip"><div class="tip-label">💡 Типичная задача на собеседовании</div><p>«Найти топ-N по каждой группе» — решается через ROW_NUMBER() + CTE + WHERE rn &lt;= N. Запомни этот паттерн.</p></div>
`,
  quizzes: [
    { q: "Как найти топ-1 товар по продажам в каждой категории?", code: null,
      opts: ["GROUP BY category ORDER BY sales DESC LIMIT 1", "ROW_NUMBER() OVER(PARTITION BY category ORDER BY sales DESC), WHERE rn=1", "MAX(sales) GROUP BY category", "RANK() OVER(ORDER BY sales DESC) WHERE rank=1"],
      correct: 1, explain: "GROUP BY + LIMIT 1 вернёт одну строку на всю таблицу, а не на каждую категорию. Нужны оконные функции: ROW_NUMBER внутри PARTITION BY category, потом фильтруем rn=1." },
    { q: "Что делает CASE WHEN в SELECT?", code: "SELECT name,\n  CASE WHEN score >= 90 THEN 'A'\n       WHEN score >= 70 THEN 'B'\n       ELSE 'C'\n  END AS grade\nFROM students;",
      opts: ["Фильтрует строки по score", "Создаёт вычисляемый столбец grade для каждой строки", "Обновляет значения в таблице", "Группирует студентов"],
      correct: 1, explain: "CASE WHEN — это выражение, не фильтр. Оно возвращает значение для каждой строки. Строки не удаляются — просто каждая получает свой grade." },
  ]
}
];

// ============================================================
// STATE
// ============================================================
let state = { checked: {}, quizPassed: {}, totalRight: 0, totalAnswered: 0 };
try { const s = localStorage.getItem('sqlacademy'); if(s) state = JSON.parse(s); } catch(e){}
function save() { try { localStorage.setItem('sqlacademy', JSON.stringify(state)); } catch(e){} }

// ============================================================
// SIDEBAR
// ============================================================
function buildSidebar() {
  const el = document.getElementById('sbModules');
  el.innerHTML = '';
  MODULES.forEach((m, i) => {
    const doneT = m.topics.filter((_,ti)=>state.checked[`${i}-${ti}`]).length;
    const allDone = doneT === m.topics.length;
    const a = document.createElement('a');
    a.href = '#';
    a.className = 'sb-item' + (allDone ? ' done' : '');
    a.id = `sb-m${i}`;
    a.onclick = (e) => { e.preventDefault(); showPage('m'+i); };
    a.innerHTML = `<div class="sb-dot"></div><span class="sb-label">${m.tag}: ${m.title}</span>${allDone?'<span class="sb-check">✓</span>':''}`;
    el.appendChild(a);
  });
  updateStats();
}

function updateStats() {
  let done = 0, total = 0;
  MODULES.forEach((m,i) => { m.topics.forEach((_,ti) => { total++; if(state.checked[`${i}-${ti}`]) done++; }); });
  const pct = total ? Math.round(done/total*100) : 0;
  document.getElementById('navBar').style.width = pct + '%';
  document.getElementById('navPct').textContent = pct + '%';
  document.getElementById('stTopics').textContent = done;
  const qTotal = Object.keys(state.quizPassed).length;
  document.getElementById('stQuiz').textContent = state.totalAnswered > 0 ? Math.round(state.totalRight/state.totalAnswered*100)+'%' : '—';
}

// ============================================================
// PAGES
// ============================================================
function showPage(id) {
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.sb-item').forEach(a=>a.classList.remove('active'));
  const pg = document.getElementById('page-'+id);
  if(pg) { pg.classList.add('active'); window.scrollTo(0,0); }
  const sb = document.getElementById('sb-'+id) || document.querySelector(`.sb-item[onclick*="${id}"]`);
  if(sb) sb.classList.add('active');
  document.querySelectorAll('.mob-btn').forEach(b=>b.classList.remove('active'));
  if(id==='home') document.getElementById('mob-home')?.classList.add('active');
  else document.getElementById('mob-modules')?.classList.add('active');
}

function showMobModules() {
  const sidebar = document.getElementById('sidebar');
  sidebar.style.display = sidebar.style.display === 'flex' ? 'none' : 'flex';
  sidebar.style.position = 'fixed';
  sidebar.style.top = '53px';
  sidebar.style.left = '0';
  sidebar.style.bottom = '60px';
  sidebar.style.width = '260px';
  sidebar.style.zIndex = '150';
}

// ============================================================
// BUILD MODULE PAGES
// ============================================================
function buildModulePages() {
  const container = document.getElementById('modulePages');
  MODULES.forEach((mod, mi) => {
    const div = document.createElement('div');
    div.className = 'page';
    div.id = `page-m${mi}`;

    // Checklist HTML
    const checklistHTML = mod.topics.map((t,ti) => {
      const key = `${mi}-${ti}`;
      const checked = state.checked[key];
      return `<div class="check-item ${checked?'checked':''}" id="ci-${mi}-${ti}" onclick="toggleCheck(${mi},${ti})">
        <div class="check-box">${checked?'✓':''}</div>
        <div class="check-text"><div class="check-title">${t.title}</div><div class="check-sub">${t.sub}</div></div>
      </div>`;
    }).join('');

    // Quiz HTML
    const quizHTML = `
      <div class="quiz-section">
        <div class="quiz-header">
          <div class="quiz-title">🧪 Мини-тест</div>
          <div class="quiz-counter" id="qcnt-${mi}">Вопрос 1 из ${mod.quizzes.length}</div>
        </div>
        <div id="quiz-body-${mi}"></div>
      </div>`;

    div.innerHTML = `
      <div class="module-page">
        <div class="module-header">
          <div class="module-tag">${mod.tag}</div>
          <div class="module-title">${mod.title}</div>
          <div class="module-desc">${mod.desc}</div>
          <div class="module-meta-row">
            <span class="meta-chip">⏱ ${mod.time}</span>
            <span class="meta-chip">📝 ${mod.topics.length} тем</span>
            <span class="meta-chip">🧪 ${mod.quizzes.length} вопроса</span>
          </div>
        </div>
        <div class="divider"></div>
        <div class="lecture">${mod.lecture}</div>
        <div class="divider"></div>
        <h2 style="font-size:18px;font-weight:700;margin-bottom:12px;">📋 Чеклист тем</h2>
        <div class="checklist">${checklistHTML}</div>
        ${quizHTML}
        <div style="display:flex;gap:12px;margin-top:32px;flex-wrap:wrap;">
          ${mi > 0 ? `<button class="btn btn-outline" onclick="showPage('m${mi-1}')">← Предыдущий</button>` : ''}
          ${mi < MODULES.length-1 ? `<button class="btn btn-primary" onclick="showPage('m${mi+1}')">Следующий модуль →</button>` : '<button class="btn btn-primary" onclick="showPage(\'home\')">🎉 Завершить курс</button>'}
        </div>
      </div>`;
    container.appendChild(div);
    initQuiz(mi);
  });
}

function toggleCheck(mi, ti) {
  const key = `${mi}-${ti}`;
  state.checked[key] = !state.checked[key];
  save();
  const el = document.getElementById(`ci-${mi}-${ti}`);
  const box = el.querySelector('.check-box');
  if(state.checked[key]) { el.classList.add('checked'); box.textContent = '✓'; }
  else { el.classList.remove('checked'); box.textContent = ''; }
  buildSidebar();
}

// ============================================================
// QUIZ ENGINE
// ============================================================
let quizState = {};
function initQuiz(mi) {
  quizState[mi] = { idx: 0, right: 0, total: 0 };
  renderQuestion(mi);
}
function renderQuestion(mi) {
  const mod = MODULES[mi];
  const qs = quizState[mi];
  const body = document.getElementById(`quiz-body-${mi}`);
  const cnt = document.getElementById(`qcnt-${mi}`);
  if(qs.idx >= mod.quizzes.length) {
    const pct = Math.round(qs.right/mod.quizzes.length*100);
    body.innerHTML = `<div class="quiz-result">
      <div class="quiz-result-score" style="color:${pct>=50?'var(--green)':'var(--red)'}">${pct}%</div>
      <div class="quiz-result-sub">${qs.right} из ${mod.quizzes.length} правильно</div>
      <div style="font-size:14px;color:${pct>=50?'var(--green)':'var(--amber)'};margin-bottom:20px;">${pct===100?'Отлично! Всё верно 🎉':pct>=50?'Хороший результат! Можно двигаться дальше.':'Рекомендуем перечитать материал.'}</div>
      <button class="btn btn-outline" onclick="resetQuiz(${mi})">Пройти ещё раз</button>
    </div>`;
    if(cnt) cnt.textContent = 'Завершён';
    state.quizPassed[mi] = pct;
    save(); updateStats();
    return;
  }
  const q = mod.quizzes[qs.idx];
  if(cnt) cnt.textContent = `Вопрос ${qs.idx+1} из ${mod.quizzes.length}`;
  body.innerHTML = `
    <div class="quiz-q">${q.q}</div>
    ${q.code ? `<div class="quiz-code">${q.code}</div>` : ''}
    <div class="quiz-opts">
      ${q.opts.map((o,i)=>`<button class="quiz-opt" onclick="answer(${mi},${i})" id="qo-${mi}-${i}">${o}</button>`).join('')}
    </div>
    <div class="quiz-feedback" id="qf-${mi}"></div>
    <div id="qnav-${mi}" style="margin-top:14px;display:none;">
      <button class="btn btn-primary" onclick="nextQ(${mi})">Следующий →</button>
    </div>`;
}
function answer(mi, chosen) {
  const q = MODULES[mi].quizzes[quizState[mi].idx];
  document.querySelectorAll(`[id^="qo-${mi}-"]`).forEach(b=>b.disabled=true);
  const fb = document.getElementById(`qf-${mi}`);
  if(chosen === q.correct) {
    document.getElementById(`qo-${mi}-${chosen}`).classList.add('correct');
    fb.className = 'quiz-feedback ok';
    fb.textContent = '✓ Верно! ' + q.explain;
    quizState[mi].right++;
    state.totalRight++;
  } else {
    document.getElementById(`qo-${mi}-${chosen}`).classList.add('wrong');
    document.getElementById(`qo-${mi}-${q.correct}`).classList.add('correct');
    fb.className = 'quiz-feedback bad';
    fb.textContent = '✗ Неверно. ' + q.explain;
  }
  quizState[mi].total++;
  state.totalAnswered++;
  document.getElementById(`qnav-${mi}`).style.display = 'block';
  save(); updateStats();
}
function nextQ(mi) { quizState[mi].idx++; renderQuestion(mi); }
function resetQuiz(mi) { quizState[mi] = {idx:0, right:0, total:0}; renderQuestion(mi); }

// ============================================================
// INIT
// ============================================================
buildModulePages();
buildSidebar();
</script>
</body>
</html>
