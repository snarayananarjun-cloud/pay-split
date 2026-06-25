<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no" />
<title>Pay Split</title>
<link rel="manifest" href="manifest.json" />
<meta name="theme-color" content="#F5F5F3" />
<meta name="apple-mobile-web-app-capable" content="yes" />
<meta name="apple-mobile-web-app-status-bar-style" content="default" />
<meta name="apple-mobile-web-app-title" content="Pay Split" />
<link rel="apple-touch-icon" href="apple-touch-icon.png" />
<link rel="icon" href="icon-192.png" />
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700;800&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #F5F5F3;
    --ink: #111;
    --soft: #999;
    --line: #E0E0DC;
    --accent: #111;
    --green: #2E7D32;
    --pill: 999px;
  }
  * { box-sizing: border-box; margin: 0; padding: 0; -webkit-tap-highlight-color: transparent; }
  html, body { background: var(--bg); font-family: 'Manrope', sans-serif; color: var(--ink); min-height: 100vh; }
  #app { max-width: 390px; margin: 0 auto; padding: 52px 24px 80px; }

  /* Screen toggle */
  .screen { display: none; }
  .screen.active { display: block; }

  /* ── Top row ── */
  .top-row { display: flex; justify-content: space-between; align-items: center; margin-bottom: 40px; }
  .top-meta { font-size: 13px; color: var(--soft); font-weight: 600; letter-spacing: .3px; }
  .top-meta strong { color: var(--ink); font-weight: 700; }
  .ghost-btn { background: none; border: none; font-family: inherit; font-size: 13px; font-weight: 600; color: var(--soft); cursor: pointer; padding: 0; }

  /* ── Pay input ── */
  .pay-block { margin-bottom: 36px; }
  .pay-eyebrow { font-size: 12px; font-weight: 700; letter-spacing: 1px; color: var(--soft); text-transform: uppercase; margin-bottom: 10px; }
  .pay-row { display: flex; align-items: baseline; gap: 3px; }
  .pay-sym { font-size: 28px; font-weight: 700; color: var(--soft); }
  .pay-input { font-size: 48px; font-weight: 800; color: var(--ink); background: none; border: none; outline: none; font-family: inherit; width: 100%; min-width: 0; letter-spacing: -1px; }
  .pay-input::placeholder { color: #CCC; }
  .pay-sub { font-size: 13px; color: var(--soft); margin-top: 6px; font-weight: 500; }

  /* ── Split button ── */
  .cta { width: 100%; background: var(--ink); color: #fff; border: none; border-radius: var(--pill); padding: 15px; font-size: 15px; font-weight: 700; font-family: inherit; cursor: pointer; margin-bottom: 40px; opacity: .3; transition: opacity .15s; }
  .cta.on { opacity: 1; }

  /* ── List ── */
  .section-label { font-size: 11px; font-weight: 700; letter-spacing: 1.2px; text-transform: uppercase; color: var(--soft); margin-bottom: 4px; }
  .list { margin-bottom: 32px; }
  .list-row { display: flex; justify-content: space-between; align-items: center; padding: 14px 0; border-bottom: 1px solid var(--line); }
  .list-row:last-child { border-bottom: none; }
  .row-left { display: flex; flex-direction: column; gap: 2px; }
  .row-name { font-size: 15px; font-weight: 600; }
  .row-sub { font-size: 12px; color: var(--soft); font-weight: 500; }
  .row-amount { font-size: 17px; font-weight: 700; }
  .row-amount.wedding { color: var(--green); font-size: 19px; }
  .row-amount.soft { color: var(--soft); }

  /* ── Divider ── */
  .divider { height: 1px; background: var(--line); margin: 8px 0 32px; }

  /* ── Edit link ── */
  .edit-link { font-size: 13px; color: var(--soft); font-weight: 600; cursor: pointer; text-decoration: underline; text-underline-offset: 3px; display: inline-block; margin-bottom: 32px; }

  /* ── Edit sheet ── */
  .edit-section { background: #EEEEED; border-radius: 18px; padding: 4px 16px; margin-bottom: 32px; }
  .edit-row { display: flex; justify-content: space-between; align-items: center; padding: 13px 0; border-bottom: 1px solid #DDDDD9; }
  .edit-row:last-child { border-bottom: none; }
  .edit-name { font-size: 14px; font-weight: 600; }
  .edit-right { display: flex; align-items: center; gap: 2px; }
  .edit-sym { font-size: 13px; color: var(--soft); }
  .edit-input { font-size: 15px; font-weight: 700; text-align: right; background: none; border: none; outline: none; font-family: inherit; color: var(--ink); width: 80px; }
  .split-edit-row { display: flex; justify-content: space-between; align-items: center; padding: 13px 0; }
  .split-name { font-size: 14px; font-weight: 600; }
  .split-controls { display: flex; align-items: center; gap: 14px; }
  .split-val { font-size: 15px; font-weight: 700; min-width: 40px; text-align: center; }
  .split-tap { width: 32px; height: 32px; background: #fff; border: 1px solid #D0D0CC; border-radius: 50%; font-size: 18px; cursor: pointer; display: flex; align-items: center; justify-content: center; font-family: inherit; color: var(--ink); }

  /* ── Logs screen ── */
  .back-row { display: flex; align-items: center; gap: 14px; margin-bottom: 36px; }
  .back-tap { background: none; border: none; font-size: 22px; cursor: pointer; padding: 0; color: var(--ink); }
  .logs-heading { font-size: 22px; font-weight: 800; }
  .log-block { margin-bottom: 28px; }
  .log-week-label { font-size: 11px; font-weight: 700; letter-spacing: 1px; text-transform: uppercase; color: var(--soft); margin-bottom: 4px; }
  .log-pay-line { font-size: 26px; font-weight: 800; margin-bottom: 8px; }
  .log-date-line { font-size: 13px; color: var(--soft); margin-bottom: 10px; font-weight: 500; }
  .log-rows { border-top: 1px solid var(--line); }
  .log-row { display: flex; justify-content: space-between; padding: 10px 0; border-bottom: 1px solid var(--line); font-size: 14px; }
  .log-row .name { color: var(--soft); font-weight: 500; }
  .log-row .val { font-weight: 700; }
  .log-row .val.wedding { color: var(--green); }
  .empty-state { text-align: center; padding: 80px 0; color: var(--soft); }
  .empty-state .e-head { font-size: 17px; font-weight: 700; color: var(--ink); margin-bottom: 6px; }

  /* ── Toast ── */
  .toast { position: fixed; bottom: 32px; left: 50%; transform: translateX(-50%) translateY(10px); background: var(--ink); color: #fff; padding: 11px 20px; border-radius: var(--pill); font-size: 13px; font-weight: 600; opacity: 0; transition: all .2s; pointer-events: none; z-index: 99; white-space: nowrap; font-family: inherit; }
  .toast.show { opacity: 1; transform: translateX(-50%) translateY(0); }
</style>
</head>
<body>
<div id="app">

  <!-- ════ MAIN ════ -->
  <div class="screen active" id="s-main">

    <div class="top-row">
      <div class="top-meta" id="top-meta">Week 1 · June</div>
      <button class="ghost-btn" onclick="goLogs()">Past weeks →</button>
    </div>

    <div class="pay-block">
      <div class="pay-eyebrow">This week's pay</div>
      <div class="pay-row">
        <span class="pay-sym">€</span>
        <input class="pay-input" id="pay-input" type="text" inputmode="decimal" placeholder="0" oninput="onInput()" />
      </div>
      <div class="pay-sub" id="month-total">€0 earned this month</div>
    </div>

    <button class="cta" id="cta" onclick="doSplit()" disabled>Split →</button>

    <!-- Results list -->
    <div id="results" style="display:none;">

      <div class="section-label">Savings</div>
      <div class="list">
        <div class="list-row">
          <div class="row-left">
            <div class="row-name">Wedding fund</div>
            <div class="row-sub" id="wedding-sub">80% of what's left</div>
          </div>
          <div class="row-amount wedding" id="r-wedding">€0</div>
        </div>
        <div class="list-row">
          <div class="row-left">
            <div class="row-name">September fund</div>
            <div class="row-sub">Visa + insurance · €550 by Sept</div>
          </div>
          <div class="row-amount soft" id="r-sept">€0</div>
        </div>
      </div>

      <div class="section-label">Fixed</div>
      <div class="list" id="fixed-list"></div>

      <div class="section-label" style="margin-top:8px;">Leftover</div>
      <div class="list">
        <div class="list-row">
          <div class="row-left">
            <div class="row-name">Miscellaneous</div>
            <div class="row-sub" id="misc-sub">20% of what's left</div>
          </div>
          <div class="row-amount soft" id="r-misc">€0</div>
        </div>
      </div>

      <div class="divider"></div>

      <span class="edit-link" onclick="toggleEdit()">Edit amounts &amp; split</span>

      <div id="edit-section" style="display:none;">
        <div class="edit-section" id="edit-rows"></div>
        <div class="edit-section" style="margin-top:12px; padding: 4px 16px;">
          <div class="split-edit-row">
            <span class="split-name">Wedding split</span>
            <div class="split-controls">
              <button class="split-tap" onclick="nudgeSplit(-5)">−</button>
              <span class="split-val" id="split-val">80%</span>
              <button class="split-tap" onclick="nudgeSplit(5)">+</button>
            </div>
          </div>
        </div>
      </div>

    </div>
  </div>

  <!-- ════ LOGS ════ -->
  <div class="screen" id="s-logs">
    <div class="back-row">
      <button class="back-tap" onclick="goMain()">←</button>
      <div class="logs-heading">Past weeks</div>
    </div>
    <div id="logs-list"></div>
  </div>

</div>

<div class="toast" id="toast"></div>

<script>
// ── Config ──
const POCKETS = JSON.parse(localStorage.getItem('ps2_pockets') || 'null') || [
  { id:'rent',      name:'Rent',          monthly:625  },
  { id:'home',      name:'Home (family)', monthly:250  },
  { id:'groceries', name:'Groceries',     monthly:80   },
  { id:'gas',       name:'Gas',           monthly:64   },
  { id:'electric',  name:'Electricity',   monthly:67   },
  { id:'transport', name:'Transport',     monthly:25   },
  { id:'sim',       name:'SIM',           monthly:13   },
  { id:'wifi',      name:'WiFi',          monthly:7.5  },
  { id:'claude',    name:'Claude Pro',    monthly:22   },
];
let wSplit = parseInt(localStorage.getItem('ps2_split') || '80');
let logs   = JSON.parse(localStorage.getItem('ps2_logs')  || '[]');
const SEPT = 550 / 13;

function persist() {
  localStorage.setItem('ps2_pockets', JSON.stringify(POCKETS));
  localStorage.setItem('ps2_split',   String(wSplit));
  localStorage.setItem('ps2_logs',    JSON.stringify(logs));
}

// ── Date helpers ──
const MONTHS = ['Jan','Feb','Mar','Apr','May','Jun','Jul','Aug','Sep','Oct','Nov','Dec'];
const DAYS   = ['Sun','Mon','Tue','Wed','Thu','Fri','Sat'];
function weekOfMonth(d) { return Math.ceil(d.getDate() / 7); }
function fmtShort(d)    { return `${DAYS[d.getDay()]} ${d.getDate()} ${MONTHS[d.getMonth()]}`; }
function monthKey(d)    { return `${d.getFullYear()}-${d.getMonth()}`; }
function eur(n)         { return '€' + Math.round(n).toLocaleString('en-IE'); }

// ── Init ──
(function init() {
  const now = new Date();
  document.getElementById('top-meta').textContent =
    `Week ${weekOfMonth(now)} · ${now.toLocaleString('default',{month:'long'})}`;
  refreshMonthTotal(0);
})();

function refreshMonthTotal(thisPay) {
  const now = new Date();
  const mk  = monthKey(now);
  const base = logs.filter(l => l.mk === mk).reduce((s,l) => s + l.pay, 0);
  document.getElementById('month-total').textContent =
    `${eur(base + thisPay)} earned this month`;
}

// ── Input ──
function onInput() {
  const v = parseFloat(document.getElementById('pay-input').value) || 0;
  const cta = document.getElementById('cta');
  cta.disabled = v <= 0;
  cta.classList.toggle('on', v > 0);
  refreshMonthTotal(v);
}

// ── Split ──
function doSplit() {
  const pay = parseFloat(document.getElementById('pay-input').value) || 0;
  if (!pay) return;

  const fixedW = POCKETS.reduce((s,p) => s + p.monthly/4, 0);
  const left   = Math.max(0, pay - fixedW - SEPT);
  const wed    = left * wSplit / 100;
  const misc   = left * (100 - wSplit) / 100;

  // Render results
  document.getElementById('r-wedding').textContent = eur(wed);
  document.getElementById('r-sept').textContent    = eur(SEPT);
  document.getElementById('r-misc').textContent    = eur(misc);
  document.getElementById('wedding-sub').textContent = `${wSplit}% of what's left`;
  document.getElementById('misc-sub').textContent    = `${100-wSplit}% of what's left`;

  const fl = document.getElementById('fixed-list');
  fl.innerHTML = POCKETS.map(p => `
    <div class="list-row">
      <div class="row-left">
        <div class="row-name">${p.name}</div>
        <div class="row-sub">€${p.monthly}/month</div>
      </div>
      <div class="row-amount soft">${eur(p.monthly/4)}</div>
    </div>
  `).join('');

  document.getElementById('results').style.display = 'block';
  buildEditRows();

  // Save log
  const now = new Date();
  const wk  = weekOfMonth(now);
  const mk  = monthKey(now);
  logs = logs.filter(l => !(l.mk === mk && l.wk === wk));
  logs.unshift({ pay, wk, mk, date: fmtShort(now),
    mLabel: now.toLocaleString('default',{month:'long',year:'numeric'}),
    wed, misc, sept: SEPT,
    pockets: POCKETS.map(p=>({name:p.name, weekly: p.monthly/4}))
  });
  persist();
  refreshMonthTotal(pay);
  toast('Split saved ✓');
}

// ── Edit ──
let editOpen = false;
function toggleEdit() {
  editOpen = !editOpen;
  document.getElementById('edit-section').style.display = editOpen ? 'block' : 'none';
  document.querySelector('.edit-link').textContent = editOpen ? 'Done editing' : 'Edit amounts & split';
}
function buildEditRows() {
  document.getElementById('split-val').textContent = `${wSplit}%`;
  const c = document.getElementById('edit-rows');
  c.innerHTML = POCKETS.map((p,i) => `
    <div class="edit-row">
      <span class="edit-name">${p.name}</span>
      <div class="edit-right">
        <span class="edit-sym">€</span>
        <input class="edit-input" type="text" inputmode="decimal"
          value="${p.monthly}"
          onchange="updateP(${i},this.value)" />
        <span class="edit-sym">/mo</span>
      </div>
    </div>
  `).join('');
}
function updateP(i, v) {
  POCKETS[i].monthly = parseFloat(v) || 0;
  persist();
  doSplit();
  toast('Updated');
}
function nudgeSplit(d) {
  wSplit = Math.min(95, Math.max(50, wSplit + d));
  document.getElementById('split-val').textContent = `${wSplit}%`;
  persist();
  doSplit();
}

// ── Logs ──
function goLogs() {
  document.getElementById('s-main').classList.remove('active');
  document.getElementById('s-logs').classList.add('active');
  const c = document.getElementById('logs-list');
  if (!logs.length) {
    c.innerHTML = `<div class="empty-state"><div class="e-head">No weeks logged yet</div>Split your first pay and it'll appear here.</div>`;
    return;
  }
  c.innerHTML = logs.map(l => `
    <div class="log-block">
      <div class="log-week-label">Week ${l.wk} · ${l.mLabel}</div>
      <div class="log-pay-line">${eur(l.pay)}</div>
      <div class="log-date-line">${l.date}</div>
      <div class="log-rows">
        <div class="log-row"><span class="name">Wedding fund</span><span class="val wedding">${eur(l.wed)}</span></div>
        <div class="log-row"><span class="name">Sept fund</span><span class="val">${eur(l.sept)}</span></div>
        ${l.pockets.slice(0,4).map(p=>`<div class="log-row"><span class="name">${p.name}</span><span class="val">${eur(p.weekly)}</span></div>`).join('')}
        <div class="log-row"><span class="name">Misc</span><span class="val">${eur(l.misc)}</span></div>
      </div>
    </div>
  `).join('');
}
function goMain() {
  document.getElementById('s-logs').classList.remove('active');
  document.getElementById('s-main').classList.add('active');
}

// ── Toast ──
function toast(msg) {
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), 1600);
}
</script>
</body>
</html>
