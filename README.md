<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Human Rights in India — Awareness & Action</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <style>
/*

Tooplate 2141 Minimal White

https://www.tooplate.com/view/2141-minimal-white

*/

@charset "utf-8";

/* CSS Document */

 * {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
 }

 body {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  line-height: 1.6;
  color: #000;
  background: #fff;
  overflow-x: hidden;
  user-select: auto;
 }

 /* Decorative Elements */
 .black-line {
  width: 100%;
  height: 1px;
  background: #000;
  margin: 60px 0;
 }

 .black-block {
  width: 20px;
  height: 20px;
  background: #000;
  position: absolute;
 }

 .vertical-line {
  width: 1px;
  height: 100px;
  background: #000;
  margin: 40px auto;
 }

 /* Navigation */
 nav {
  position: fixed;
  top: 0;
  width: 100%;
  background: rgba(255, 255, 255, 0.98);
  backdrop-filter: blur(10px);
  z-index: 1000;
  padding: 20px 0;
  border-bottom: 2px solid #000;
  transition: all 0.3s ease;
 }

 nav.scrolled {
  padding: 15px 0;
  box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
 }

 .nav-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
 }

 .logo {
  font-size: 24px;
  font-weight: 700;
  letter-spacing: -1px;
  position: relative;
  color: #000;
  text-decoration: none;
 }

 .logo::after {
  content: '';
  position: absolute;
  right: -15px;
  top: 50%;
  transform: translateY(-50%);
  width: 8px;
  height: 8px;
  background: #000;
 }

 /* Hamburger Menu */
 .menu-toggle {
  display: none;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 30px;
  height: 30px;
  cursor: pointer;
  z-index: 1001;
 }

 .menu-toggle span {
  display: block;
  width: 25px;
  height: 2px;
  background: #000;
  margin: 3px 0;
  transition: all 0.3s ease;
 }

 .menu-toggle.active span:nth-child(1) {
  transform: rotate(45deg) translate(5px, 5px);
 }

 .menu-toggle.active span:nth-child(2) {
  opacity: 0;
 }

 .menu-toggle.active span:nth-child(3) {
  transform: rotate(-45deg) translate(7px, -6px);
 }

 .nav-links {
  display: flex;
  gap: 40px;
  list-style: none;
 }
 .nav-links a {
  color: #000;
  text-decoration: none;
  font-size: 13px;
  font-weight: 500;
  letter-spacing: 1px;
  transition: all 0.3s ease;
  position: relative;
 }

 .nav-links a::before {
  content: '';
  position: absolute;
  left: -15px;
  top: 50%;
  transform: translateY(-50%);
  width: 0;
  height: 1px;
  background: #000;
  transition: width 0.3s ease;
 }

 .nav-links a:hover::before,
 .nav-links a.active::before {
  width: 10px;
 }

 .nav-links a.active {
  font-weight: 700;
 }

 /* Section 1: Hero */
 .hero {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 80px 20px;
  position: relative;
  overflow: hidden;
 }

 .hero::before {
  content: '';
  position: absolute;
  top: 20%;
  left: 10%;
  width: 100px;
  height: 1px;
  background: #000;
  animation: slideRight 8s ease-in-out infinite;
 }

 .hero::after {
  content: '';
  position: absolute;
  bottom: 20%;
  right: 10%;
  width: 150px;
  height: 1px;
  background: #000;
  animation: slideLeft 8s ease-in-out infinite;
 }

 .hero-decoration {
  position: absolute;
  top: 30%;
  right: 15%;
  width: 40px;
  height: 40px;
  border: 2px solid #000;
  transform: rotate(45deg);
  animation: rotateSquare 10s linear infinite;
 }

 /* Animated Objects (Reduced) */
 .floating-objects {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  pointer-events: none;
  z-index: 1;
 }

 .floating-circle {
  position: absolute;
  width: 80px;
  height: 80px;
  border: 1px solid #000;
  border-radius: 50%;
  opacity: 0.2;
  animation: floatUp 18s ease-in-out infinite;
 }

 .floating-circle:nth-child(1) {
  left: 10%;
  bottom: -100px;
  animation-delay: 0s;
  width: 60px;
  height: 60px;
 }

 .floating-circle:nth-child(2) {
  right: 15%;
  bottom: -100px;
  animation-delay: 8s;
  width: 100px;
  height: 100px;
 }

 .floating-square {
  position: absolute;
  width: 30px;
  height: 30px;
  background: #000;
  opacity: 0.08;
  animation: floatDiagonal 25s linear infinite;
  top: 40%;
  left: -50px;
 }

 .floating-line {
  position: absolute;
  height: 1px;
  background: #000;
  opacity: 0.15;
  animation: expandContract 10s ease-in-out infinite;
  width: 200px;
  top: 65%;
  right: 10%;
  transform-origin: center;
 }

 .hero-content {
  text-align: center;
  max-width: 800px;
  animation: fadeInUp 1s ease;
  position: relative;
  z-index: 2;
 }

 /* Animations */
 @keyframes floatUp {
  0%, 100% {
   transform: translateY(0) scale(1);
   opacity: 0;
  }
  10% {
   opacity: 0.2;
  }
  50% {
   transform: translateY(-600px) scale(1.1);
   opacity: 0.05;
  }
  90% {
   opacity: 0;
  }
 }
 @keyframes floatDiagonal {
  0% {
   transform: translate(0, 0) rotate(0deg);
  }
  100% {
   transform: translate(1400px, -300px) rotate(360deg);
  }
 }

 @keyframes expandContract {
  0%, 100% {
   transform: scaleX(0.5) rotate(0deg);
  }
  50% {
   transform: scaleX(1.2) rotate(180deg);
  }
 }

 @keyframes rotateSquare {
  0% {
   transform: rotate(45deg) scale(1);
  }
  25% {
   transform: rotate(135deg) scale(1.1);
  }
  50% {
   transform: rotate(225deg) scale(1);
  }
  75% {
   transform: rotate(315deg) scale(0.9);
  }
  100% {
   transform: rotate(405deg) scale(1);
  }
 }

 @keyframes slideRight {
  0%, 100% {
   transform: translateX(0);
   opacity: 0.5;
  }
  50% {
   transform: translateX(50px);
   opacity: 1;
  }
 }

 @keyframes slideLeft {
  0%, 100% {
   transform: translateX(0);
   opacity: 0.5;
  }
  50% {
   transform: translateX(-50px);
   opacity: 1;
  }
 }

 .hero h1 {
  font-size: clamp(48px, 8vw, 88px);
  font-weight: 100;
  letter-spacing: -3px;
  margin-bottom: 30px;
  line-height: 0.9;
  position: relative;
 }

 .hero h1::after {
  content: '';
  position: absolute;
  bottom: -15px;
  left: 50%;
  transform: translateX(-50%);
  width: 60px;
  height: 2px;
  background: #000;
 }

 .hero .subtitle {
  font-size: 16px;
  color: #000;
  font-weight: 400;
  margin-bottom: 50px;
  letter-spacing: 2px;
  text-transform: uppercase;
 }

 .cta-button {
  display: inline-block;
  padding: 18px 50px;
  background: #000;
  color: #fff;
  text-decoration: none;
  font-size: 12px;
  letter-spacing: 2px;
  transition: all 0.3s ease;
  border: 2px solid #000;
  position: relative;
 }

 .cta-button::before {
  content: '';
  position: absolute;
  top: -10px;
  right: -10px;
  width: 20px;
  height: 20px;
  border-top: 2px solid #000;
  border-right: 2px solid #000;
 }

 .cta-button:hover {
  background: transparent;
  color: #000;
  transform: translate(-5px, -5px);
 }
 /* Section 2: About - Mixed Layouts */
 .about {
  padding: 120px 20px;
  background: #fff;
  position: relative;
 }

 .about::before {
  content: '';
  position: absolute;
  top: 50px;
  left: 0;
  width: 100%;
  height: 1px;
  background: #000;
 }

 .container {
  max-width: 1200px;
  margin: 0 auto;
 }

 /* Quote Block */
 .about-intro {
  margin-bottom: 80px;
 }

 .quote-block {
  max-width: 900px;
  margin: 0 auto;
  text-align: center;
  position: relative;
 }

 .quote-mark {
  font-size: 120px;
  line-height: 1;
  font-weight: 100;
  position: absolute;
  top: -40px;
  left: -60px;
  opacity: 0.1;
 }

 .quote-block h3 {
  font-size: 32px;
  font-weight: 300;
  line-height: 1.4;
  letter-spacing: -1px;
  margin-bottom: 30px;
 }

 .quote-author {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
 }

 .author-line {
  width: 50px;
  height: 1px;
  background: #000;
 }

 .quote-author p {
  font-size: 14px;
  letter-spacing: 1px;
  text-transform: uppercase;
  font-weight: 500;
 }

 /* Stats Grid */
 .stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2px;
  background: #000;
  padding: 2px;
  margin-bottom: 100px;
 }

 .stat-item {
  background: #fff;
  padding: 60px 20px;
  text-align: center;
  position: relative;
 }

 .stat-number {
  font-size: 48px;
  font-weight: 100;
  letter-spacing: -2px;
  margin-bottom: 10px;
 }

 .stat-label {
  font-size: 12px;
  letter-spacing: 2px;
  text-transform: uppercase;
  font-weight: 500;
 }

 .stat-decoration {
  position: absolute;
  top: 20px;
  right: 20px;
  width: 20px;
  height: 20px;
  border: 1px solid #000;
  transform: rotate(45deg);
 }
 /* Philosophy Section */
 .philosophy-section {
  display: grid;
  grid-template-columns: 300px 1fr;
  gap: 80px;
  margin-bottom: 100px;
  align-items: start;
 }

 .philosophy-header {
  position: relative;
 }

 .philosophy-header h2 {
  font-size: 64px;
  font-weight: 100;
  letter-spacing: -2px;
  writing-mode: vertical-rl;
  text-orientation: mixed;
 }

 .header-decoration {
  position: absolute;
  bottom: 0;
  right: -20px;
  width: 40px;
  height: 40px;
  background: #000;
 }

 .philosophy-content {
  padding-top: 40px;
 }

 .lead-text {
  font-size: 24px;
  line-height: 1.6;
  margin-bottom: 60px;
  font-weight: 300;
 }

 .philosophy-points {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 40px;
 }

 .point-item {
  position: relative;
  padding-left: 20px;
 }

 .point-number {
  position: absolute;
  left: 0;
  top: 0;
  font-size: 10px;
  font-weight: 700;
 }

 .point-item h4 {
  font-size: 16px;
  font-weight: 500;
  margin-bottom: 8px;
  letter-spacing: 0.5px;
 }

 .point-item p {
  font-size: 14px;
  color: #666;
  line-height: 1.6;
 }

 /* Process Timeline */
 .process-timeline {
  margin-bottom: 100px;
 }

 .section-subtitle {
  font-size: 48px;
  font-weight: 100;
  text-align: center;
  margin-bottom: 60px;
  letter-spacing: -1px;
 }

 .timeline-container {
  position: relative;
  display: flex;
  justify-content: space-between;
  max-width: 900px;
  margin: 0 auto;
 }

 .timeline-line {
  position: absolute;
  top: 20px;
  left: 0;
  right: 0;
  height: 2px;
  background: #000;
  z-index: 0;
 }

 .timeline-item {
  position: relative;
  text-align: center;
  flex: 1;
 }

 .timeline-dot {
  width: 40px;
  height: 40px;
  background: #fff;
  border: 2px solid #000;
  margin: 0 auto 30px;
  position: relative;
  z-index: 1;
  transition: all 0.3s ease;
 }

 .timeline-item:hover .timeline-dot {
  background: #000;
  transform: rotate(45deg);
 }

 .timeline-content h4 {
  font-size: 18px;
  font-weight: 500;
  margin-bottom: 8px;
  letter-spacing: 0.5px;
 }

 .timeline-content p {
  font-size: 14px;
  color: #666;
 }
 /* Values Grid */
 .values-section {
  text-align: center;
 }

 .values-header {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
  margin-bottom: 60px;
 }

 .values-header h2 {
  font-size: 48px;
  font-weight: 100;
  letter-spacing: -1px;
 }

 .black-square {
  width: 15px;
  height: 15px;
  background: #000;
 }

 .values-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0;
 }

 .value-card {
  padding: 60px 20px;
  border: 1px solid #000;
  transition: all 0.3s ease;
 }

 .value-card.black {
  background: #000;
  color: #fff;
 }

 .value-icon {
  font-size: 48px;
  font-weight: 100;
  margin-bottom: 20px;
 }

 .value-card h4 {
  font-size: 14px;
  letter-spacing: 2px;
  text-transform: uppercase;
  font-weight: 500;
 }

 .value-card:hover {
  transform: translateY(-10px);
 }

 .split-layout {
  display: grid;
  grid-template-columns: 1fr 2px 1fr;
  gap: 60px;
  align-items: center;
  margin-top: 80px;
 }

 .split-divider {
  width: 2px;
  height: 300px;
  background: #000;
  justify-self: center;
 }

 .split-left {
  text-align: right;
  padding-right: 20px;
 }

 .split-left h2 {
  font-size: 64px;
  font-weight: 100;
  letter-spacing: -2px;
  margin-bottom: 30px;
  position: relative;
 }

 .split-left h2::before {
  content: '';
  position: absolute;
  left: -40px;
  top: 50%;
  width: 30px;
  height: 30px;
  background: #000;
  transform: translateY(-50%);
 }

 .split-right {
  padding-left: 20px;
 }

 .split-right p {
  font-size: 18px;
  line-height: 2;
  margin-bottom: 30px;
 }

 .accent-box {
  display: inline-block;
  padding: 10px 20px;
  border: 1px solid #000;
  font-size: 12px;
  letter-spacing: 1px;
  text-transform: uppercase;
  position: relative;
 }

 .accent-box::after {
  content: '';
  position: absolute;
  bottom: -5px;
  right: -5px;
  width: 100%;
  height: 100%;
  background: #000;
  z-index: -1;
 }
 /* Section 3: Services - Asymmetric Grid */
 .services {
  padding: 120px 20px;
  background: #fafafa;
  position: relative;
 }

 .services::before,
 .services::after {
  content: '';
  position: absolute;
  width: 50px;
  height: 50px;
  border: 2px solid #000;
 }

 .services::before {
  top: 80px;
  left: 5%;
  animation: rotateSlowly 20s linear infinite;
 }

 .services::after {
  bottom: 80px;
  right: 5%;
  transform: rotate(45deg);
  animation: rotateSlowly 20s linear infinite reverse;
 }

 @keyframes rotateSlowly {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
 }

 .services-header {
  text-align: center;
  margin-bottom: 80px;
  position: relative;
 }

 .services-header h2 {
  font-size: 56px;
  font-weight: 100;
  letter-spacing: -1px;
  margin-bottom: 20px;
  position: relative;
  display: inline-block;
 }

 .services-header h2::before,
 .services-header h2::after {
  content: '';
  position: absolute;
  width: 30px;
  height: 1px;
  background: #000;
  top: 50%;
  transform: translateY(-50%);
 }

 .services-header h2::before {
  left: -50px;
 }

 .services-header h2::after {
  right: -50px;
 }

 .services-header::after {
  content: '';
  position: absolute;
  bottom: -30px;
  left: 50%;
  transform: translateX(-50%);
  width: 200px;
  height: 1px;
  background: linear-gradient(to right, transparent, #000 20%, #000 80%, transparent);
 }

 .asymmetric-grid {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 40px;
  margin-bottom: 40px;
  position: relative;
 }

 .asymmetric-grid.reverse {
  grid-template-columns: 1fr 2fr;
 }

 .service-large * {
  position: relative;
  z-index: 1;
 }

 .service-large {
  background: #fff;
  padding: 60px;
  border-left: 4px solid #000;
  position: relative;
  transition: all 0.4s cubic-bezier(0.25, 0.46, 0.45, 0.94);
  overflow: hidden;
 }

 .service-large::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.02);
  transition: left 0.6s ease;
  pointer-events: none;
 }

 .service-large:hover::before {
  left: 0;
 }

 .service-large::after {
  content: '';
  position: absolute;
  top: 40px;
  right: 40px;
  width: 15px;
  height: 15px;
  background: #000;
  transition: all 0.3s ease;
  pointer-events: none;
  z-index: 0;
 }

 .service-large:hover::after {
  transform: scale(1.5) rotate(45deg);
 }

 .service-large:hover {
  transform: translateX(10px);
  border-left-width: 8px;
 }

 .asymmetric-grid.reverse .service-large {
  border-left: none;
  border-right: 4px solid #000;
 }

 .asymmetric-grid.reverse .service-large::after {
  right: auto;
  left: 40px;
 }

 .asymmetric-grid.reverse .service-large:hover {
  transform: translateX(-10px);
  border-right-width: 8px;
 }
 .service-small {
  background: #000;
  color: #fff;
  padding: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  position: relative;
  overflow: hidden;
  transition: all 0.4s ease;
 }

 .service-small::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 0;
  height: 0;
  border: 1px solid rgba(255, 255, 255, 0.2);
  border-radius: 50%;
  transition: all 0.6s ease;
  pointer-events: none;
 }

 .service-small:hover::before {
  width: 200px;
  height: 200px;
 }

 .service-number {
  font-size: 88px;
  font-weight: 100;
  line-height: 1;
  margin-bottom: 20px;
  transition: all 0.3s ease;
  position: relative;
 }

 .service-small:hover .service-number {
  transform: scale(1.1);
 }

 .service-large h3,
 .service-large p {
  position: relative;
  z-index: 1;
  user-select: text;
 }

 .service-large h3 {
  font-size: 36px;
  font-weight: 300;
  margin-bottom: 20px;
  letter-spacing: -1px;
  display: inline-block;
 }

 .service-large h3::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 0;
  width: 0;
  height: 1px;
  background: #000;
  transition: width 0.3s ease;
 }

 .service-large:hover h3::after {
  width: 100%;
 }

 .service-large p {
  color: #666;
  line-height: 1.8;
  font-size: 16px;
  margin-bottom: 30px;
  user-select: text;
 }

 .service-tag {
  display: inline-block;
  padding: 8px 16px;
  border: 1px solid #000;
  font-size: 11px;
  letter-spacing: 1px;
  text-transform: uppercase;
  margin-top: 20px;
  transition: all 0.3s ease;
  cursor: pointer;
  position: relative;
  z-index: 1;
  text-decoration: none;
  color: #000;
 }

 .service-tag:hover {
  background: #000;
  color: #fff;
  transform: translateY(-2px);
 }

 /* Footer & Contact already in your CSS above (unchanged) */

 /* Accessibility - Reduced Motion */
 @media (prefers-reduced-motion: reduce) {
  * {
   animation: none !important;
   transition: none !important;
  }
 }
