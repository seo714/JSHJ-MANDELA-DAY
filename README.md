
<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Rights & Dignity — Human Rights Awareness</title>
    <meta name="description" content="Stories, data, and actions to improve awareness of human rights, with a focus on gender equality in developing regions." />
    <link rel="icon" href="/favicon.ico" />
    <style>
        :root {
            --bg: #ffffff;
            --text: #1f2937;
            --muted: #6b7280;
            --line: #e5e7eb;
            --accent: #2563eb;
            --accent-ghost: #eff6ff;
            --radius: 14px
        }

        * {
            box-sizing: border-box
        }

        body {
            margin: 0;
            font-family: Inter,system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial;
            line-height: 1.6;
            color: var(--text);
            background: var(--bg)
        }

        a {
            color: var(--accent);
            text-decoration: none
        }

            a:hover {
                text-decoration: underline
            }

        /* Layout */
        .container {
            max-width: 1040px;
            margin: 0 auto;
            padding: 24px
        }

        header {
            border-bottom: 1px solid var(--line);
            background: #fff;
            position: sticky;
            top: 0;
            z-index: 10
        }

        nav {
            display: flex;
            align-items: center;
            justify-content: space-between
        }

        .brand {
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: 700
        }

        .logo {
            width: 28px;
            height: 28px;
            border-radius: 8px;
            background: var(--accent)
        }

        .navlinks a {
            margin-left: 16px;
            color: #374151
        }

        .button {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            border: 1px solid var(--accent);
            color: #fff;
            background: var(--accent);
            border-radius: 999px;
            padding: 10px 14px;
            font-weight: 600
        }

            .button.ghost {
                background: var(--accent-ghost);
                color: var(--accent)
            }

        /* Hero */
        .hero-wrap {
            display: block
        }

        .hero {
            position: relative;
            min-height: 52vh;
            display: grid
        }

            .hero img {
                width: 100%;
                height: 52vh;
                object-fit: cover;
                border-bottom: 1px solid var(--line)
            }

        .hero-overlay {
            position: absolute;
            inset: 0;
            display: flex;
            align-items: center
        }

        .hero-content {
            max-width: 1040px;
            margin: 0 auto;
            padding: 24px
        }

        .hero-card {
            background: rgba(255,255,255,.96);
            backdrop-filter: saturate(1.1) blur(2px);
            border: 1px solid var(--line);
            border-radius: var(--radius);
            padding: 22px;
            box-shadow: 0 6px 22px rgba(0,0,0,.06)
        }

        h1 {
            font-size: 2.25rem;
            line-height: 1.2;
            margin: 0 0 8px
        }

        .lead {
            color: var(--muted);
            margin: 0 0 12px
        }

        /* Sections */
        .section {
            padding: 28px 0
        }

            .section h2 {
                font-size: 1.5rem;
                margin: 0 0 12px
            }

        .grid {
            display: grid;
            gap: 16px
        }

        .cards {
            grid-template-columns: repeat(auto-fit,minmax(260px,1fr))
        }

        .card {
            background: #fff;
            border: 1px solid var(--line);
            border-radius: var(--radius);
            padding: 18px
        }

        .meta {
            font-size: .9rem;
            color: var(--muted)
        }

        footer {
            border-top: 1px solid var(--line);
            color: var(--muted);
            font-size: .95rem
        }

        /* Accessibility helpers */
        .sr-only {
            position: absolute;
            width: 1px;
            height: 1px;
            padding: 0;
            margin: -1px;
            overflow: hidden;
            clip: rect(0,0,0,0);
            white-space: nowrap;
            border: 0
        }

        @media (max-width: 860px) {
            .hero img {
                height: 44vh
            }

            h1 {
                font-size: 1.9rem
            }
        }

        /* Optional subtle dark mode */
        @media (prefers-color-scheme: dark) {
            :root {
                --bg: #0b0e12;
                --text: #e5e7eb;
                --muted: #94a3b8;
                --line: #1f2937;
                --accent: #60a5fa;
                --accent-ghost: #0b1220
            }

            header, .card, .hero-card, footer {
                background: #0f141b
            }

            .navlinks a {
                color: #cbd5e1
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav aria-label="Primary">
                <div class="brand">
                    <div class="logo" aria-hidden="true"></div>
                    <span>Rights & Dignity</span>
                </div>
                <div class="navlinks">
                    <a href="#cases">Cases</a>
                    <a href="#learn">Learn</a>
                    <a href="#act">Act</a>
                    <a href="#about">About</a>
                    <button class="button ghost" onclick="toggleLang()" aria-label="Toggle language">🌐 <span id="lang-label">EN</span></button>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero with big image & project name -->
    <main class="container">
        <!-- CASE STUDIES -->
        <section id="cases" class="section">
            <h2>Case Studies</h2>
            <p class="meta">Keep it respectful, concise, and always cite sources (UN, WHO, World Bank, reputable NGOs, national statistics).</p>
            <div class="grid cards">
                <article class="card">
                    <h3>Example: Barriers to girls’ secondary education</h3>
                    <p class="meta">Country/Region • Year • <a href="#">Source</a></p>
                    <p>Summarize structural issues (law, access, safety, norms) in 3–4 sentences. Avoid sensational details.</p>
                </article>
                <article class="card">
                    <h3>Example: Legal reforms & enforcement gaps</h3>
                    <p class="meta">Country/Region • Year • <a href="#">Source</a></p>
                    <p>Explain what changed in law vs. practice; note data limits and context.</p>
                </article>
                <article class="card">
                    <h3>Example: Community-led safety initiatives</h3>
                    <p class="meta">City/Region • Year • <a href="#">Source</a></p>
                    <p>Describe program design, outcomes, and how to replicate ethically.</p>
                </article>
            </div>
        </section>

        <!-- LEARN -->
        <section id="learn" class="section">
            <h2>Learn</h2>
            <div class="grid cards">
                <div class="card">
                    <h3>Key Concepts</h3>
                    <ul>
                        <li>UDHR: Universal Declaration of Human Rights</li>
                        <li>CEDAW: Ending discrimination against women</li>
                        <li>Intersectionality & access to justice</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>Data Literacy</h3>
                    <ul>
                        <li>Read indicators carefully; check definitions</li>
                        <li>Under-reporting & survey limits</li>
                        <li>Context matters across regions</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>Ethical Guidelines</h3>
                    <ul>
                        <li>Dignity-first language; no victim-blaming</li>
                        <li>Consent & privacy for stories/images</li>
                        <li>Local voices and cultural sensitivity</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- ACT -->
        <section id="act" class="section">
            <h2>Take Action</h2>
            <div class="grid cards">
                <div class="card">
                    <h3>Learn & Share</h3>
                    <p>Download fact sheets, host a discussion at school, or share explainers.</p>
                    <button class="button" aria-label="Download fact sheet">Download PDF</button>
                </div>
                <div class="card">
                    <h3>Support</h3>
                    <p>Find reputable local NGOs and understand how donations are used.</p>
                    <a class="button" href="#">Find NGOs</a>
                </div>
                <div class="card">
                    <h3>Pledge</h3>
                    <form onsubmit="event.preventDefault(); alert('Thank you for pledging.');">
                        <label class="sr-only" for="email">Email</label>
                        <input id="email" type="email" placeholder="Email" required style="width:100%;padding:10px;border-radius:10px;border:1px solid var(--line);background:#fff;color:var(--text);margin:6px 0" />
                        <button class="button" type="submit">I Pledge to Learn & Act</button>
                    </form>
                </div>
            </div>
        </section>

        <!-- ABOUT -->
        <section id="about" class="section">
            <h2>About This Project</h2>
            <div class="card">
                <p>Student-led project to promote accurate, respectful human-rights awareness and practical action. Built with accessible web standards. Multilingual. Low-bandwidth friendly.</p>
                <p class="meta">We avoid explicit images and sensational language; focus stays on structures, rights, and solutions.</p>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div style="padding:18px 0">© <span id="year"></span> Rights & Dignity • <a href="#">Contact</a> • <a href="#">Privacy</a></div>
        </div>
    </footer>

    <script>
    // year
    document.getElementById('year').textContent = new Date().getFullYear();

    // simple i18n scaffold (EN/KR)
    const strings = {
      en: {
        title: 'Rights & Dignity',
        lead: 'A minimal, friendly site to share credible cases, context, and ways to support human rights—starting with gender equality.',
        lang: 'EN'
      },
      ko: {
        title: '권리와 존엄',
        lead: '신뢰할 수 있는 사례와 맥락을 바탕으로 인권(특히 성평등)에 대한 올바른 인식을 전하고, 실천으로 이어지도록 돕는 미니멀하고 친근한 사이트입니다.',
        lang: 'KR'
      }
    };
    let current = 'en';
    function toggleLang(){
      current = current === 'en' ? 'ko' : 'en';
      const s = strings[current];
      document.getElementById('hero-title').textContent = s.title;
      document.getElementById('hero-lead').textContent = s.lead;
      document.getElementById('lang-label').textContent = s.lang;
      document.documentElement.lang = current === 'en' ? 'en' : 'ko';
    }
    </script>
</body>
</html>
<!doctype html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Rights & Dignity — Human Rights Awareness</title>
    <meta name="description" content="Stories, data, and actions to improve awareness of human rights, with a focus on gender equality in developing regions." />
    <link rel="icon" href="/favicon.ico" />
    <style>
        :root {
            --bg: #ffffff;
            --text: #1f2937;
            --muted: #6b7280;
            --line: #e5e7eb;
            --accent: #2563eb;
            --accent-ghost: #eff6ff;
            --radius: 14px
        }

        * {
            box-sizing: border-box
        }

        body {
            margin: 0;
            font-family: Inter,system-ui,-apple-system,Segoe UI,Roboto,Helvetica,Arial;
            line-height: 1.6;
            color: var(--text);
            background: var(--bg)
        }

        a {
            color: var(--accent);
            text-decoration: none
        }

            a:hover {
                text-decoration: underline
            }

        /* Layout */
        .container {
            max-width: 1040px;
            margin: 0 auto;
            padding: 24px
        }

        header {
            border-bottom: 1px solid var(--line);
            background: #fff;
            position: sticky;
            top: 0;
            z-index: 10
        }

        nav {
            display: flex;
            align-items: center;
            justify-content: space-between
        }

        .brand {
            display: flex;
            align-items: center;
            gap: 10px;
            font-weight: 700
        }

        .logo {
            width: 28px;
            height: 28px;
            border-radius: 8px;
            background: var(--accent)
        }

        .navlinks a {
            margin-left: 16px;
            color: #374151
        }

        .button {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            border: 1px solid var(--accent);
            color: #fff;
            background: var(--accent);
            border-radius: 999px;
            padding: 10px 14px;
            font-weight: 600
        }

            .button.ghost {
                background: var(--accent-ghost);
                color: var(--accent)
            }

        /* Hero */
        .hero-wrap {
            display: block
        }

        .hero {
            position: relative;
            min-height: 52vh;
            display: grid
        }

            .hero img {
                width: 100%;
                height: 52vh;
                object-fit: cover;
                border-bottom: 1px solid var(--line)
            }

        .hero-overlay {
            position: absolute;
            inset: 0;
            display: flex;
            align-items: center
        }

        .hero-content {
            max-width: 1040px;
            margin: 0 auto;
            padding: 24px
        }

        .hero-card {
            background: rgba(255,255,255,.96);
            backdrop-filter: saturate(1.1) blur(2px);
            border: 1px solid var(--line);
            border-radius: var(--radius);
            padding: 22px;
            box-shadow: 0 6px 22px rgba(0,0,0,.06)
        }

        h1 {
            font-size: 2.25rem;
            line-height: 1.2;
            margin: 0 0 8px
        }

        .lead {
            color: var(--muted);
            margin: 0 0 12px
        }

        /* Sections */
        .section {
            padding: 28px 0
        }

            .section h2 {
                font-size: 1.5rem;
                margin: 0 0 12px
            }

        .grid {
            display: grid;
            gap: 16px
        }

        .cards {
            grid-template-columns: repeat(auto-fit,minmax(260px,1fr))
        }

        .card {
            background: #fff;
            border: 1px solid var(--line);
            border-radius: var(--radius);
            padding: 18px
        }

        .meta {
            font-size: .9rem;
            color: var(--muted)
        }

        footer {
            border-top: 1px solid var(--line);
            color: var(--muted);
            font-size: .95rem
        }

        /* Accessibility helpers */
        .sr-only {
            position: absolute;
            width: 1px;
            height: 1px;
            padding: 0;
            margin: -1px;
            overflow: hidden;
            clip: rect(0,0,0,0);
            white-space: nowrap;
            border: 0
        }

        @media (max-width: 860px) {
            .hero img {
                height: 44vh
            }

            h1 {
                font-size: 1.9rem
            }
        }

        /* Optional subtle dark mode */
        @media (prefers-color-scheme: dark) {
            :root {
                --bg: #0b0e12;
                --text: #e5e7eb;
                --muted: #94a3b8;
                --line: #1f2937;
                --accent: #60a5fa;
                --accent-ghost: #0b1220
            }

            header, .card, .hero-card, footer {
                background: #0f141b
            }

            .navlinks a {
                color: #cbd5e1
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <nav aria-label="Primary">
                <div class="brand">
                    <div class="logo" aria-hidden="true"></div>
                    <span>Rights & Dignity</span>
                </div>
                <div class="navlinks">
                    <a href="#cases">Cases</a>
                    <a href="#learn">Learn</a>
                    <a href="#act">Act</a>
                    <a href="#about">About</a>
                    <button class="button ghost" onclick="toggleLang()" aria-label="Toggle language">🌐 <span id="lang-label">EN</span></button>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero with big image & project name -->
    <div class="col-md-4 pt-5">
        <h2 class="h2 text-light border-bottom pb-3 border-light">teamates</h2>
        <ul class="list-unstyled text-light footer-link-list">
            <li><a class="text-light text-decoration-none" href="#">20702 강사라</a></li>
            <li><a class="text-light text-decoration-none" href="#">20711 김하연</a></li>
            <li><a class="text-light text-decoration-none" href="#">20713 민지유</a></li>
            <li><a class="text-light text-decoration-none" href="#">20723 이재서</a></li>
        </ul>
    </div>
    <div class="hero-wrap">
        <!-- Replace src with your own image file: hero.jpg (same folder) -->
        <div class="hero" role="img" aria-label="People walking together in a city market; community and dignity">
            <img src="hero.PNG" alt="Community scene representing dignity and equality" />
            <div class="hero-overlay">
                <div class="hero-content">
                    <div class="hero-card">
                        <h1 id="hero-title">Rights & Dignity</h1>
                        <p class="lead" id="hero-lead">A minimal, friendly site to share credible cases, context, and ways to support human rights—starting with gender equality.</p>
                        <div style="display:flex;gap:10px;flex-wrap:wrap">
                            <a class="button" href="#act">Get Involved</a>
                            <a class="button ghost" href="#cases">See Cases</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <main class="container">
        <!-- CASE STUDIES -->
        <section id="cases" class="section">
            <h2>Case Studies</h2>
            <p class="meta">Keep it respectful, concise, and always cite sources (UN, WHO, World Bank, reputable NGOs, national statistics).</p>
            <div class="grid cards">
                <article class="card">
                    <h3>Example: Barriers to girls’ secondary education</h3>
                    <p class="meta">Country/Region • Year • <a href="#">Source</a></p>
                    <p>Summarize structural issues (law, access, safety, norms) in 3–4 sentences. Avoid sensational details.</p>
                </article>
                <article class="card">
                    <h3>Example: Legal reforms & enforcement gaps</h3>
                    <p class="meta">Country/Region • Year • <a href="#">Source</a></p>
                    <p>Explain what changed in law vs. practice; note data limits and context.</p>
                </article>
                <article class="card">
                    <h3>Example: Community-led safety initiatives</h3>
                    <p class="meta">City/Region • Year • <a href="#">Source</a></p>
                    <p>Describe program design, outcomes, and how to replicate ethically.</p>
                </article>
            </div>
        </section>

        <!-- LEARN -->
        <section id="learn" class="section">
            <h2>Learn</h2>
            <div class="grid cards">
                <div class="card">
                    <h3>Key Concepts</h3>
                    <ul>
                        <li>UDHR: Universal Declaration of Human Rights</li>
                        <li>CEDAW: Ending discrimination against women</li>
                        <li>Intersectionality & access to justice</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>Data Literacy</h3>
                    <ul>
                        <li>Read indicators carefully; check definitions</li>
                        <li>Under-reporting & survey limits</li>
                        <li>Context matters across regions</li>
                    </ul>
                </div>
                <div class="card">
                    <h3>Ethical Guidelines</h3>
                    <ul>
                        <li>Dignity-first language; no victim-blaming</li>
                        <li>Consent & privacy for stories/images</li>
                        <li>Local voices and cultural sensitivity</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- ACT -->
        <section id="act" class="section">
            <h2>Take Action</h2>
            <div class="grid cards">
                <div class="card">
                    <h3>Learn & Share</h3>
                    <p>Download fact sheets, host a discussion at school, or share explainers.</p>
                    <button class="button" aria-label="Download fact sheet">Download PDF</button>
                </div>
                <div class="card">
                    <h3>Support</h3>
                    <p>Find reputable local NGOs and understand how donations are used.</p>
                    <a class="button" href="#">Find NGOs</a>
                </div>
                <div class="card">
                    <h3>Pledge</h3>
                    <form onsubmit="event.preventDefault(); alert('Thank you for pledging.');">
                        <label class="sr-only" for="email">Email</label>
                        <input id="email" type="email" placeholder="Email" required style="width:100%;padding:10px;border-radius:10px;border:1px solid var(--line);background:#fff;color:var(--text);margin:6px 0" />
                        <button class="button" type="submit">I Pledge to Learn & Act</button>
                    </form>
                </div>
            </div>
        </section>

        <!-- ABOUT -->
        <section id="about" class="section">
            <h2>About This Project</h2>
            <div class="card">
                <p>Student-led project to promote accurate, respectful human-rights awareness and practical action. Built with accessible web standards. Multilingual. Low-bandwidth friendly.</p>
                <p class="meta">We avoid explicit images and sensational language; focus stays on structures, rights, and solutions.</p>
                <h3>Team Members</h3>
                <ul class="list-unstyled">
                    <li>20702 강사라</li>
                    <li>20711 김하연</li>
                    <li>20713 민지유</li>
                    <li>20723 이재서</li>
                </ul>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div style="padding:18px 0">© <span id="year"></span> Rights & Dignity • <a href="#">Contact</a> • <a href="#">Privacy</a></div>
        </div>
    </footer>

    <script>
        // year
        document.getElementById('year').textContent = new Date().getFullYear();

        // simple i18n scaffold (EN/KR)
        const strings = {
            en: {
                title: 'Rights & Dignity',
                lead: 'A minimal, friendly site to share credible cases, context, and ways to support human rights—starting with gender equality.',
                lang: 'EN'
            },
            ko: {
                title: '권리와 존엄',
                lead: '신뢰할 수 있는 사례와 맥락을 바탕으로 인권(특히 성평등)에 대한 올바른 인식을 전하고, 실천으로 이어지도록 돕는 미니멀하고 친근한 사이트입니다.',
                lang: 'KR'
            }
        };
        let current = 'en';
        function toggleLang() {
            current = current === 'en' ? 'ko' : 'en';
            const s = strings[current];
            document.getElementById('hero-title').textContent = s.title;
            document.getElementById('hero-lead').textContent = s.lead;
            document.getElementById('lang-label').textContent = s.lang;
            document.documentElement.lang = current === 'en' ? 'en' : 'ko';
        }
    </script>
</body>
</html>
