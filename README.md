<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CA–EU Youth Forum 2026 | Самарканд</title>
<meta name="description" content="Центральноазиатско-Европейский молодёжный форум 2026 — Самарканд, Узбекистан, 13–14 августа 2026">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=Onest:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
:root {
  --c-navy: #0B1E3D;
  --c-blue: #1A4FAF;
  --c-gold: #C9973A;
  --c-gold-light: #F0C96A;
  --c-cream: #F7F3EB;
  --c-white: #FFFFFF;
  --c-gray: #6B7280;
  --c-gray-light: #F1EFE8;
  --c-text: #111827;
  --c-eu-yellow: #FFCC00;
  --font-display: 'Playfair Display', Georgia, serif;
  --font-body: 'Onest', system-ui, sans-serif;
  --radius: 12px;
  --shadow: 0 4px 32px rgba(11,30,61,0.10);
}
* { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }
body {
  font-family: var(--font-body);
  color: var(--c-text);
  background: var(--c-white);
  line-height: 1.7;
  overflow-x: hidden;
}

/* ── NAV ── */
.nav {
  position: fixed; top: 0; left: 0; right: 0; z-index: 100;
  background: rgba(11,30,61,0.95);
  backdrop-filter: blur(12px);
  border-bottom: 1px solid rgba(201,151,58,0.2);
}
.nav-inner {
  max-width: 1200px; margin: 0 auto;
  padding: 0 2rem;
  display: flex; align-items: center; justify-content: space-between;
  height: 68px;
}
.nav-logo {
  display: flex; align-items: center; gap: 12px;
  text-decoration: none;
}
.nav-logo-badge {
  width: 40px; height: 40px;
  background: var(--c-gold);
  border-radius: 8px;
  display: flex; align-items: center; justify-content: center;
  font-size: 11px; font-weight: 700;
  color: var(--c-navy);
  letter-spacing: 0.5px;
  line-height: 1.2;
  text-align: center;
}
.nav-logo-text {
  color: var(--c-white);
  font-size: 13px;
  font-weight: 500;
  line-height: 1.3;
}
.nav-logo-text span { color: var(--c-gold); display: block; font-size: 11px; font-weight: 400; }
.nav-links {
  display: flex; gap: 4px; list-style: none;
}
.nav-links a {
  color: rgba(255,255,255,0.8);
  text-decoration: none;
  font-size: 14px;
  padding: 6px 12px;
  border-radius: 6px;
  transition: all 0.2s;
}
.nav-links a:hover { color: var(--c-gold); background: rgba(201,151,58,0.1); }
.nav-cta {
  background: var(--c-gold);
  color: var(--c-navy) !important;
  font-weight: 600 !important;
  border-radius: 8px !important;
  padding: 8px 18px !important;
}
.nav-cta:hover { background: var(--c-gold-light) !important; color: var(--c-navy) !important; }
.nav-lang {
  display: flex; gap: 4px; margin-left: 16px;
}
.nav-lang button {
  background: none; border: 1px solid rgba(255,255,255,0.2);
  color: rgba(255,255,255,0.7);
  font-size: 12px; font-weight: 500;
  padding: 4px 8px; border-radius: 4px;
  cursor: pointer; transition: all 0.2s;
}
.nav-lang button.active, .nav-lang button:hover {
  background: var(--c-gold); color: var(--c-navy); border-color: var(--c-gold);
}
.hamburger {
  display: none;
  flex-direction: column; gap: 5px;
  background: none; border: none; cursor: pointer; padding: 4px;
}
.hamburger span { width: 24px; height: 2px; background: white; border-radius: 2px; transition: all 0.3s; }

