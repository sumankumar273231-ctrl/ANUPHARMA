<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>ODPHARMA - Pharmacy Education Portal</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

html {
    scroll-behavior: smooth;
}

body {
    background: #f1f8ff;
    color: #1e293b;
}

/* ANNOUNCEMENT BAR */

.announcement {
    background: linear-gradient(100deg, #124da0, #087b59);
    color: red;
    text-align: center;
    padding: 14px 12px;
    font-size: 15px;
    font-weight: 600;
    line-height: 1.6;
}

.update {
    background: #ffffff30;
    padding: 7px 13px;
    border-radius: 7px;
    margin-right: 12px;
    font-size: 13px;
}

/* HEADER */

.header {
    background: blue;
    padding: 18px 5%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 15px;
    box-shadow: 0 3px 15px #00000010;
}

.brand {
    display: flex;
    align-items: center;
    gap: 12px;
}

.logo {
    background: linear-gradient(135deg, #0875d1, #07865c);
    color: yellow;
    width: 57px;
    height: 57px;
    border-radius: 14px;
    display: grid;
    place-items: center;
    font-size: 27px;
    font-weight: bold;
}

.brand h1 {
    color: #1451a0;
    font-size: 25px;
}

.brand p {
    color: #64748b;
    font-size: 13px;
    margin-top: 4px;
}

.header-buttons {
    display: flex;
    align-items: center;
    gap: 12px;
}

.header-buttons button {
    padding: 12px 18px;
    border-radius: 10px;
    font-size: 15px;
    font-weight: bold;
    cursor: pointer;
}

.search-btn {
    background: #f1f5f9;
    border: 1px solid #dbe4ef;
    color: #1e293b;
    font-size: 21px !important;
}

.admin-btn {
    background: green;
    color: #1260bd;
    border: 2px solid #1260bd;
}

.login-btn {
    background: #1260d5;
    color: white;
    border: 2px solid #1260d5;
}

/* HERO SECTION */

.hero {
    padding: 85px 5%;
    background: linear-gradient(135deg, #eff7ff, #edfaf5);
}

.hero-container {
    max-width: 1250px;
    margin: auto;
}

.badge {
    display: inline-block;
    background: white;
    color: #168454;
    border: 1px solid #dce9f3;
    padding: 12px 22px;
    border-radius: 30px;
    font-weight: bold;
    font-size: 15px;
    box-shadow: 0 3px 10px #00000010;
    margin-bottom: 28px;
}

.hero h2 {
    font-size: clamp(34px, 5vw, 57px);
    line-height: 1.15;
    max-width: 850px;
    margin-bottom: 24px;
    color: #1e293b;
}

.hero h2 span {
    color: #1260bd;
}

.hero-description {
    max-width: 850px;
    font-size: 19px;
    line-height: 1.8;
    color: #64748b;
    margin-bottom: 35px;
}

/* BUTTONS */

.hero-buttons {
    display: flex;
    gap: 18px;
    flex-wrap: wrap;
}

.hero-buttons a {
    text-decoration: none;
    padding: 17px 28px;
    border-radius: 11px;
    font-size: 17px;
    font-weight: bold;
    transition: 0.3s;
}

.explore {
    background: #1260d5;
    color: white;
}

.notes {
    background: #168653;
    color: white;
}

.hero-buttons a:hover {
    transform: translateY(-3px);
    opacity: 0.9;
}

/* STATISTICS */

.stats {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 25px;
    border-top: 1px solid #dce5ed;
    margin-top: 48px;
    padding-top: 35px;
}

.stat h3 {
    font-size: 30px;
    color: #1260d5;
    margin-bottom: 8px;
}

.stat p {
    color: #64748b;
    font-size: 16px;
    font-weight: 600;
}

/* FEATURES */

.features {
    padding: 60px 5%;
}

.section-title {
    text-align: center;
    margin-bottom: 35px;
}

.section-title h2 {
    font-size: 30px;
    color: #174b88;
}

.feature-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 22px;
    max-width: 1200px;
    margin: auto;
}

.feature-card {
    background: white;
    padding: 30px 22px;
    border-radius: 16px;
    border: 1px solid #e1eaf3;
    box-shadow: 0 5px 20px #00000008;
}

.feature-card .icon {
    font-size: 38px;
    margin-bottom: 15px;
}

.feature-card h3 {
    color: #1451a0;
    margin-bottom: 10px;
}

.feature-card p {
    color: #64748b;
    line-height: 1.6;
}

/* FOOTER */

footer {
    background: #103d69;
    color: white;
    padding: 35px 15px;
    text-align: center;
}

footer p {
    color: #dbeafe;
    margin-top: 10px;
    font-size: 14px;
}

/* MOBILE RESPONSIVE */

@media(max-width: 650px) {

    .announcement {
        font-size: 12px;
        padding: 12px 8px;
    }

    .update {
        display: inline-block;
        margin-bottom: 5px;
    }

    .header {
        flex-wrap: wrap;
        padding: 15px;
    }

    .brand {
        width: 100%;
    }

    .brand h1 {
        font-size: 23px;
    }

    .header-buttons {
        width: 100%;
        gap: 8px;
    }

    .header-buttons button {
        flex: 1;
        padding: 11px 8px;
        font-size: 13px;
    }

    .search-btn {
        flex: 0 0 48px !important;
    }

    .hero {
        padding: 55px 20px;
    }

    .badge {
        font-size: 12px;
        padding: 10px 14px;
    }

    .hero-description {
        font-size: 16px;
    }

    .hero-buttons {
        flex-direction: column;
    }

    .hero-buttons a {
        text-align: center;
    }

    .stats {
        grid-template-columns: repeat(2, 1fr);
        gap: 28px 12px;
    }

    .stat h3 {
        font-size: 25px;
    }

    .stat p {
        font-size: 13px;
    }

    .features {
        padding: 40px 18px;
    }
}
</style>
</head>

<body>

<!-- ANNOUNCEMENT -->

<div class="announcement">
    <span class="update">UPDATE</span>
    Welcome to ODPHARMA — PCI Syllabus Aligned Notes,
    Video Lectures & Question Bank Portal.
</div>

<!-- HEADER -->

<header class="header">

    <div class="brand">
        <div class="logo">Rx</div>

        <div>
            <h1>ODPHARMA</h1>
            <p>Pharmacy Education Portal</p>
        </div>
    </div>

    <div class="header-buttons">

        <button class="search-btn"
        onclick="document.getElementById('features').scrollIntoView()">
            🔍
        </button>

        <button class="admin-btn"
        onclick="alert('Admin panel will be added in the next development stage.')">
            Admin
        </button>

        <button class="login-btn"
        onclick="alert('Student login will be added in the next development stage.')">
            Login / Register
        </button>

    </div>

</header>

<!-- HERO -->

<section class="hero" id="home">

<div class="hero-container">

    <div class="badge">
        PCI Syllabus Aligned • Pharmacy Study Hub
    </div>

    <h2>
        Your Complete Pharmacy
        <span>Learning Platform</span>
    </h2>

    <p class="hero-description">
        Access structured unit-wise handwritten notes,
        HD concept video lectures, PCI syllabus PDFs,
        important exam questions, and previous year
        papers in one clean platform.
    </p>

    <div class="hero-buttons">

        <a href="#features" class="explore">
            Explore More →
        </a>

        <a href="#features" class="notes">
            Get Free Notes
        </a>

    </div>

    <!-- STATISTICS -->

    <div class="stats">

        <div class="stat">
            <h3>0+</h3>
            <p>Uploaded Notes</p>
        </div>

        <div class="stat">
            <h3>0+</h3>
            <p>Video Lectures</p>
        </div>

        <div class="stat">
            <h3>0+</h3>
            <p>Question Papers</p>
        </div>

        <div class="stat">
            <h3>8</h3>
            <p>Semesters Covered</p>
        </div>

    </div>

</div>

</section>

<!-- FEATURES -->

<section class="features" id="features">

    <div class="section-title">
        <h2>Explore Pharmacy Resources</h2>
    </div>

    <div class="feature-grid">

        <div class="feature-card">
            <div class="icon">🎓</div>
            <h3>B.Pharmacy</h3>
            <p>Complete semester-wise pharmacy study materials.</p>
        </div>

        <div class="feature-card">
            <div class="icon">📚</div>
            <h3>Study Notes</h3>
            <p>Chapter-wise and unit-wise educational notes.</p>
        </div>

        <div class="feature-card">
            <div class="icon">📄</div>
            <h3>PDF Library</h3>
            <p>Access pharmacy educational PDF resources.</p>
        </div>

        <div class="feature-card">
            <div class="icon">💘</div>
            <h3>SAMEER 💝 RESHMA</h3>
            <p HOW DO IMPRESS A GIRL NEW COURSE🤣. </p>
        </div>

    </div>

</section>

<!-- FOOTER -->

<footer>
    <h2>ODPHARMA</h2>
    <p>Your Pharmacy Learning Platform</p>
    <p>Learn • Explore • Grow</p>
    <p>© 2026 ODPHARMA. All Rights Reserved.</p>
     <p>ABOUT ME</p> 
</footer>

</body>
</html>
