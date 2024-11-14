<!DOCTYPE html>
<html lang="sk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfólio - [Tvoje Meno]</title>
    <link rel="stylesheet" href="style.css">
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        /* Telo stránky */
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f5f5f5;
            color: #333;
            scroll-behavior: smooth;
            overflow-x: hidden;
        }

        /* Hlavná hlavička */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 40px;
            background: #333;
            color: #fff;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 10;
            transition: background 0.3s ease;
        }

        header.scrolled {
            background: rgba(0, 0, 0, 0.8);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }

        /* Logo */
        .logo {
            font-size: 1.5em;
            font-weight: bold;
            color: #4caf50;
        }

        /* Navigačné odkazy */
        nav a {
            color: #fff;
            margin: 0 15px;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #4caf50;
        }

        /* Sekcie */
        section {
            padding: 100px 20px;
            max-width: 1200px;
            margin: 80px auto;
            opacity: 0;
            transform: translateY(50px);
            transition: all 0.6s ease-out;
        }

        section.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Projekty */
        .project-gallery {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .project {
            position: relative;
            width: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }

        .project img {
            width: 100%;
            display: block;
            transition: transform 0.3s ease;
        }

        .project:hover {
            transform: scale(1.05);
        }

        .project:hover img {
            transform: scale(1.1);
        }

        /* O mne a Kontakt */
        .contact-info a {
            color: #333;
            font-weight: bold;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .contact-info a:hover {
            color: #4caf50;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background-color: #333;
            color: #fff;
            margin-top: 20px;
        }

    </style>
</head>
<body>

<header id="header">
    <div class="logo">[Tvoje Meno]</div>
    <nav>
        <a href="#about">O mne</a>
        <a href="#services">Služby</a>
        <a href="#projects">Projekty</a>
        <a href="#contact">Kontakt</a>
    </nav>
</header>

<section id="about">
    <h2>O mne</h2>
    <p>**Profesionálny grafický dizajnér** so skúsenosťami v oblasti branding, UI/UX a digitálneho umenia. Tvorím dizajny, ktoré kombinujú estetiku s funkčnosťou a prinášajú hodnotu.</p>
</section>

<section id="services">
    <h2>Moje Služby</h2>
    <ul>
        <li>Branding – Výrazná vizuálna identita</li>
        <li>UI/UX Dizajn – Intuitívne a moderné rozhrania</li>
        <li>Animácie – Dynamické a pútavé efekty</li>
    </ul>
</section>

<section id="projects">
    <h2>Projekty</h2>
    <div class="project-gallery">
        <div class="project">
            <img src="img/project1.jpg" alt="Projekt 1">
            <p>Moderný UI/UX dizajn pre technologickú firmu.</p