/* ── HERO ── */
.hero {
  min-height: 100vh;
  background: linear-gradient(135deg, #0B1E3D 0%, #1A3A6B 45%, #0B2D4A 100%);
  position: relative; overflow: hidden;
  display: flex; align-items: center;
  padding-top: 68px;
}
.hero-bg-pattern {
  position: absolute; inset: 0;
  background-image:
    radial-gradient(circle at 20% 80%, rgba(201,151,58,0.12) 0%, transparent 50%),
    radial-gradient(circle at 80% 20%, rgba(26,79,175,0.3) 0%, transparent 50%),
    repeating-linear-gradient(45deg, rgba(255,255,255,0.015) 0px, rgba(255,255,255,0.015) 1px, transparent 1px, transparent 60px);
}
.hero-stars {
  position: absolute; inset: 0;
  background-image:
    radial-gradient(1.5px 1.5px at 15% 25%, rgba(255,204,0,0.6) 0%, transparent 100%),
    radial-gradient(1px 1px at 40% 15%, rgba(255,255,255,0.5) 0%, transparent 100%),
    radial-gradient(1.5px 1.5px at 70% 30%, rgba(255,204,0,0.4) 0%, transparent 100%),
    radial-gradient(1px 1px at 85% 60%, rgba(255,255,255,0.4) 0%, transparent 100%),
    radial-gradient(1px 1px at 25% 70%, rgba(255,255,255,0.3) 0%, transparent 100%),
    radial-gradient(1px 1px at 60% 80%, rgba(255,204,0,0.5) 0%, transparent 100%),
    radial-gradient(1.5px 1.5px at 90% 45%, rgba(255,255,255,0.4) 0%, transparent 100%);
}
.hero-arc {
  position: absolute; bottom: -2px; left: 0; right: 0;
}
.hero-inner {
  max-width: 1200px; margin: 0 auto; padding: 6rem 2rem 8rem;
  display: grid; grid-template-columns: 1fr 1fr; gap: 4rem; align-items: center;
  position: relative; z-index: 2;
}
.hero-eyebrow {
  display: inline-flex; align-items: center; gap: 8px;
  background: rgba(201,151,58,0.15);
  border: 1px solid rgba(201,151,58,0.4);
  border-radius: 30px;
  padding: 6px 16px;
  font-size: 12px; font-weight: 600;
  color: var(--c-gold);
  letter-spacing: 1.5px;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
}
.hero-eyebrow-dot { width: 6px; height: 6px; background: var(--c-gold); border-radius: 50%; animation: pulse 2s infinite; }
@keyframes pulse { 0%,100%{opacity:1;transform:scale(1)} 50%{opacity:0.5;transform:scale(1.3)} }
.hero-title {
  font-family: var(--font-display);
  font-size: clamp(2.2rem, 4.5vw, 3.8rem);
  font-weight: 900;
  color: var(--c-white);
  line-height: 1.1;
  margin-bottom: 1.2rem;
}
.hero-title .accent { color: var(--c-gold); }
.hero-subtitle {
  font-size: 1.1rem;
  color: rgba(255,255,255,0.75);
  margin-bottom: 2rem;
  line-height: 1.7;
}
.hero-meta {
  display: flex; gap: 1.5rem; margin-bottom: 2.5rem;
  flex-wrap: wrap;
}
.hero-meta-item {
  display: flex; align-items: center; gap: 8px;
  color: rgba(255,255,255,0.8); font-size: 0.9rem;
}
.hero-meta-icon {
  width: 32px; height: 32px;
  background: rgba(201,151,58,0.2);
  border-radius: 8px;
  display: flex; align-items: center; justify-content: center;
  font-size: 16px;
}
.hero-actions { display: flex; gap: 1rem; flex-wrap: wrap; }
.btn-primary {
  background: var(--c-gold);
  color: var(--c-navy);
  border: none;
  padding: 14px 28px;
  border-radius: 10px;
  font-family: var(--font-body);
  font-size: 0.95rem;
  font-weight: 700;
  cursor: pointer;
  text-decoration: none;
  display: inline-block;
  transition: all 0.25s;
  letter-spacing: 0.3px;
}
.btn-primary:hover { background: var(--c-gold-light); transform: translateY(-2px); box-shadow: 0 8px 24px rgba(201,151,58,0.3); }
.btn-secondary {
  background: transparent;
  color: var(--c-white);
  border: 1.5px solid rgba(255,255,255,0.4);
  padding: 14px 28px;
  border-radius: 10px;
  font-family: var(--font-body);
  font-size: 0.95rem;
  font-weight: 500;
  cursor: pointer;
  text-decoration: none;
  display: inline-block;
  transition: all 0.25s;
}
.btn-secondary:hover { border-color: white; background: rgba(255,255,255,0.08); }
.hero-visual {
  display: flex; justify-content: center; align-items: center;
}
.hero-card-stack {
  position: relative; width: 100%; max-width: 420px;
}
.hero-card {
  background: rgba(255,255,255,0.07);
  border: 1px solid rgba(255,255,255,0.15);
  border-radius: 20px;
  padding: 2rem;
  backdrop-filter: blur(10px);
}
.hero-card-flags {
  display: flex; gap: 8px; margin-bottom: 1.5rem;
}
.flag {
  width: 42px; height: 28px; border-radius: 5px; overflow: hidden;
  display: flex; flex-direction: column;
}
.flag-uz { background: linear-gradient(to bottom, #1eb6e8 33.3%, #fff 33.3%, #fff 66.6%, #44ae42 66.6%); position: relative; }
.flag-uz::after { content: ''; position: absolute; left: 4px; top: 5px; width: 8px; height: 8px; background: white; border-radius: 50%; }
.flag-eu {
  background: #003399;
  display: flex; align-items: center; justify-content: center;
  font-size: 11px;
  letter-spacing: -1px;
}
.flag-kz { background: linear-gradient(to bottom, #00AFCA 100%); }
.flag-kg { background: linear-gradient(to bottom, #E8112D 100%); }
.flag-tj { background: linear-gradient(to bottom, #C30017 33.3%, #FFFFFF 33.3%, #FFFFFF 66.6%, #006600 66.6%); }
.flag-tm { background: #30A956; }
.hero-card-stat {
  text-align: center; margin-bottom: 1rem;
}
.hero-card-stat .num {
  font-family: var(--font-display);
  font-size: 3rem; font-weight: 900;
  color: var(--c-gold); line-height: 1;
}
.hero-card-stat .label {
  color: rgba(255,255,255,0.7); font-size: 0.85rem;
}
.hero-card-divider { border: none; border-top: 1px solid rgba(255,255,255,0.1); margin: 1rem 0; }
.hero-card-dates {
  display: grid; grid-template-columns: 1fr 1fr; gap: 12px;
}
.hero-date-box {
  background: rgba(201,151,58,0.12);
  border: 1px solid rgba(201,151,58,0.25);
  border-radius: 10px;
  padding: 12px;
  text-align: center;
}
.hero-date-box .day {
  font-family: var(--font-display);
  font-size: 1.8rem; font-weight: 700;
  color: var(--c-gold); line-height: 1;
}
.hero-date-box .month { color: rgba(255,255,255,0.7); font-size: 0.8rem; margin-top: 2px; }
.countdown {
  margin-top: 1.5rem;
  background: rgba(0,0,0,0.2);
  border-radius: 12px; padding: 1rem;
  text-align: center;
}
.countdown-label { color: rgba(255,255,255,0.6); font-size: 0.8rem; margin-bottom: 8px; text-transform: uppercase; letter-spacing: 1px; }
.countdown-nums {
  display: flex; gap: 8px; justify-content: center;
}
.countdown-unit {
  background: rgba(255,255,255,0.08);
  border-radius: 8px; padding: 8px 10px;
  min-width: 50px;
}
.countdown-unit .n { font-family: var(--font-display); font-size: 1.4rem; font-weight: 700; color: white; line-height: 1; }
.countdown-unit .l { font-size: 0.65rem; color: rgba(255,255,255,0.5); text-transform: uppercase; letter-spacing: 0.5px; margin-top: 2px; }
.hero-scroll {
  position: absolute; bottom: 6rem; left: 50%; transform: translateX(-50%);
  display: flex; flex-direction: column; align-items: center; gap: 8px;
  color: rgba(255,255,255,0.5); font-size: 0.75rem; letter-spacing: 1px;
  text-transform: uppercase;
}
.scroll-arrow { width: 24px; height: 24px; border-right: 2px solid rgba(255,255,255,0.4); border-bottom: 2px solid rgba(255,255,255,0.4); transform: rotate(45deg); animation: bounce 1.8s infinite; }
@keyframes bounce { 0%,100%{transform:rotate(45deg) translateY(0)} 50%{transform:rotate(45deg) translateY(6px)} }

/* ── SECTIONS ── */
section { padding: 6rem 1.5rem; }
.section-inner { max-width: 1200px; margin: 0 auto; }
.section-label {
  display: inline-block;
  font-size: 11px; font-weight: 700;
  letter-spacing: 2.5px; text-transform: uppercase;
  color: var(--c-gold);
  margin-bottom: 0.7rem;
}
.section-title {
  font-family: var(--font-display);
  font-size: clamp(1.8rem, 3.5vw, 2.8rem);
  font-weight: 700;
  color: var(--c-navy);
  line-height: 1.2;
  margin-bottom: 1rem;
}
.section-subtitle {
  font-size: 1.05rem;
  color: var(--c-gray);
  max-width: 580px;
  line-height: 1.7;
}
.text-center { text-align: center; }
.text-center .section-subtitle { margin: 0 auto; }

/* ── STATS BAR ── */
.stats-bar {
  background: var(--c-navy);
  padding: 3rem 1.5rem;
}
.stats-grid {
  max-width: 1200px; margin: 0 auto;
  display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem;
}
.stat-item { text-align: center; padding: 1.5rem; }
.stat-num {
  font-family: var(--font-display);
  font-size: 2.8rem; font-weight: 900;
  color: var(--c-gold);
  line-height: 1;
}
.stat-label { color: rgba(255,255,255,0.7); font-size: 0.9rem; margin-top: 6px; }

/* ── ABOUT ── */
.about { background: var(--c-cream); }
.about-grid {
  display: grid; grid-template-columns: 1fr 1fr; gap: 5rem; align-items: center;
}
.about-image-block {
  position: relative;
}
.about-img-placeholder {
  width: 100%; aspect-ratio: 4/3;
  background: linear-gradient(135deg, var(--c-navy) 0%, #1A4FAF 100%);
  border-radius: 20px;
  display: flex; align-items: center; justify-content: center;
  overflow: hidden;
  position: relative;
}
.about-img-placeholder::before {
  content: '';
  position: absolute; inset: 0;
  background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.04'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
}
.about-img-text {
  text-align: center; color: white; z-index: 1; padding: 2rem;
}
.about-img-text .big { font-family: var(--font-display); font-size: 3rem; font-weight: 900; color: var(--c-gold); }
.about-img-text p { font-size: 0.9rem; color: rgba(255,255,255,0.7); margin-top: 4px; }
.about-badge {
  position: absolute; bottom: -20px; right: -20px;
  background: var(--c-gold); border-radius: 16px; padding: 16px 20px;
  text-align: center; box-shadow: var(--shadow);
}
.about-badge .b-num { font-family: var(--font-display); font-size: 1.8rem; font-weight: 900; color: var(--c-navy); line-height: 1; }
.about-badge .b-label { font-size: 0.75rem; color: rgba(11,30,61,0.7); margin-top: 2px; }
.about-features { display: flex; flex-direction: column; gap: 1.2rem; margin-top: 2rem; }
.feature-item {
  display: flex; align-items: flex-start; gap: 1rem;
  padding: 1rem 1.2rem;
  background: white;
  border-radius: 12px;
  border: 1px solid rgba(0,0,0,0.06);
}
.feature-icon {
  width: 40px; height: 40px; flex-shrink: 0;
  background: rgba(201,151,58,0.1);
  border-radius: 10px;
  display: flex; align-items: center; justify-content: center;
  font-size: 20px;
}
.feature-text h4 { font-weight: 600; font-size: 0.95rem; margin-bottom: 2px; color: var(--c-navy); }
.feature-text p { font-size: 0.85rem; color: var(--c-gray); line-height: 1.5; }

/* ── PROGRAM ── */
.program { background: white; }
.program-tabs {
  display: flex; gap: 8px; margin-bottom: 3rem;
  border-bottom: 2px solid var(--c-gray-light);
  padding-bottom: 0;
}
.tab-btn {
  background: none; border: none; cursor: pointer;
  font-family: var(--font-body);
  font-size: 0.95rem; font-weight: 500;
  color: var(--c-gray);
  padding: 10px 20px;
  border-radius: 8px 8px 0 0;
  transition: all 0.2s;
  position: relative;
}
.tab-btn.active {
  color: var(--c-navy); font-weight: 700;
}
.tab-btn.active::after {
  content: ''; position: absolute; bottom: -2px; left: 0; right: 0;
  height: 2px; background: var(--c-gold); border-radius: 2px 2px 0 0;
}
.program-day { display: none; }
.program-day.active { display: block; }
.program-timeline { position: relative; }
.program-item {
  display: grid; grid-template-columns: 80px 1fr; gap: 1.5rem;
  margin-bottom: 1rem;
  padding: 1.2rem;
  border-radius: 12px;
  transition: background 0.2s;
}
.program-item:hover { background: var(--c-cream); }
.program-time {
  font-family: var(--font-display);
  font-size: 1rem; font-weight: 700;
  color: var(--c-gold);
  padding-top: 2px;
}
.program-content h4 { font-weight: 600; color: var(--c-navy); margin-bottom: 4px; }
.program-content p { font-size: 0.88rem; color: var(--c-gray); }
.program-tag {
  display: inline-block;
  font-size: 0.72rem; font-weight: 600; letter-spacing: 0.5px;
  text-transform: uppercase;
  padding: 3px 10px; border-radius: 20px;
  margin-bottom: 6px;
}
.tag-keynote { background: rgba(201,151,58,0.12); color: #8B6914; }
.tag-panel { background: rgba(26,79,175,0.1); color: #1A4FAF; }
.tag-workshop { background: rgba(16,185,129,0.1); color: #065F46; }
.tag-break { background: rgba(107,114,128,0.1); color: #4B5563; }
.tag-networking { background: rgba(139,92,246,0.1); color: #5B21B6; }

/* ── SPEAKERS ── */
.speakers { background: var(--c-cream); }
.speakers-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 1.5rem;
}
.speaker-card {
  background: white;
  border-radius: 16px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.06);
  transition: all 0.3s;
}
.speaker-card:hover { transform: translateY(-6px); box-shadow: var(--shadow); }
.speaker-photo {
  aspect-ratio: 1;
  background: linear-gradient(135deg, var(--c-navy) 0%, #1A4FAF 100%);
  display: flex; align-items: center; justify-content: center;
  font-size: 3rem;
  position: relative; overflow: hidden;
}
.speaker-photo::after {
  content: ''; position: absolute;
  bottom: 0; left: 0; right: 0;
  height: 40%; background: linear-gradient(to top, rgba(11,30,61,0.5), transparent);
}
.speaker-body { padding: 1.2rem; }
.speaker-name { font-weight: 700; color: var(--c-navy); font-size: 1rem; margin-bottom: 2px; }
.speaker-role { font-size: 0.82rem; color: var(--c-gray); margin-bottom: 8px; }
.speaker-country {
  display: inline-flex; align-items: center; gap: 5px;
  font-size: 0.78rem; color: var(--c-gold); font-weight: 500;
}

/* ── REGISTRATION ── */
.registration { background: white; }
.reg-layout {
  display: grid; grid-template-columns: 1fr 1.2fr; gap: 4rem; align-items: start;
}
.reg-info h3 { font-family: var(--font-display); font-size: 1.5rem; font-weight: 700; color: var(--c-navy); margin-bottom: 1rem; }
.reg-benefits { list-style: none; display: flex; flex-direction: column; gap: 10px; margin-top: 1.5rem; }
.reg-benefits li {
  display: flex; align-items: flex-start; gap: 10px;
  font-size: 0.9rem; color: #374151;
}
.reg-benefits li::before { content: '✦'; color: var(--c-gold); font-size: 0.8rem; margin-top: 3px; flex-shrink: 0; }
.reg-deadline {
  margin-top: 2rem;
  background: var(--c-navy);
  border-radius: 12px; padding: 1.2rem 1.5rem;
  color: white;
}
.reg-deadline .d-label { font-size: 0.8rem; text-transform: uppercase; letter-spacing: 1px; color: rgba(255,255,255,0.6); }
.reg-deadline .d-date { font-family: var(--font-display); font-size: 1.5rem; font-weight: 700; color: var(--c-gold); }
.reg-form {
  background: var(--c-cream);
  border-radius: 20px;
  padding: 2.5rem;
  border: 1px solid rgba(0,0,0,0.06);
}
.reg-form h3 { font-weight: 700; font-size: 1.2rem; color: var(--c-navy); margin-bottom: 1.5rem; }
.form-group { margin-bottom: 1.2rem; }
.form-group label { display: block; font-size: 0.85rem; font-weight: 600; color: #374151; margin-bottom: 6px; }
.form-group input, .form-group select, .form-group textarea {
  width: 100%;
  background: white;
  border: 1.5px solid #E5E7EB;
  border-radius: 10px;
  padding: 11px 14px;
  font-family: var(--font-body);
  font-size: 0.9rem;
  color: var(--c-text);
  outline: none;
  transition: border-color 0.2s;
}
.form-group input:focus, .form-group select:focus, .form-group textarea:focus {
  border-color: var(--c-gold);
  box-shadow: 0 0 0 3px rgba(201,151,58,0.1);
}
.form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
.form-submit {
  width: 100%;
  background: var(--c-navy);
  color: white;
  border: none;
  padding: 14px;
  border-radius: 10px;
  font-family: var(--font-body);
  font-size: 1rem; font-weight: 700;
  cursor: pointer;
  transition: all 0.25s;
  margin-top: 8px;
}
.form-submit:hover { background: #1A4FAF; transform: translateY(-1px); }
.form-note { font-size: 0.78rem; color: var(--c-gray); text-align: center; margin-top: 10px; }

/* ── NEWS ── */
.news { background: var(--c-cream); }
.news-grid {
  display: grid; grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
  gap: 1.5rem;
}
.news-card {
  background: white;
  border-radius: 16px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.06);
  transition: all 0.3s;
}
.news-card:hover { transform: translateY(-4px); box-shadow: var(--shadow); }
.news-img {
  aspect-ratio: 16/9;
  background: linear-gradient(135deg, var(--c-navy) 0%, #1A4FAF 100%);
  display: flex; align-items: center; justify-content: center;
  font-size: 2.5rem;
}
.news-body { padding: 1.5rem; }
.news-date { font-size: 0.8rem; color: var(--c-gold); font-weight: 600; margin-bottom: 8px; }
.news-title { font-weight: 700; color: var(--c-navy); font-size: 1rem; margin-bottom: 8px; line-height: 1.4; }
.news-excerpt { font-size: 0.85rem; color: var(--c-gray); line-height: 1.6; }
.news-link { display: inline-block; margin-top: 12px; font-size: 0.85rem; font-weight: 600; color: var(--c-blue); text-decoration: none; }
.news-link:hover { color: var(--c-gold); }

/* ── GALLERY ── */
.gallery { background: white; }
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-template-rows: auto;
  gap: 12px;
}
.gallery-item {
  border-radius: 12px; overflow: hidden;
  aspect-ratio: 1;
  background: linear-gradient(135deg, var(--c-navy), #1A4FAF);
  display: flex; align-items: center; justify-content: center;
  font-size: 2.5rem; cursor: pointer;
  transition: transform 0.3s;
  position: relative;
}
.gallery-item:hover { transform: scale(1.02); }
.gallery-item:nth-child(1) { grid-column: span 2; aspect-ratio: auto; height: 220px; }
.gallery-item-label {
  position: absolute; bottom: 10px; left: 10px; right: 10px;
  background: rgba(11,30,61,0.7);
  border-radius: 8px; padding: 6px 10px;
  color: white; font-size: 0.78rem;
  backdrop-filter: blur(4px);
}

/* ── PARTNERS ── */
.partners { background: var(--c-cream); padding: 4rem 1.5rem; }
.partners-inner { max-width: 1000px; margin: 0 auto; text-align: center; }
.partners-title { font-size: 0.85rem; font-weight: 600; letter-spacing: 2px; text-transform: uppercase; color: var(--c-gray); margin-bottom: 2rem; }
.partners-logos {
  display: flex; flex-wrap: wrap; gap: 1.5rem;
  align-items: center; justify-content: center;
}
.partner-logo {
  background: white; border: 1px solid #E5E7EB;
  border-radius: 12px; padding: 14px 24px;
  font-size: 0.9rem; font-weight: 700;
  color: var(--c-navy);
  display: flex; align-items: center; gap: 8px;
  min-width: 130px; justify-content: center;
}

/* ── FAQ ── */
.faq { background: white; }
.faq-list { max-width: 760px; margin: 0 auto; }
.faq-item {
  border-bottom: 1px solid var(--c-gray-light);
}
.faq-question {
  width: 100%; background: none; border: none; cursor: pointer;
  font-family: var(--font-body);
  font-size: 0.98rem; font-weight: 600; color: var(--c-navy);
  text-align: left;
  padding: 1.3rem 0;
  display: flex; align-items: center; justify-content: space-between; gap: 1rem;
  transition: color 0.2s;
}
.faq-question:hover { color: var(--c-gold); }
.faq-arrow { font-size: 1.2rem; transition: transform 0.3s; flex-shrink: 0; }
.faq-answer {
  font-size: 0.9rem; color: var(--c-gray);
  line-height: 1.7;
  max-height: 0; overflow: hidden;
  transition: max-height 0.35s ease, padding 0.35s ease;
}
.faq-item.open .faq-answer { max-height: 300px; padding-bottom: 1rem; }
.faq-item.open .faq-arrow { transform: rotate(180deg); }

/* ── CONTACTS ── */
.contacts { background: var(--c-navy); }
.contacts-grid {
  display: grid; grid-template-columns: 1fr 1fr; gap: 4rem; align-items: start;
}
.contacts .section-title { color: white; }
.contacts .section-subtitle { color: rgba(255,255,255,0.65); }
.contact-list { margin-top: 2rem; display: flex; flex-direction: column; gap: 1rem; }
.contact-item {
  display: flex; align-items: center; gap: 12px;
  color: rgba(255,255,255,0.8); font-size: 0.9rem;
}
.contact-icon {
  width: 40px; height: 40px;
  background: rgba(201,151,58,0.15);
  border-radius: 10px;
  display: flex; align-items: center; justify-content: center;
  font-size: 18px; flex-shrink: 0;
}
.contact-item a { color: var(--c-gold); text-decoration: none; }
.contact-item a:hover { text-decoration: underline; }
.social-row { display: flex; gap: 10px; margin-top: 1.5rem; }
.social-btn {
  width: 42px; height: 42px;
  background: rgba(255,255,255,0.1);
  border-radius: 10px;
  display: flex; align-items: center; justify-content: center;
  font-size: 1.1rem; text-decoration: none; color: white;
  transition: background 0.2s;
}
.social-btn:hover { background: var(--c-gold); }
.contact-map-placeholder {
  background: rgba(255,255,255,0.05);
  border: 1px solid rgba(255,255,255,0.1);
  border-radius: 20px;
  padding: 3rem 2rem;
  text-align: center; color: rgba(255,255,255,0.7);
}
.map-icon { font-size: 3rem; margin-bottom: 1rem; }
.map-address { font-size: 0.9rem; line-height: 1.6; color: rgba(255,255,255,0.6); }

/* ── FOOTER ── */
footer {
  background: #060F1E;
  padding: 3rem 1.5rem 2rem;
  color: rgba(255,255,255,0.5);
}
.footer-inner { max-width: 1200px; margin: 0 auto; }
.footer-top {
  display: grid; grid-template-columns: 2fr 1fr 1fr; gap: 3rem;
  padding-bottom: 2rem; border-bottom: 1px solid rgba(255,255,255,0.08);
  margin-bottom: 2rem;
}
.footer-brand p { font-size: 0.85rem; line-height: 1.7; color: rgba(255,255,255,0.5); margin-top: 1rem; max-width: 280px; }
.footer-col h4 { font-size: 0.85rem; font-weight: 700; color: white; margin-bottom: 1rem; letter-spacing: 0.5px; }
.footer-col ul { list-style: none; display: flex; flex-direction: column; gap: 7px; }
.footer-col ul a { font-size: 0.83rem; color: rgba(255,255,255,0.5); text-decoration: none; transition: color 0.2s; }
.footer-col ul a:hover { color: var(--c-gold); }
.footer-bottom { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 1rem; font-size: 0.8rem; }
.footer-bottom a { color: rgba(255,255,255,0.4); text-decoration: none; }

/* ── SUCCESS MODAL ── */
.modal-overlay {
  display: none; position: fixed; inset: 0; z-index: 200;
  background: rgba(0,0,0,0.6); align-items: center; justify-content: center;
  padding: 1rem;
}
.modal-overlay.show { display: flex; }
.modal-box {
  background: white; border-radius: 20px;
  padding: 3rem; text-align: center;
  max-width: 420px; width: 100%;
}
.modal-icon { font-size: 4rem; margin-bottom: 1rem; }
.modal-box h3 { font-family: var(--font-display); font-size: 1.5rem; color: var(--c-navy); margin-bottom: 0.5rem; }
.modal-box p { color: var(--c-gray); font-size: 0.9rem; margin-bottom: 1.5rem; }
.modal-close {
  background: var(--c-navy); color: white;
  border: none; border-radius: 10px; padding: 12px 28px;
  font-family: var(--font-body); font-size: 0.9rem; font-weight: 600;
  cursor: pointer;
}

/* ── RESPONSIVE ── */
@media (max-width: 900px) {
  .hero-inner { grid-template-columns: 1fr; gap: 3rem; text-align: center; }
  .hero-meta { justify-content: center; }
  .hero-actions { justify-content: center; }
  .about-grid, .reg-layout, .contacts-grid { grid-template-columns: 1fr; gap: 2.5rem; }
  .about-badge { bottom: -10px; right: 0; }
  .stats-grid { grid-template-columns: repeat(2, 1fr); }
  .footer-top { grid-template-columns: 1fr; gap: 2rem; }
  .gallery-grid { grid-template-columns: repeat(2, 1fr); }
  .gallery-item:nth-child(1) { grid-column: span 2; }
  .form-row { grid-template-columns: 1fr; }
}
@media (max-width: 640px) {
  .nav-links { display: none; }
  .nav-links.open { display: flex; flex-direction: column; position: absolute; top: 68px; left: 0; right: 0; background: rgba(11,30,61,0.98); padding: 1rem; gap: 0; border-bottom: 1px solid rgba(255,255,255,0.1); }
  .hamburger { display: flex; }
  section { padding: 4rem 1.2rem; }
  .stats-grid { grid-template-columns: repeat(2, 1fr); }
  .speakers-grid { grid-template-columns: repeat(2, 1fr); }
  .gallery-grid { grid-template-columns: 1fr; }
  .gallery-item:nth-child(1) { grid-column: 1; height: auto; }
  .hero-visual { display: none; }
}

/* ── ANIMATIONS ── */
.fade-up {
  opacity: 0; transform: translateY(30px);
  transition: opacity 0.6s ease, transform 0.6s ease;
}
.fade-up.visible { opacity: 1; transform: translateY(0); }
</style>
</head>
<body>

<!-- NAV -->
<nav class="nav" id="mainNav">
  <div class="nav-inner">
    <a href="#" class="nav-logo">
      <div class="nav-logo-badge">CA<br>EU</div>
      <div class="nav-logo-text">
        Youth Forum 2026
        <span>Samarkand, Uzbekistan</span>
      </div>
    </a>
    <button class="hamburger" id="hamburger" aria-label="Меню">
      <span></span><span></span><span></span>
    </button>
    <ul class="nav-links" id="navLinks">
      <li><a href="#about" data-ru="О форуме" data-en="About">О форуме</a></li>
      <li><a href="#program" data-ru="Программа" data-en="Program">Программа</a></li>
      <li><a href="#speakers" data-ru="Спикеры" data-en="Speakers">Спикеры</a></li>
      <li><a href="#news" data-ru="Новости" data-en="News">Новости</a></li>
      <li><a href="#contacts" data-ru="Контакты" data-en="Contacts">Контакты</a></li>
      <li><a href="#registration" class="nav-cta" data-ru="Регистрация" data-en="Register">Регистрация</a></li>
    </ul>
    <div class="nav-lang">
      <button class="active" onclick="setLang('ru')">RU</button>
      <button onclick="setLang('en')">EN</button>
    </div>
  </div>
</nav>

<!-- HERO -->
<section class="hero" id="home">
  <div class="hero-bg-pattern"></div>
  <div class="hero-stars"></div>
  <div class="hero-inner">
    <div class="hero-content">
      <div class="hero-eyebrow">
        <span class="hero-eyebrow-dot"></span>
        <span data-ru="Самарканд, Узбекистан · 13–14 Августа 2026" data-en="Samarkand, Uzbekistan · August 13–14, 2026">Самарканд, Узбекистан · 13–14 Августа 2026</span>
      </div>
      <h1 class="hero-title">
        <span data-ru="Центральноазиатско-" data-en="Central Asia –">Центральноазиатско-</span><br>
        <span class="accent" data-ru="Европейский" data-en="European Union">Европейский</span><br>
        <span data-ru="Молодёжный Форум" data-en="Youth Forum">Молодёжный Форум</span>
      </h1>
      <p class="hero-subtitle" data-ru="Площадка для диалога молодых лидеров Центральной Азии и Европейского Союза. Два дня дискуссий, нетворкинга и конкретных решений для будущего региона." data-en="A platform for dialogue between young leaders of Central Asia and the European Union. Two days of discussions, networking and concrete solutions for the future of the region.">
        Площадка для диалога молодых лидеров Центральной Азии и Европейского Союза. Два дня дискуссий, нетворкинга и конкретных решений для будущего региона.
      </p>
      <div class="hero-meta">
        <div class="hero-meta-item">
          <div class="hero-meta-icon">📍</div>
          <span data-ru="Самарканд, Узбекистан" data-en="Samarkand, Uzbekistan">Самарканд, Узбекистан</span>
        </div>
        <div class="hero-meta-item">
          <div class="hero-meta-icon">🗓</div>
          <span>13–14 August 2026</span>
        </div>
        <div class="hero-meta-item">
          <div class="hero-meta-icon">🌐</div>
          <span data-ru="6 стран" data-en="6 countries">6 стран</span>
        </div>
      </div>
      <div class="hero-actions">
        <a href="#registration" class="btn-primary" data-ru="Зарегистрироваться" data-en="Register Now">Зарегистрироваться</a>
        <a href="#program" class="btn-secondary" data-ru="Программа форума" data-en="View Program">Программа форума</a>
      </div>
    </div>
    <div class="hero-visual">
      <div class="hero-card-stack">
        <div class="hero-card">
          <div class="hero-card-flags">
            <div class="flag flag-uz"></div>
            <div class="flag flag-eu" style="color:#FFCC00;font-weight:700">EU</div>
            <div class="flag flag-kz"></div>
            <div class="flag flag-kg"></div>
            <div class="flag flag-tj"></div>
            <div class="flag flag-tm"></div>
          </div>
          <div class="hero-card-stat">
            <div class="num">300+</div>
            <div class="label" data-ru="участников из 6 стран" data-en="participants from 6 countries">участников из 6 стран</div>
          </div>
          <hr class="hero-card-divider">
          <div class="hero-card-dates">
            <div class="hero-date-box">
              <div class="day">13</div>
              <div class="month" data-ru="Август · День 1" data-en="August · Day 1">Август · День 1</div>
            </div>
            <div class="hero-date-box">
              <div class="day">14</div>
              <div class="month" data-ru="Август · День 2" data-en="August · Day 2">Август · День 2</div>
            </div>
          </div>
          <div class="countdown">
            <div class="countdown-label" data-ru="До начала форума" data-en="Until forum starts">До начала форума</div>
            <div class="countdown-nums">
              <div class="countdown-unit"><div class="n" id="cd-d">--</div><div class="l" data-ru="дней" data-en="days">дней</div></div>
              <div class="countdown-unit"><div class="n" id="cd-h">--</div><div class="l" data-ru="часов" data-en="hours">часов</div></div>
              <div class="countdown-unit"><div class="n" id="cd-m">--</div><div class="l" data-ru="минут" data-en="min">минут</div></div>
              <div class="countdown-unit"><div class="n" id="cd-s">--</div><div class="l" data-ru="секунд" data-en="sec">секунд</div></div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="hero-scroll">
    <div class="scroll-arrow"></div>
  </div>
  <svg class="hero-arc" viewBox="0 0 1440 60" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M0 60 C360 0 1080 0 1440 60 L1440 60 L0 60 Z" fill="#0B1E3D"/>
  </svg>
</section>

<!-- STATS -->
<div class="stats-bar">
  <div class="stats-grid">
    <div class="stat-item fade-up">
      <div class="stat-num">300+</div>
      <div class="stat-label" data-ru="Участников" data-en="Participants">Участников</div>
    </div>
    <div class="stat-item fade-up">
      <div class="stat-num">6</div>
      <div class="stat-label" data-ru="Стран-участниц" data-en="Participating Countries">Стран-участниц</div>
    </div>
    <div class="stat-item fade-up">
      <div class="stat-num">20+</div>
      <div class="stat-label" data-ru="Спикеров и экспертов" data-en="Speakers & Experts">Спикеров и экспертов</div>
    </div>
    <div class="stat-item fade-up">
      <div class="stat-num">2</div>
      <div class="stat-label" data-ru="Дня интенсивной работы" data-en="Days of Intensive Work">Дня интенсивной работы</div>
    </div>
  </div>
</div>

<!-- ABOUT -->
<section class="about" id="about">
  <div class="section-inner">
    <div class="about-grid">
      <div class="about-image-block">
        <div class="about-img-placeholder">
          <div class="about-img-text">
            <div class="big">🏛</div>
            <p data-ru="Самарканд — жемчужина Центральной Азии" data-en="Samarkand — Pearl of Central Asia">Самарканд — жемчужина Центральной Азии</p>
          </div>
        </div>
        <div class="about-badge">
          <div class="b-num">2026</div>
          <div class="b-label" data-ru="Год проведения" data-en="Forum Year">Год проведения</div>
        </div>
      </div>
      <div>
        <div class="section-label" data-ru="О ФОРУМЕ" data-en="ABOUT">О ФОРУМЕ</div>
        <h2 class="section-title" data-ru="Мост между двумя регионами" data-en="A Bridge Between Two Regions">Мост между двумя регионами</h2>
        <p class="section-subtitle" data-ru="CA–EU Youth Forum — ежегодная международная платформа для молодых лидеров до 35 лет из стран Центральной Азии и Европейского Союза. Форум создаёт пространство для обмена опытом, совместной работы и формирования нового поколения лидеров." data-en="CA–EU Youth Forum is an annual international platform for young leaders under 35 from Central Asian countries and the European Union. The forum creates space for experience sharing, collaborative work and shaping the next generation of leaders.">
          CA–EU Youth Forum — ежегодная международная платформа для молодых лидеров до 35 лет из стран Центральной Азии и Европейского Союза. Форум создаёт пространство для обмена опытом, совместной работы и формирования нового поколения лидеров.
        </p>
        <div class="about-features">
          <div class="feature-item">
            <div class="feature-icon">🎯</div>
            <div class="feature-text">
              <h4 data-ru="Диалог и дипломатия" data-en="Dialogue & Diplomacy">Диалог и дипломатия</h4>
              <p data-ru="Площадка для открытого обсуждения ключевых вопросов сотрудничества ЦА и ЕС." data-en="A platform for open discussion of key CA-EU cooperation issues.">Площадка для открытого обсуждения ключевых вопросов сотрудничества ЦА и ЕС.</p>
            </div>
          </div>
          <div class="feature-item">
            <div class="feature-icon">🚀</div>
            <div class="feature-text">
              <h4 data-ru="Нетворкинг и карьера" data-en="Networking & Career">Нетворкинг и карьера</h4>
              <p data-ru="Встречи с топ-экспертами, дипломатами и молодыми профессионалами из 6+ стран." data-en="Meetings with top experts, diplomats and young professionals from 6+ countries.">Встречи с топ-экспертами, дипломатами и молодыми профессионалами из 6+ стран.</p>
            </div>
          </div>
          <div class="feature-item">
            <div class="feature-icon">📚</div>
            <div class="feature-text">
              <h4 data-ru="Воркшопы и обучение" data-en="Workshops & Training">Воркшопы и обучение</h4>
              <p data-ru="Практические сессии по лидерству, публичной политике, устойчивому развитию." data-en="Practical sessions on leadership, public policy, and sustainable development.">Практические сессии по лидерству, публичной политике, устойчивому развитию.</p>
            </div>
          </div>
          <div class="feature-item">
            <div class="feature-icon">🏆</div>
            <div class="feature-text">
              <h4 data-ru="Гранты и стипендии" data-en="Grants & Scholarships">Гранты и стипендии</h4>
              <p data-ru="Стипендиальная программа для лучших участников. Покрытие проезда и проживания." data-en="Scholarship program for the best participants. Travel and accommodation covered.">Стипендиальная программа для лучших участников. Покрытие проезда и проживания.</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- PROGRAM -->
<section class="program" id="program">
  <div class="section-inner">
    <div class="text-center" style="margin-bottom:3rem">
      <div class="section-label" data-ru="ПРОГРАММА" data-en="PROGRAM">ПРОГРАММА</div>
      <h2 class="section-title" data-ru="Два дня насыщенной программы" data-en="Two Days of Intensive Program">Два дня насыщенной программы</h2>
    </div>
    <div class="program-tabs">
      <button class="tab-btn active" onclick="switchDay(1)" id="tab1" data-ru="13 августа — День 1" data-en="August 13 — Day 1">13 августа — День 1</button>
      <button class="tab-btn" onclick="switchDay(2)" id="tab2" data-ru="14 августа — День 2" data-en="August 14 — Day 2">14 августа — День 2</button>
    </div>
    <div class="program-day active" id="day1">
      <div class="program-timeline">
        <div class="program-item">
          <div class="program-time">09:00</div>
          <div class="program-content">
            <span class="program-tag tag-break" data-ru="Регистрация" data-en="Registration">Регистрация</span>
            <h4 data-ru="Регистрация участников и приветственный кофе" data-en="Participant registration and welcome coffee">Регистрация участников и приветственный кофе</h4>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">10:00</div>
          <div class="program-content">
            <span class="program-tag tag-keynote" data-ru="Пленарная сессия" data-en="Plenary">Пленарная сессия</span>
            <h4 data-ru="Торжественное открытие форума" data-en="Solemn Opening Ceremony">Торжественное открытие форума</h4>
            <p data-ru="Приветственные слова официальных лиц ЕС и Узбекистана, представление программы." data-en="Welcome speeches from EU and Uzbekistan officials, program introduction.">Приветственные слова официальных лиц ЕС и Узбекистана, представление программы.</p>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">11:30</div>
          <div class="program-content">
            <span class="program-tag tag-keynote" data-ru="Keynote" data-en="Keynote">Keynote</span>
            <h4 data-ru="ЦА и ЕС: новое измерение партнёрства" data-en="CA & EU: A New Dimension of Partnership">ЦА и ЕС: новое измерение партнёрства</h4>
            <p data-ru="Ключевая лекция о перспективах сотрудничества двух регионов в 2026–2030 гг." data-en="Key lecture on prospects for cooperation between the two regions in 2026–2030.">Ключевая лекция о перспективах сотрудничества двух регионов в 2026–2030 гг.</p>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">13:00</div>
          <div class="program-content">
            <span class="program-tag tag-break">🍽 Break</span>
            <h4 data-ru="Обед и неформальный нетворкинг" data-en="Lunch & Informal Networking">Обед и неформальный нетворкинг</h4>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">14:30</div>
          <div class="program-content">
            <span class="program-tag tag-panel" data-ru="Панель" data-en="Panel">Панель</span>
            <h4 data-ru="Молодёжь и зелёная трансформация" data-en="Youth & Green Transformation">Молодёжь и зелёная трансформация</h4>
            <p data-ru="Дискуссия с экспертами по климату и устойчивому развитию." data-en="Discussion with climate and sustainable development experts.">Дискуссия с экспертами по климату и устойчивому развитию.</p>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">16:00</div>
          <div class="program-content">
            <span class="program-tag tag-workshop" data-ru="Воркшоп" data-en="Workshop">Воркшоп</span>
            <h4 data-ru="Параллельные рабочие группы" data-en="Parallel Working Groups">Параллельные рабочие группы</h4>
            <p data-ru="Цифровая экономика · Устойчивое развитие · Молодёжная политика" data-en="Digital Economy · Sustainable Development · Youth Policy">Цифровая экономика · Устойчивое развитие · Молодёжная политика</p>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">19:00</div>
          <div class="program-content">
            <span class="program-tag tag-networking" data-ru="Нетворкинг" data-en="Networking">Нетворкинг</span>
            <h4 data-ru="Культурный вечер в Самарканде" data-en="Cultural Evening in Samarkand">Культурный вечер в Самарканде</h4>
            <p data-ru="Приём для участников с элементами национальной культуры Узбекистана." data-en="Reception for participants with elements of Uzbek national culture.">Приём для участников с элементами национальной культуры Узбекистана.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="program-day" id="day2">
      <div class="program-timeline">
        <div class="program-item">
          <div class="program-time">09:30</div>
          <div class="program-content">
            <span class="program-tag tag-keynote">Keynote</span>
            <h4 data-ru="Цифровая дипломатия и молодёжь" data-en="Digital Diplomacy & Youth">Цифровая дипломатия и молодёжь</h4>
            <p data-ru="Как технологии меняют международные отношения." data-en="How technology is transforming international relations.">Как технологии меняют международные отношения.</p>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">11:00</div>
          <div class="program-content">
            <span class="program-tag tag-workshop" data-ru="Воркшоп" data-en="Workshop">Воркшоп</span>
            <h4 data-ru="Лидерство и публичные коммуникации" data-en="Leadership & Public Communications">Лидерство и публичные коммуникации</h4>
            <p data-ru="Практическая сессия с известными медиа-тренерами и политиками." data-en="Practical session with well-known media trainers and politicians.">Практическая сессия с известными медиа-тренерами и политиками.</p>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">13:00</div>
          <div class="program-content">
            <span class="program-tag tag-break">🍽 Break</span>
            <h4 data-ru="Обед" data-en="Lunch">Обед</h4>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">14:00</div>
          <div class="program-content">
            <span class="program-tag tag-panel" data-ru="Панель" data-en="Panel">Панель</span>
            <h4 data-ru="Самаркандская декларация молодёжи" data-en="Samarkand Youth Declaration">Самаркандская декларация молодёжи</h4>
            <p data-ru="Презентация рекомендаций рабочих групп, голосование и принятие итогового документа." data-en="Presentation of working group recommendations, vote and adoption of the final document.">Презентация рекомендаций рабочих групп, голосование и принятие итогового документа.</p>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">16:00</div>
          <div class="program-content">
            <span class="program-tag tag-keynote" data-ru="Закрытие" data-en="Closing">Закрытие</span>
            <h4 data-ru="Торжественное закрытие и вручение сертификатов" data-en="Closing Ceremony & Certificate Presentation">Торжественное закрытие и вручение сертификатов</h4>
          </div>
        </div>
        <div class="program-item">
          <div class="program-time">17:30</div>
          <div class="program-content">
            <span class="program-tag tag-networking" data-ru="Нетворкинг" data-en="Networking">Нетворкинг</span>
            <h4 data-ru="Экскурсия по историческому центру Самарканда" data-en="Tour of Samarkand's Historical Center">Экскурсия по историческому центру Самарканда</h4>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- SPEAKERS -->
<section class="speakers" id="speakers">
  <div class="section-inner">
    <div class="text-center" style="margin-bottom:3rem">
      <div class="section-label" data-ru="СПИКЕРЫ" data-en="SPEAKERS">СПИКЕРЫ</div>
      <h2 class="section-title" data-ru="Эксперты и лидеры мнений" data-en="Experts & Opinion Leaders">Эксперты и лидеры мнений</h2>
      <p class="section-subtitle" data-ru="Более 20 спикеров из Центральной Азии, Европейского Союза и международных организаций." data-en="More than 20 speakers from Central Asia, the European Union and international organizations.">Более 20 спикеров из Центральной Азии, Европейского Союза и международных организаций.</p>
    </div>
    <div class="speakers-grid">
      <div class="speaker-card">
        <div class="speaker-photo">🎓</div>
        <div class="speaker-body">
          <div class="speaker-name">Dr. Anna Kowalski</div>
          <div class="speaker-role" data-ru="Директор по внешним связям ЕС" data-en="Director of EU External Relations">Директор по внешним связям ЕС</div>
          <div class="speaker-country">🇪🇺 <span data-ru="Европейский Союз" data-en="European Union">Европейский Союз</span></div>
        </div>
      </div>
      <div class="speaker-card">
        <div class="speaker-photo" style="background: linear-gradient(135deg,#1eb6e8,#003399)">🏛</div>
        <div class="speaker-body">
          <div class="speaker-name" data-ru="Акбар Тошматов" data-en="Akbar Toshmatov">Акбар Тошматов</div>
          <div class="speaker-role" data-ru="Заместитель министра молодёжи УЗ" data-en="Deputy Minister of Youth, UZ">Заместитель министра молодёжи УЗ</div>
          <div class="speaker-country">🇺🇿 <span data-ru="Узбекистан" data-en="Uzbekistan">Узбекистан</span></div>
        </div>
      </div>
      <div class="speaker-card">
        <div class="speaker-photo" style="background: linear-gradient(135deg,#00AFCA,#0B1E3D)">💡</div>
        <div class="speaker-body">
          <div class="speaker-name">Prof. Mira Seitkali</div>
          <div class="speaker-role" data-ru="Эксперт по климатической политике" data-en="Climate Policy Expert">Эксперт по климатической политике</div>
          <div class="speaker-country">🇰🇿 <span data-ru="Казахстан" data-en="Kazakhstan">Казахстан</span></div>
        </div>
      </div>
      <div class="speaker-card">
        <div class="speaker-photo" style="background: linear-gradient(135deg,#E8112D,#600010)">🌍</div>
        <div class="speaker-body">
          <div class="speaker-name">Tobias Ehrmann</div>
          <div class="speaker-role" data-ru="Директор фонда EU-CA Relations" data-en="Director, EU-CA Relations Foundation">Директор фонда EU-CA Relations</div>
          <div class="speaker-country">🇩🇪 <span data-ru="Германия" data-en="Germany">Германия</span></div>
        </div>
      </div>
      <div class="speaker-card">
        <div class="speaker-photo" style="background: linear-gradient(135deg,#30A956,#0B1E3D)">📊</div>
        <div class="speaker-body">
          <div class="speaker-name" data-ru="Гульнора Рашидова" data-en="Gulnora Rashidova">Гульнора Рашидова</div>
          <div class="speaker-role" data-ru="Исследователь, ПРООН Узбекистан" data-en="Researcher, UNDP Uzbekistan">Исследователь, ПРООН Узбекистан</div>
          <div class="speaker-country">🇺🇿 <span data-ru="Узбекистан" data-en="Uzbekistan">Узбекистан</span></div>
        </div>
      </div>
      <div class="speaker-card">
        <div class="speaker-photo" style="background: linear-gradient(135deg,#C30017,#3B0009)">🎤</div>
        <div class="speaker-body">
          <div class="speaker-name">Ainur Bekova</div>
          <div class="speaker-role" data-ru="Молодёжный активист, TEDx Speaker" data-en="Youth Activist, TEDx Speaker">Молодёжный активист, TEDx Speaker</div>
          <div class="speaker-country">🇰🇬 <span data-ru="Кыргызстан" data-en="Kyrgyzstan">Кыргызстан</span></div>
        </div>
      </div>
    </div>
    <div style="text-align:center;margin-top:2.5rem">
      <p style="color:var(--c-gray);font-size:0.9rem;margin-bottom:1rem" data-ru="Полный список спикеров будет объявлен в июне 2026" data-en="Full list of speakers to be announced in June 2026">Полный список спикеров будет объявлен в июне 2026</p>
    </div>
  </div>
</section>

<!-- REGISTRATION -->
<section class="registration" id="registration">
  <div class="section-inner">
    <div class="reg-layout">
      <div class="reg-info fade-up">
        <div class="section-label" data-ru="РЕГИСТРАЦИЯ" data-en="REGISTRATION">РЕГИСТРАЦИЯ</div>
        <h2 class="section-title" data-ru="Стань участником форума" data-en="Become a Forum Participant">Стань участником форума</h2>
        <p class="section-subtitle" data-ru="Форум открыт для молодых лидеров от 18 до 35 лет из стран Центральной Азии и ЕС. Участие бесплатное для отобранных кандидатов." data-en="The forum is open to young leaders aged 18-35 from Central Asian countries and the EU. Participation is free for selected candidates.">
          Форум открыт для молодых лидеров от 18 до 35 лет из стран Центральной Азии и ЕС. Участие бесплатное для отобранных кандидатов.
        </p>
        <ul class="reg-benefits">
          <li data-ru="Бесплатное участие в двухдневной программе" data-en="Free participation in the two-day program">Бесплатное участие в двухдневной программе</li>
          <li data-ru="Официальный сертификат участника" data-en="Official participation certificate">Официальный сертификат участника</li>
          <li data-ru="Возможность получить стипендию (проезд + проживание)" data-en="Opportunity to receive a scholarship (travel + accommodation)">Возможность получить стипендию (проезд + проживание)</li>
          <li data-ru="Нетворкинг с лидерами из 6 стран" data-en="Networking with leaders from 6 countries">Нетворкинг с лидерами из 6 стран</li>
          <li data-ru="Культурная программа в Самарканде" data-en="Cultural program in Samarkand">Культурная программа в Самарканде</li>
          <li data-ru="Рекомендательные письма от организаторов" data-en="Recommendation letters from organizers">Рекомендательные письма от организаторов</li>
        </ul>
        <div class="reg-deadline">
          <div class="d-label" data-ru="Дедлайн подачи заявок" data-en="Application Deadline">Дедлайн подачи заявок</div>
          <div class="d-date">30 июня 2026</div>
        </div>
      </div>
      <div class="reg-form fade-up">
        <h3 data-ru="Подать заявку" data-en="Apply Now">Подать заявку</h3>
        <div class="form-row">
          <div class="form-group">
            <label data-ru="Имя *" data-en="First Name *">Имя *</label>
            <input type="text" id="firstName" placeholder="Иван" required>
          </div>
          <div class="form-group">
            <label data-ru="Фамилия *" data-en="Last Name *">Фамилия *</label>
            <input type="text" id="lastName" placeholder="Иванов" required>
          </div>
        </div>
        <div class="form-group">
          <label data-ru="Email *" data-en="Email *">Email *</label>
          <input type="email" id="email" placeholder="ivan@example.com" required>
        </div>
        <div class="form-row">
          <div class="form-group">
            <label data-ru="Страна *" data-en="Country *">Страна *</label>
            <select id="country" required>
              <option value="" data-ru="Выберите страну" data-en="Select country">Выберите страну</option>
              <option data-ru="Узбекистан" data-en="Uzbekistan">Узбекистан</option>
              <option data-ru="Казахстан" data-en="Kazakhstan">Казахстан</option>
              <option data-ru="Кыргызстан" data-en="Kyrgyzstan">Кыргызстан</option>
              <option data-ru="Таджикистан" data-en="Tajikistan">Таджикистан</option>
              <option data-ru="Туркменистан" data-en="Turkmenistan">Туркменистан</option>
              <option data-ru="Страна ЕС" data-en="EU Country">Страна ЕС</option>
            </select>
          </div>
          <div class="form-group">
            <label data-ru="Возраст *" data-en="Age *">Возраст *</label>
            <input type="number" id="age" min="18" max="35" placeholder="25">
          </div>
        </div>
        <div class="form-group">
          <label data-ru="Организация / Университет" data-en="Organization / University">Организация / Университет</label>
          <input type="text" id="org" placeholder="Ташкентский Государственный Университет">
        </div>
        <div class="form-group">
          <label data-ru="Мотивационное письмо (до 500 слов) *" data-en="Motivation Letter (up to 500 words) *">Мотивационное письмо (до 500 слов) *</label>
          <textarea id="motivation" rows="4" style="resize:vertical" placeholder="Расскажите, почему вы хотите участвовать..."></textarea>
        </div>
        <div class="form-group" style="display:flex;align-items:flex-start;gap:10px">
          <input type="checkbox" id="agree" style="width:auto;margin-top:3px">
          <label for="agree" style="font-size:0.82rem;font-weight:400;color:var(--c-gray)" data-ru="Я согласен(а) с политикой обработки персональных данных" data-en="I agree to the personal data processing policy">Я согласен(а) с политикой обработки персональных данных</label>
        </div>
        <button class="form-submit" onclick="submitForm()" data-ru="Отправить заявку →" data-en="Submit Application →">Отправить заявку →</button>
        <p class="form-note" data-ru="Результаты отбора будут направлены на email до 15 июля 2026" data-en="Selection results will be sent by email by July 15, 2026">Результаты отбора будут направлены на email до 15 июля 2026</p>
      </div>
    </div>
  </div>
</section>

<!-- NEWS -->
<section class="news" id="news">
  <div class="section-inner">
    <div style="display:flex;justify-content:space-between;align-items:flex-end;margin-bottom:3rem;flex-wrap:wrap;gap:1rem">
      <div>
        <div class="section-label" data-ru="НОВОСТИ" data-en="NEWS">НОВОСТИ</div>
        <h2 class="section-title" data-ru="Актуальные новости" data-en="Latest News">Актуальные новости</h2>
      </div>
      <a href="#" style="font-size:0.9rem;font-weight:600;color:var(--c-blue);text-decoration:none" data-ru="Все новости →" data-en="All news →">Все новости →</a>
    </div>
    <div class="news-grid">
      <div class="news-card">
        <div class="news-img">📰</div>
        <div class="news-body">
          <div class="news-date">12 мая 2026</div>
          <h3 class="news-title" data-ru="Открыта регистрация на CA–EU Youth Forum 2026" data-en="Registration open for CA–EU Youth Forum 2026">Открыта регистрация на CA–EU Youth Forum 2026</h3>
          <p class="news-excerpt" data-ru="Принимаются заявки от молодых лидеров из 6 стран. Дедлайн — 30 июня 2026 года." data-en="Applications are being accepted from young leaders from 6 countries. Deadline — June 30, 2026.">Принимаются заявки от молодых лидеров из 6 стран. Дедлайн — 30 июня 2026 года.</p>
          <a href="#" class="news-link" data-ru="Читать далее →" data-en="Read more →">Читать далее →</a>
        </div>
      </div>
      <div class="news-card">
        <div class="news-img">🤝</div>
        <div class="news-body">
          <div class="news-date">28 апреля 2026</div>
          <h3 class="news-title" data-ru="Делегация ЕС посетила Самарканд для подготовки форума" data-en="EU Delegation Visited Samarkand to Prepare for Forum">Делегация ЕС посетила Самарканд для подготовки форума</h3>
          <p class="news-excerpt" data-ru="Переговоры о логистике и программе форума состоялись в Самарканде с участием местных партнёров." data-en="Negotiations on the logistics and program of the forum took place in Samarkand with the participation of local partners.">Переговоры о логистике и программе форума состоялись в Самарканде с участием местных партнёров.</p>
          <a href="#" class="news-link" data-ru="Читать далее →" data-en="Read more →">Читать далее →</a>
        </div>
      </div>
      <div class="news-card">
        <div class="news-img">🌱</div>
        <div class="news-body">
          <div class="news-date">15 апреля 2026</div>
          <h3 class="news-title" data-ru="Объявлена тема форума 2026: «Зелёный переход и молодёжь»" data-en="Forum 2026 Theme Announced: 'Green Transition & Youth'">Объявлена тема форума 2026: «Зелёный переход и молодёжь»</h3>
          <p class="news-excerpt" data-ru="Основная тема форума посвящена роли молодёжи в переходе к устойчивой экономике в регионе." data-en="The main theme of the forum is dedicated to the role of youth in the transition to a sustainable economy in the region.">Основная тема форума посвящена роли молодёжи в переходе к устойчивой экономике в регионе.</p>
          <a href="#" class="news-link" data-ru="Читать далее →" data-en="Read more →">Читать далее →</a>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- GALLERY -->
<section class="gallery" id="gallery">
  <div class="section-inner">
    <div class="text-center" style="margin-bottom:3rem">
      <div class="section-label" data-ru="ГАЛЕРЕЯ" data-en="GALLERY">ГАЛЕРЕЯ</div>
      <h2 class="section-title" data-ru="Форум в лицах" data-en="Forum in Pictures">Форум в лицах</h2>
    </div>
    <div class="gallery-grid">
      <div class="gallery-item" style="background:linear-gradient(135deg,#0B1E3D,#1A4FAF)">
        🎤
        <div class="gallery-item-label" data-ru="Пленарная сессия 2025" data-en="Plenary Session 2025">Пленарная сессия 2025</div>
      </div>
      <div class="gallery-item" style="background:linear-gradient(135deg,#1A4FAF,#0B2D4A)">🤝</div>
      <div class="gallery-item" style="background:linear-gradient(135deg,#C9973A,#8B6914)">🌟</div>
      <div class="gallery-item" style="background:linear-gradient(135deg,#0B2D4A,#0B1E3D)">📸</div>
      <div class="gallery-item" style="background:linear-gradient(135deg,#1eb6e8,#003399)">🌍</div>
      <div class="gallery-item" style="background:linear-gradient(135deg,#30A956,#0B1E3D)">🏛</div>
    </div>
    <div style="text-align:center;margin-top:2rem">
      <a href="#" class="btn-primary" style="display:inline-block" data-ru="Все фотографии →" data-en="All Photos →">Все фотографии →</a>
    </div>
  </div>
</section>

<!-- PARTNERS -->
<div class="partners">
  <div class="partners-inner">
    <div class="partners-title" data-ru="ОРГАНИЗАТОРЫ И ПАРТНЁРЫ" data-en="ORGANIZERS & PARTNERS">ОРГАНИЗАТОРЫ И ПАРТНЁРЫ</div>
    <div class="partners-logos">
      <div class="partner-logo">🇪🇺 European Union</div>
      <div class="partner-logo">🇺🇿 Узбекистан</div>
      <div class="partner-logo">🌐 UNDP</div>
      <div class="partner-logo">📚 UNESCO</div>
      <div class="partner-logo">🤝 OSCE</div>
      <div class="partner-logo">🌱 GIZ</div>
    </div>
  </div>
</div>

<!-- FAQ -->
<section class="faq" id="faq">
  <div class="section-inner">
    <div class="text-center" style="margin-bottom:3rem">
      <div class="section-label">FAQ</div>
      <h2 class="section-title" data-ru="Часто задаваемые вопросы" data-en="Frequently Asked Questions">Часто задаваемые вопросы</h2>
    </div>
    <div class="faq-list">
      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span data-ru="Кто может подать заявку на форум?" data-en="Who can apply to the forum?">Кто может подать заявку на форум?</span>
          <span class="faq-arrow">▼</span>
        </button>
        <div class="faq-answer" data-ru="Форум открыт для молодых лидеров от 18 до 35 лет из Узбекистана, Казахстана, Кыргызстана, Таджикистана, Туркменистана и стран Европейского Союза. Приветствуются студенты, молодые специалисты, НКО-активисты и предприниматели." data-en="The forum is open to young leaders aged 18-35 from Uzbekistan, Kazakhstan, Kyrgyzstan, Tajikistan, Turkmenistan and EU member states. Students, young professionals, NGO activists and entrepreneurs are welcome.">
          Форум открыт для молодых лидеров от 18 до 35 лет из Узбекистана, Казахстана, Кыргызстана, Таджикистана, Туркменистана и стран Европейского Союза. Приветствуются студенты, молодые специалисты, НКО-активисты и предприниматели.
        </div>
      </div>
      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span data-ru="Сколько стоит участие?" data-en="How much does participation cost?">Сколько стоит участие?</span>
          <span class="faq-arrow">▼</span>
        </button>
        <div class="faq-answer" data-ru="Участие в форуме бесплатное для всех отобранных участников. Дополнительно лучшие кандидаты могут получить стипендию, покрывающую проезд и проживание в Самарканде." data-en="Forum participation is free for all selected participants. Additionally, the best candidates can receive a scholarship covering travel and accommodation in Samarkand.">
          Участие в форуме бесплатное для всех отобранных участников. Дополнительно лучшие кандидаты могут получить стипендию, покрывающую проезд и проживание в Самарканде.
        </div>
      </div>
      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span data-ru="На каком языке проходит форум?" data-en="What language is the forum conducted in?">На каком языке проходит форум?</span>
          <span class="faq-arrow">▼</span>
        </button>
        <div class="faq-answer" data-ru="Рабочие языки форума — русский и английский. Синхронный перевод будет доступен на пленарных сессиях." data-en="The working languages of the forum are Russian and English. Simultaneous interpretation will be available at plenary sessions.">
          Рабочие языки форума — русский и английский. Синхронный перевод будет доступен на пленарных сессиях.
        </div>
      </div>
      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span data-ru="Как узнать результаты отбора?" data-en="How to find out the selection results?">Как узнать результаты отбора?</span>
          <span class="faq-arrow">▼</span>
        </button>
        <div class="faq-answer" data-ru="Результаты отбора будут направлены на адрес электронной почты, указанный в заявке, не позднее 15 июля 2026 года. Все заявители получат уведомление вне зависимости от результата." data-en="Selection results will be sent to the email address provided in the application no later than July 15, 2026. All applicants will receive notification regardless of the outcome.">
          Результаты отбора будут направлены на адрес электронной почты, указанный в заявке, не позднее 15 июля 2026 года. Все заявители получат уведомление вне зависимости от результата.
        </div>
      </div>
      <div class="faq-item">
        <button class="faq-question" onclick="toggleFaq(this)">
          <span data-ru="Нужна ли виза для участия?" data-en="Is a visa required to participate?">Нужна ли виза для участия?</span>
          <span class="faq-arrow">▼</span>
        </button>
        <div class="faq-answer" data-ru="Гражданам большинства стран ЕС виза для въезда в Узбекистан не требуется (безвизовый режим или e-Visa). Организаторы помогут с оформлением официальных приглашений при необходимости." data-en="Citizens of most EU countries do not need a visa to enter Uzbekistan (visa-free or e-Visa). Organizers will help with official invitations if needed.">
          Гражданам большинства стран ЕС виза для въезда в Узбекистан не требуется (безвизовый режим или e-Visa). Организаторы помогут с оформлением официальных приглашений при необходимости.
        </div>
      </div>
    </div>
  </div>
</section>

<!-- CONTACTS -->
<section class="contacts" id="contacts">
  <div class="section-inner">
    <div class="contacts-grid">
      <div>
        <div class="section-label" style="color:var(--c-gold)" data-ru="КОНТАКТЫ" data-en="CONTACTS">КОНТАКТЫ</div>
        <h2 class="section-title" data-ru="Свяжитесь с нами" data-en="Get in Touch">Свяжитесь с нами</h2>
        <p class="section-subtitle" data-ru="Есть вопросы? Мы рады помочь. Напишите нам — мы ответим в течение 24 часов." data-en="Have questions? We're happy to help. Write to us — we'll respond within 24 hours.">
          Есть вопросы? Мы рады помочь. Напишите нам — мы ответим в течение 24 часов.
        </p>
        <div class="contact-list">
          <div class="contact-item">
            <div class="contact-icon">📧</div>
            <div><a href="mailto:info@cayouthforum.uz">info@cayouthforum.uz</a></div>
          </div>
          <div class="contact-item">
            <div class="contact-icon">📞</div>
            <div>+998 71 000 00 00</div>
          </div>
          <div class="contact-item">
            <div class="contact-icon">📍</div>
            <div data-ru="Самарканд, Узбекистан · Конференц-зал отеля Silk Road" data-en="Samarkand, Uzbekistan · Silk Road Hotel Conference Hall">Самарканд, Узбекистан · Конференц-зал отеля Silk Road</div>
          </div>
        </div>
        <div class="social-row">
          <a href="#" class="social-btn" title="Telegram">✈</a>
          <a href="#" class="social-btn" title="Instagram">📷</a>
          <a href="#" class="social-btn" title="LinkedIn">💼</a>
          <a href="#" class="social-btn" title="Facebook">👥</a>
        </div>
      </div>
      <div class="contact-map-placeholder">
        <div class="map-icon">🗺</div>
        <p style="color:white;font-weight:600;margin-bottom:8px" data-ru="Место проведения" data-en="Venue">Место проведения</p>
        <div class="map-address" data-ru="Отель «Шёлковый путь»<br>пр. Ислама Каримова, 1<br>Самарканд, Узбекистан 140100<br><br>Конференц-центр · 2-й этаж<br>Залы A, B, C" data-en="Silk Road Hotel<br>1 Islam Karimov Ave<br>Samarkand, Uzbekistan 140100<br><br>Conference Center · 2nd Floor<br>Halls A, B, C">
          Отель «Шёлковый путь»<br>пр. Ислама Каримова, 1<br>Самарканд, Узбекистан 140100<br><br>Конференц-центр · 2-й этаж<br>Залы A, B, C
        </div>
        <a href="https://maps.google.com/?q=Samarkand,Uzbekistan" target="_blank" class="btn-secondary" style="margin-top:1.5rem;display:inline-block;font-size:0.85rem" data-ru="Открыть в Google Maps →" data-en="Open in Google Maps →">Открыть в Google Maps →</a>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-inner">
    <div class="footer-top">
      <div class="footer-brand">
        <div style="display:flex;align-items:center;gap:10px;margin-bottom:0.5rem">
          <div style="width:36px;height:36px;background:var(--c-gold);border-radius:6px;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:700;color:var(--c-navy)">CA<br>EU</div>
          <span style="color:white;font-weight:600;font-size:1rem">Youth Forum 2026</span>
        </div>
        <p data-ru="Центральноазиатско-Европейский молодёжный форум — ежегодная международная площадка для молодых лидеров двух регионов." data-en="Central Asia–European Union Youth Forum is an annual international platform for young leaders from two regions.">Центральноазиатско-Европейский молодёжный форум — ежегодная международная площадка для молодых лидеров двух регионов.</p>
      </div>
      <div class="footer-col">
        <h4 data-ru="Навигация" data-en="Navigation">Навигация</h4>
        <ul>
          <li><a href="#about" data-ru="О форуме" data-en="About">О форуме</a></li>
          <li><a href="#program" data-ru="Программа" data-en="Program">Программа</a></li>
          <li><a href="#speakers" data-ru="Спикеры" data-en="Speakers">Спикеры</a></li>
          <li><a href="#news" data-ru="Новости" data-en="News">Новости</a></li>
          <li><a href="#gallery" data-ru="Галерея" data-en="Gallery">Галерея</a></li>
        </ul>
      </div>
      <div class="footer-col">
        <h4 data-ru="Участие" data-en="Participation">Участие</h4>
        <ul>
          <li><a href="#registration" data-ru="Регистрация" data-en="Registration">Регистрация</a></li>
          <li><a href="#faq" data-ru="FAQ" data-en="FAQ">FAQ</a></li>
          <li><a href="#contacts" data-ru="Контакты" data-en="Contacts">Контакты</a></li>
          <li><a href="#" data-ru="Политика конфиденциальности" data-en="Privacy Policy">Политика конфиденциальности</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      <span>© 2026 CA–EU Youth Forum. <span data-ru="Все права защищены." data-en="All rights reserved.">Все права защищены.</span></span>
      <span data-ru="Самарканд, Узбекистан" data-en="Samarkand, Uzbekistan">🇺🇿 Самарканд, Узбекистан</span>
    </div>
  </div>
</footer>

<!-- SUCCESS MODAL -->
<div class="modal-overlay" id="successModal">
  <div class="modal-box">
    <div class="modal-icon">✅</div>
    <h3 data-ru="Заявка отправлена!" data-en="Application Sent!">Заявка отправлена!</h3>
    <p data-ru="Спасибо за заявку! Результаты отбора будут направлены на ваш email до 15 июля 2026 года." data-en="Thank you for your application! Selection results will be sent to your email by July 15, 2026.">Спасибо за заявку! Результаты отбора будут направлены на ваш email до 15 июля 2026 года.</p>
    <button class="modal-close" onclick="document.getElementById('successModal').classList.remove('show')" data-ru="Закрыть" data-en="Close">Закрыть</button>
  </div>
</div>

<script>
// ── COUNTDOWN ──
function updateCountdown() {
  const target = new Date('2026-08-13T09:00:00+05:00');
  const now = new Date();
  const diff = target - now;
  if (diff <= 0) { document.getElementById('cd-d').textContent='00'; return; }
  const d = Math.floor(diff/86400000);
  const h = Math.floor((diff%86400000)/3600000);
  const m = Math.floor((diff%3600000)/60000);
  const s = Math.floor((diff%60000)/1000);
  document.getElementById('cd-d').textContent = String(d).padStart(2,'0');
  document.getElementById('cd-h').textContent = String(h).padStart(2,'0');
  document.getElementById('cd-m').textContent = String(m).padStart(2,'0');
  document.getElementById('cd-s').textContent = String(s).padStart(2,'0');
}
updateCountdown(); setInterval(updateCountdown,1000);

// ── LANG SWITCH ──
let currentLang = 'ru';
function setLang(lang) {
  currentLang = lang;
  document.querySelectorAll('[data-ru]').forEach(el => {
    const text = el.getAttribute('data-'+lang);
    if (text) el.innerHTML = text;
  });
  document.querySelectorAll('.nav-lang button').forEach(b => b.classList.remove('active'));
  event.target.classList.add('active');
}

// ── PROGRAM TABS ──
function switchDay(n) {
  document.querySelectorAll('.program-day').forEach(d => d.classList.remove('active'));
  document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
  document.getElementById('day'+n).classList.add('active');
  document.getElementById('tab'+n).classList.add('active');
}

// ── FAQ ──
function toggleFaq(btn) {
  const item = btn.closest('.faq-item');
  const wasOpen = item.classList.contains('open');
  document.querySelectorAll('.faq-item').forEach(i => i.classList.remove('open'));
  if (!wasOpen) item.classList.add('open');
}

// ── FORM ──
function submitForm() {
  const firstName = document.getElementById('firstName').value;
  const email = document.getElementById('email').value;
  const agree = document.getElementById('agree').checked;
  if (!firstName || !email) {
    alert(currentLang==='ru' ? 'Заполните обязательные поля' : 'Please fill in required fields');
    return;
  }
  if (!agree) {
    alert(currentLang==='ru' ? 'Необходимо согласиться с политикой конфиденциальности' : 'Please agree to the privacy policy');
    return;
  }
  document.getElementById('successModal').classList.add('show');
}

// ── HAMBURGER ──
document.getElementById('hamburger').addEventListener('click', function() {
  document.getElementById('navLinks').classList.toggle('open');
});

// ── SCROLL ANIMATIONS ──
const observer = new IntersectionObserver(entries => {
  entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('visible'); });
}, { threshold: 0.15 });
document.querySelectorAll('.fade-up').forEach(el => observer.observe(el));

// ── NAV ACTIVE ──
window.addEventListener('scroll', function() {
  const nav = document.getElementById('mainNav');
  if (window.scrollY > 50) nav.style.background='rgba(11,30,61,0.98)';
  else nav.style.background='rgba(11,30,61,0.95)';
});

// close modal on overlay click
document.getElementById('successModal').addEventListener('click', function(e) {
  if (e.target === this) this.classList.remove('show');
});
</script>
</body>
</html>
