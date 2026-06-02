/* ══════════════════════════════════════════
   NATURE THEME — FIT2179 DV2
   Australia's Threatened Species Crisis
   ══════════════════════════════════════════ */

:root {
  --bg:       #f4f1ea;
  --surface:  #ffffff;
  --surface2: #e9ece4;
  --border:   #d1d8c9;
  --text:     #2c3e2d;
  --muted:    #6b7a68;
  --ce:       #c84b31;
  --en:       #d98841;
  --vu:       #e1b12c;
  --accent:   #4a6741;
  --link:     #3a5a30;
  --nav-h:    56px;
}

*, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }

body {
  background: var(--bg);
  color: var(--text);
  font-family: 'Source Sans 3', sans-serif;
  font-size: 16px;
  line-height: 1.65;
}

/* NAV */
.topnav {
  position: sticky; top: 0; z-index: 100;
  background: rgba(244, 241, 234, 0.96);
  backdrop-filter: blur(8px);
  border-bottom: 1px solid var(--border);
  height: var(--nav-h);
  display: flex; align-items: center;
}
.nav-inner {
  max-width: 1200px; margin: 0 auto; padding: 0 32px;
  width: 100%; display: flex; align-items: center; justify-content: space-between;
}
.nav-brand { font-weight: 700; font-size: 0.88rem; color: var(--text); }
.nav-links { display: flex; gap: 28px; }
.nav-links a {
  text-decoration: none; font-size: 0.82rem; font-weight: 600;
  letter-spacing: 0.8px; text-transform: uppercase; color: var(--muted); transition: color 0.2s;
}
.nav-links a:hover { color: var(--accent); }

/* HERO */
.hero {
  background: linear-gradient(160deg, #e4ede0 0%, #f4f1ea 40%, #faf9f5 100%);
  padding: 90px 40px 70px; text-align: center;
  border-bottom: 1px solid var(--border);
  position: relative; overflow: hidden;
}
.hero::before {
  content: ''; position: absolute; inset: 0;
  background: radial-gradient(ellipse at 50% 0%, rgba(74,103,65,.09) 0%, transparent 68%);
  pointer-events: none;
}
.hero-kicker {
  font-size: 10.5px; font-weight: 700; letter-spacing: 5px;
  text-transform: uppercase; color: var(--accent); margin-bottom: 20px;
}
.hero h1 {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2.4rem, 5vw, 4.4rem);
  font-weight: 900; line-height: 1.08; color: var(--text);
  margin-bottom: 22px; letter-spacing: -0.5px;
}
.hero h1 em { font-style: normal; color: var(--ce); }
.hero-sub {
  max-width: 680px; margin: 0 auto 44px;
  color: var(--muted); font-size: 1.05rem; line-height: 1.78;
}
.hero-note { font-size: 0.78rem; color: var(--muted); margin-top: 28px; opacity: 0.7; }

/* STAT CARDS */
.stat-row { display: flex; justify-content: center; flex-wrap: wrap; gap: 20px; }
.stat-card {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: 12px; padding: 22px 36px; text-align: center; min-width: 158px;
  box-shadow: 0 4px 16px rgba(44,62,45,.05);
  transition: transform 0.15s, box-shadow 0.15s;
}
.stat-card:hover { transform: translateY(-2px); box-shadow: 0 8px 24px rgba(44,62,45,.1); }
.stat-num { font-family: 'Playfair Display', serif; font-size: 2.7rem; font-weight: 700; line-height: 1; }
.stat-label { font-size: 0.72rem; font-weight: 700; letter-spacing: 1.8px; text-transform: uppercase; color: var(--muted); margin-top: 7px; }
.stat-card.ce  .stat-num { color: var(--ce); }
.stat-card.en  .stat-num { color: var(--en); }
.stat-card.vu  .stat-num { color: var(--vu); }
.stat-card.tot .stat-num { color: var(--accent); }

/* PAGE LAYOUT */
.page { max-width: 1200px; margin: 0 auto; padding: 0 32px; }
section { padding: 68px 0 24px; }

