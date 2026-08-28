```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

:root {
    --primary: #2563eb;
    --primary-dark: #1d4ed8;
    --bg: #f8fafc;
    --card: #ffffff;
    --text: #0f172a;
    --muted: #64748b;
    --border: #e2e8f0;
    --header: rgba(255,255,255,.92);
    --soft: #eff6ff;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: var(--bg);
    color: var(--text);
    line-height: 1.6;
}

.container {
    width: min(1120px, 92%);
    margin: auto;
}


/* HEADER */

.header {
    position: sticky;
    top: 0;
    z-index: 100;
    background: var(--header);
    backdrop-filter: blur(12px);
    border-bottom: 1px solid var(--border);
}

.nav {
    height: 72px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    color: var(--text);
    text-decoration: none;
    font-size: 22px;
    font-weight: 800;
}

.menu {
    display: flex;
    gap: 25px;
}

.menu a {
    color: var(--muted);
    text-decoration: none;
    font-weight: 600;
}

.menu a:hover {
    color: var(--primary);
}

.theme-btn {
    width: 42px;
    height: 42px;
    border: 1px solid var(--border);
    border-radius: 50%;
    background: var(--card);
    cursor: pointer;
    font-size: 18px;
}


/* HERO */

.hero {
    padding: 90px 0;
    background:
        radial-gradient(circle at 90% 10%, #dbeafe, transparent 35%),
        radial-gradient(circle at 10% 90%, #e0e7ff, transparent 35%);
}

.hero-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 50px;
}

.hero-text {
    max-width: 680px;
}

.badge {
    display: inline-block;
    background: #dbeafe;
    color: var(--primary-dark);
    padding: 7px 14px;
    border-radius: 30px;
    font-size: 13px;
    font-weight: 800;
    margin-bottom: 20px;
}

.hero h1 {
    font-size: clamp(42px, 6vw, 70px);
    line-height: 1.05;
    margin-bottom: 25px;
}

.hero h1 span {
    color: var(--primary);
    display: block;
}

.hero p {
    color: var(--muted);
    font-size: 18px;
    max-width: 650px;
    margin-bottom: 30px;
}

.hero-buttons {
    display: flex;
    gap: 12px;
    flex-wrap: wrap;
}

.primary-btn,
.secondary-btn {
    display: inline-block;
    padding: 13px 20px;
    border-radius: 10px;
    text-decoration: none;
    font-weight: 700;
}

.primary-btn {
    background: var(--primary);
    color: white;
}

.primary-btn:hover {
    background: var(--primary-dark);
}

.secondary-btn {
    background: var(--card);
    color: var(--text);
    border: 1px solid var(--border);
}


/* HERO CARD */

.hero-card {
    width: 290px;
    min-width: 290px;
    padding: 40px 25px;
    text-align: center;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 25px;
    box-shadow: 0 20px 50px rgba(15,23,42,.08);
}

.book-icon {
    font-size: 65px;
}

.hero-card h3 {
    font-size: 28px;
}

.hero-card p {
    margin: 5px 0 20px;
}

.stats {
    display: flex;
    justify-content: center;
    gap: 35px;
    border-top: 1px solid var(--border);
    padding-top: 20px;
}

.stats strong {
    display: block;
    color: var(--primary);
    font-size: 20px;
}

.stats small {
    color: var(--muted);
}


/* SEARCH */

.search-section {
    padding: 30px 0 0;
}

.search-box {
    max-width: 700px;
    margin: auto;
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 4px 18px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 14px;
    box-shadow: 0 8px 30px rgba(15,23,42,.05);
}

.search-box span {
    font-size: 22px;
}

.search-box input {
    width: 100%;
    padding: 15px 5px;
    border: 0;
    outline: 0;
    background: transparent;
    color: var(--text);
    font-size: 16px;
}


/* SECTIONS */

.main-section,
.syllabus-section {
    padding: 75px 0;
}

.section-heading {
    text-align: center;
    margin-bottom: 40px;
}

.small-title {
    color: var(--primary);
    font-size: 12px;
    letter-spacing: 1.5px;
    font-weight: 800;
}

.section-heading h2 {
    font-size: 38px;
    margin: 8px 0;
}

.section-heading p {
    color: var(--muted);
}


/* SYLLABUS */

.syllabus-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
}

.syllabus-card {
    padding: 30px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 20px;
}

.syllabus-icon {
    font-size: 40px;
    margin-bottom: 10px;
}

.syllabus-card h3 {
    font-size: 22px;
    margin-bottom: 8px;
}

.syllabus-card p {
    color: var(--muted);
    margin-bottom: 18px;
}

.card-link {
    color: var(--primary);
    font-weight: 800;
    text-decoration: none;
    border: 0;
    background: none;
    cursor: pointer;
    font-size: 15px;
}

.syllabus-card.new {
    border-top: 4px solid var(--primary);
}

.syllabus-card.exam {
    border-top: 4px solid #f59e0b;
}


/* SUBJECTS */

.subject-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 18px;
}

.subject-card {
    display: flex;
    gap: 18px;
    padding: 24px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 18px;
    transition: .2s;
}

.subject-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 15px 35px rgba(15,23,42,.08);
    border-color: #93c5fd;
}

.subject-icon {
    width: 62px;
    height: 62px;
    min-width: 62px;
    display: grid;
    place-items: center;
    background: var(--soft);
    border-radius: 15px;
    font-size: 28px;
}

.subject-card h3 {
    font-size: 20px;
}

.subject-card p {
    color: var(--muted);
    font-size: 14px;
    margin: 4px 0 13px;
}

.notes-btn {
    border: 0;
    padding: 8px 14px;
    border-radius: 8px;
    background: var(--primary);
    color: white;
    cursor: pointer;
    font-weight: 700;
}

.notes-btn:hover {
    background: var(--primary-dark);
}

.no-results {
    display: none;
    text-align: center;
    color: var(--muted);
    padding: 30px;
}


/* ABOUT */

.about {
    padding: 70px 0;
    background: var(--card);
    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
}

.about-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 50px;
    align-items: center;
}

.about h2 {
    font-size: 36px;
    margin-top: 8px;
}

.about p {
    color: var(--muted);
    font-size: 17px;
}


/* FOOTER */

.footer {
    text-align: center;
    padding: 40px 0;
}

.footer h3 {
    font-size: 22px;
}

.footer p {
    color: var(--muted);
}

.copyright {
    margin-top: 12px;
    font-size: 13px;
}


/* MODALS */

.modal {
    position: fixed;
    inset: 0;
    z-index: 500;
    display: none;
    align-items: center;
    justify-content: center;
    padding: 20px;
    background: rgba(15,23,42,.7);
}

.modal.active {
    display: flex;
}

.modal-content {
    position: relative;
    width: min(620px, 100%);
    max-height: 85vh;
    overflow-y: auto;
    padding: 35px;
    background: var(--card);
    border-radius: 20px;
}

.close-btn {
    position: absolute;
    top: 12px;
    right: 18px;
    border: 0;
    background: none;
    color: var(--muted);
    font-size: 32px;
    cursor: pointer;
}

.modal-icon {
    font-size: 45px;
}

.modal-content h2 {
    margin: 5px 0;
}

.modal-content > p {
    color: var(--muted);
}

.chapter-list {
    display: grid;
    gap: 10px;
    margin-top: 20px;
}

.chapter {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 15px;
    padding: 14px;
    border: 1px solid var(--border);
    border-radius: 10px;
}

.chapter span {
    font-weight: 600;
}

.download-btn {
    padding: 7px 12px;
    background: var(--soft);
    color: var(--primary);
    border-radius: 7px;
    text-decoration: none;
    font-size: 13px;
    font-weight: 700;
}

.smart-info {
    display: grid;
    gap: 12px;
    margin: 20px 0;
}

.smart-info div {
    padding: 12px;
    background: var(--soft);
    border-radius: 8px;
}

.smart-info strong {
    color: var(--primary);
    margin-right: 8px;
}

.notice {
    padding: 12px;
    background: #fff7ed;
    border-radius: 8px;
}


/* DARK MODE */

body.dark {
    --bg: #0f172a;
    --card: #1e293b;
    --text: #f8fafc;
    --muted: #94a3b8;
    --border: #334155;
    --header: rgba(15,23,42,.94);
    --soft: #172554;
}

body.dark .hero {
    background:
        radial-gradient(circle at 90% 10%, #1e3a8a, transparent 35%),
        radial-gradient(circle at 10% 90%, #312e81, transparent 35%);
}

body.dark .badge {
    background: #172554;
    color: #93c5fd;
}

body.dark .notice {
    background: #422006;
}


/* RESPONSIVE */

@media (max-width: 800px) {

    .menu {
        display: none;
    }

    .hero-content {
        flex-direction: column;
        text-align: center;
    }

    .hero-buttons {
        justify-content: center;
    }

    .hero-card {
        width: 100%;
        max-width: 320px;
    }

    .subject-grid,
    .syllabus-grid {
        grid-template-columns: 1fr;
    }

    .about-content {
        grid-template-columns: 1fr;
        gap: 20px;
    }
}


@media (max-width: 500px) {

    .hero {
        padding: 60px 0;
    }

    .hero h1 {
        font-size: 42px;
    }

    .section-heading h2 {
        font-size: 30px;
    }

    .subject-card {
        padding: 18px;
    }

    .subject-icon {
        width: 50px;
        min-width: 50px;
        height: 50px;
        font-size: 23px;
    }

    .modal-content {
        padding: 25px 18px;
    }
}
```