</style>
</head>
<body>

  <nav>
    <div class="nav-container">
      <a class="logo" href="#home">Rights&India</a>
      <div class="menu-toggle" id="menuToggle"><span></span><span></span><span></span></div>
      <ul class="nav-links" id="navLinks">
        <li><a class="active" href="#home">Home</a></li>
        <li><a href="#about">Overview</a></li>
        <li><a href="#philosophy">Principles</a></li>
        <li><a href="#process">Path</a></li>
        <li><a href="#values">Values</a></li>
        <li><a href="#services">Resources</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </nav>

  <section class="hero" id="home">
    <div class="floating-objects">
      <div class="floating-circle"></div>
      <div class="floating-circle"></div>
      <div class="floating-square"></div>
      <div class="floating-line"></div>
    </div>
    <div class="hero-decoration"></div>
    <div class="hero-content fade-in">
      <h1>Human Rights in India</h1>
      <p class="subtitle">Awareness · Dignity · Equality · Action</p>
      <a href="#about" class="cta-button">Learn the Issues</a>
    </div>
  </section>
  <section class="about" id="about">
    <div class="container">

      <div class="about-intro">
        <div class="quote-block">
          <div class="quote-mark">“</div>
          <h3>Every person deserves freedom, safety, and a fair chance to thrive. Building awareness is the first step; turning awareness into everyday action is the goal.</h3>
          <div class="quote-author">
            <div class="author-line"></div>
            <p>Community Pledge — Learn · Care · Act</p>
            <div class="author-line"></div>
          </div>
        </div>
      </div>

      <div class="stats-grid">
        <div class="stat-item">
          <div class="stat-decoration"></div>
          <div class="stat-number">Justice</div>
          <div class="stat-label">Rule of Law & Due Process</div>
        </div>
        <div class="stat-item">
          <div class="stat-decoration"></div>
          <div class="stat-number">Dignity</div>
          <div class="stat-label">Freedom from Discrimination</div>
        </div>
        <div class="stat-item">
          <div class="stat-decoration"></div>
          <div class="stat-number">Safety</div>
          <div class="stat-label">Protection from Violence</div>
        </div>
        <div class="stat-item">
          <div class="stat-decoration"></div>
          <div class="stat-number">Voice</div>
          <div class="stat-label">Expression & Participation</div>
        </div>
      </div>

      <div class="philosophy-section" id="philosophy">
        <div class="philosophy-header">
          <h2>Principles</h2>
          <div class="header-decoration"></div>
        </div>
        <div class="philosophy-content">
          <p class="lead-text">
            India’s Constitution enshrines equality, liberty, and dignity. Yet lived experiences vary across region, caste, class, gender, age, disability, religion, and sexuality. Our approach balances people-centered stories with evidence, focusing on practical, local action.
          </p>
          <div class="philosophy-points">
            <div class="point-item">
              <div class="point-number">01</div>
              <h4>Equality in Daily Life</h4>
              <p>Confront discrimination related to caste, gender, and religion in schools, workplaces, and public services. Promote inclusive language and fair opportunities.</p>
            </div>
            <div class="point-item">
              <div class="point-number">02</div>
              <h4>Safety & Bodily Autonomy</h4>
              <p>Address gender-based violence, child protection, and harassment. Support survivor-centered responses and access to medical, legal, and psychosocial help.</p>
            </div>
            <div class="point-item">
              <div class="point-number">03</div>
              <h4>Economic & Social Rights</h4>
              <p>Advance rights to education, health, sanitation, decent work, and a clean environment. Reduce barriers that keep marginalized communities from public benefits.</p>
            </div>
          </div>
        </div>
      </div>

      <div class="process-timeline" id="process">
        <h3 class="section-subtitle">Path from Awareness to Action</h3>
        <div class="timeline-container">
          <div class="timeline-line"></div>

          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <div class="timeline-content">
              <h4>Observe</h4>
              <p>Notice rights-related issues in your locality—access, safety, language, and behavior.</p>
            </div>
          </div>

          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <div class="timeline-content">
              <h4>Learn</h4>
              <p>Understand constitutional rights, due process, and anti-discrimination principles.</p>
            </div>
          </div>

          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <div class="timeline-content">
              <h4>Speak</h4>
              <p>Use respectful dialogue, report incidents, and amplify marginalized voices.</p>
            </div>
          </div>

          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <div class="timeline-content">
              <h4>Act</h4>
              <p>Support local initiatives, accessibility fixes, legal aid, and community monitoring.</p>
            </div>
          </div>

          <div class="timeline-item">
            <div class="timeline-dot"></div>
            <div class="timeline-content">
              <h4>Sustain</h4>
              <p>Track progress, share results, and build habits that normalize rights-respecting culture.</p>
            </div>
          </div>

        </div>
      </div>

      <div class="values-section" id="values">
        <div class="values-header">
          <div class="black-square"></div>
          <h2>Core Values</h2>
          <div class="black-square"></div>
        </div>

        <div class="values-grid">
          <div class="value-card"><div class="value-icon">A</div><h4>Accountability</h4></div>
          <div class="value-card black"><div class="value-icon">E</div><h4>Equity</h4></div>
          <div class="value-card"><div class="value-icon">D</div><h4>Dignity</h4></div>
          <div class="value-card black"><div class="value-icon">S</div><h4>Solidarity</h4></div>
        </div>

        <div class="split-layout">
          <div class="split-left">
            <h2>What’s at Stake</h2>
            <div class="accent-box">Rights are real when practiced daily</div>
          </div>
          <div class="split-divider"></div>
          <div class="split-right">
            <p>Gender equality must include safety, education, mobility, and economic opportunity. Ending caste-based exclusion requires inclusive policies and everyday allyship.</p>
            <p>Children deserve protection from labor, trafficking, and violence, with universal access to schooling and nutrition. Freedom of expression thrives where dialogue is safe and inclusive.</p>
          </div>
        </div>
      </div>

    </div>
  </section>
  <section class="services" id="services">
    <div class="container">
      <div class="="services-header">
        <h2>Awareness & Resources</h2>
        <p class="subtitle">Balanced approach: people-centered stories + practical tools</p>
      </div>

      <div class="asymmetric-grid">
        <div class="service-large">
          <h3>Understand the Landscape</h3>
          <p>Learn how rights relate to everyday issues—school access, sanitation, safe transport, digital safety, disability access, and workplace dignity. Compare policies and lived experiences.</p>
          <a class="service-tag" href="#about">Read Overview</a>
        </div>
        <div class="service-small"><div class="service-number">01</div><h4>Know your rights</h4></div>
      </div>

      <div class="asymmetric-grid reverse">
        <div class="service-small"><div class="service-number">02</div><h4>Support survivors</h4></div>
        <div class="service-large">
          <h3>Safety & Support</h3>
          <p>Encourage survivor-centered responses: confidentiality, non-judgmental listening, access to medical and legal support, and clear reporting pathways where safe and appropriate.</p>
          <a class="service-tag" href="#contact">Get Guidance</a>
        </div>
      </div>

      <div class="asymmetric-grid">
        <div class="service-large">
          <h3>Inclusive Schools & Workplaces</h3>
          <p>Promote anti-bullying, anti-harassment, and anti-discrimination practices. Ensure accessibility, menstrual health support, grievance redressal, and fair selection processes.</p>
          <a class="service-tag" href="#contact">Start a Checklist</a>
        </div>
        <div class="service-small"><div class="service-number">03</div><h4>Build inclusion</h4></div>
      </div>
    </div>
  </section>

  <section class="contact" id="contact">
    <div class="container">
      <div class="contact-grid">

        <div class="contact-info">
          <h2>Connect</h2>
          <div class="info-item"><h4>Purpose</h4><p>Share concerns, request workshops, or collaborate on local awareness campaigns.</p></div>
          <div class="info-item"><h4>Confidentiality</h4><p>We take privacy seriously. Share only what you feel safe to share.</p></div>
          <div class="info-item"><h4>Next Steps</h4><p>We’ll respond with learning materials, local referral options, and practical actions.</p></div>
        </div>

        <div class="contact-divider"></div>

        <div class="contact-form">
          <form>
            <div class="form-group">
              <select id="name" style="width:100%;padding:15px 0;border:none;border-bottom:2px solid #000;background:transparent;font-size:16px;">
                <option value="">Select Your Name</option>
                <option>강사라</option>
                <option>김하연</option>
                <option>민지유</option>
                <option>이재서</option>
              </select>
              <label for="name" style="top:-20px;font-size:11px;font-weight:500;">Your Name</label>
            </div>

            <div class="form-group">
              <input id="email" type="email" placeholder=" " />
              <label for="email">Email</label>
            </div>

            <div class="form-group">
              <textarea id="message" rows="5" placeholder=" "></textarea>
              <label for="message">Message (topic, city, any access needs)</label>
            </div>

            <button class="submit-btn" type="submit">Send</button>
          </form>
        </div>

      </div>
    </div>
  </section>

  <footer><p>© Human Rights in India — Learn · Care · Act</p></footer>

  <script>
    const menu = document.getElementById('menuToggle');
    const links = document.getElementById('navLinks');
    menu?.addEventListener('click', () => {
      menu.classList.toggle('active');
      links.classList.toggle('active');
    });
    window.addEventListener('scroll', () => {
      document.querySelector('nav')?.classList.toggle('scrolled', window.scrollY > 10);
    });
  </script>

</body>
</html>