/* SECTION HEADERS */
.section-label {
  font-size: 10.5px; letter-spacing: 4.5px; text-transform: uppercase;
  color: var(--accent); font-weight: 700; margin-bottom: 10px;
}
.section-title {
  font-family: 'Playfair Display', serif;
  font-size: clamp(1.6rem, 3vw, 2.4rem);
  font-weight: 700; margin-bottom: 14px; color: var(--text);
  letter-spacing: -0.3px; line-height: 1.2;
}
.section-desc {
  color: var(--muted); max-width: 720px; margin-bottom: 36px;
  font-size: 1.0rem; line-height: 1.75;
}

/* CHART GRIDS */
.chart-grid-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 24px; margin-bottom: 28px; }
.chart-full { margin-bottom: 28px; }

/* CHART CARDS */
.chart-card {
  background: var(--surface); border: 1px solid var(--border);
  border-radius: 14px; padding: 26px 22px 20px;
  box-shadow: 0 2px 10px rgba(44,62,45,.04);
}
.chart-card h3 {
  font-family: 'Playfair Display', serif; font-size: 1.08rem;
  font-weight: 700; margin-bottom: 5px; color: var(--text); line-height: 1.35;
}
.chart-desc {
  font-size: 0.83rem; color: var(--muted); margin-bottom: 16px;
  line-height: 1.55; max-width: 600px;
}
.chart-annotation {
  font-size: 0.82rem; color: var(--muted); margin-top: 12px;
  padding: 10px 14px;
  background: rgba(74,103,65,.05);
  border-left: 3px solid var(--accent);
  border-radius: 0 6px 6px 0; line-height: 1.5;
}
.chart-annotation strong { color: var(--text); }
.chart-card .vega-embed { width: 100%; }
.chart-card .vega-embed canvas,
.chart-card .vega-embed svg { max-width: 100%; }

/* LEGEND STRIP */
.legend-strip {
  display: flex; gap: 28px; flex-wrap: wrap; margin-bottom: 28px;
  padding: 14px 18px; background: var(--surface);
  border: 1px solid var(--border); border-radius: 8px;
}
.legend-item { display: flex; align-items: center; gap: 9px; font-size: 0.85rem; color: var(--text); }
.legend-dot { width: 13px; height: 13px; border-radius: 3px; flex-shrink: 0; }

/* DIVIDER */
.divider { border: none; border-top: 1px solid var(--border); margin: 16px 0; }

/* CALLOUT */
.callout {
  background: rgba(200,75,49,.045);
  border-left: 4px solid var(--ce);
  border-radius: 0 10px 10px 0;
  padding: 20px 28px; margin: 28px 0 8px;
  font-size: 0.97rem; color: var(--text); line-height: 1.7;
}
.callout strong { color: var(--ce); }

/* FOOTER */
.nature-footer {
  background: linear-gradient(180deg, var(--bg) 0%, var(--surface2) 100%);
  border-top: 2px solid var(--border);
  padding: 60px 32px 48px; margin-top: 72px;
}
.footer-content { max-width: 1200px; margin: 0 auto; }
.footer-meta { display: grid; grid-template-columns: 1fr 1fr 1fr; gap: 36px; margin-bottom: 32px; }
.footer-block { font-size: 0.87rem; color: var(--muted); line-height: 1.7; }
.footer-block strong {
  display: block; font-size: 0.72rem; letter-spacing: 2px;
  text-transform: uppercase; color: var(--accent); margin-bottom: 8px; font-weight: 700;
}
.footer-block a { color: var(--link); text-decoration: none; font-weight: 600; word-break: break-word; }
.footer-block a:hover { color: var(--accent); text-decoration: underline; }
.footer-copy {
  font-size: 0.80rem; color: var(--muted); line-height: 1.65;
  border-top: 1px solid var(--border); padding-top: 20px; opacity: 0.75;
}

/* RESPONSIVE */
@media (max-width: 900px) {
  .chart-grid-2 { grid-template-columns: 1fr; }
  .footer-meta  { grid-template-columns: 1fr; }
}
@media (max-width: 640px) {
  .hero { padding: 60px 20px 50px; }
  .page { padding: 0 16px; }
  .nav-inner { padding: 0 16px; }
  .nav-links { display: none; }
  .hero-sub { font-size: 0.97rem; }
  .stat-card { min-width: 130px; padding: 16px 20px; }
}