# all-or-nothing
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Wanderlust Philippines | Travel & Tourism</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f5f8f6;
            color: #24332b;
            line-height: 1.6;
        }

        /* =========================
           NAVIGATION
        ========================= */

        header {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(255,255,255,0.96);
            box-shadow: 0 3px 15px rgba(0,0,0,0.08);
        }

        nav {
            max-width: 1200px;
            margin: auto;
            padding: 18px 25px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 25px;
            font-weight: bold;
            color: #176b57;
            letter-spacing: 1px;
        }

        .logo span {
            color: #d89b35;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 28px;
        }

        nav ul li a {
            text-decoration: none;
            color: #24332b;
            font-weight: bold;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: #176b57;
        }

        /* =========================
           HERO
        ========================= */

        .hero {
            min-height: 90vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 50px 20px;

            background:
                linear-gradient(rgba(12,55,45,0.55), rgba(12,55,45,0.45)),
                url("https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1600&q=80");

            background-size: cover;
            background-position: center;
            color: white;
        }

        .hero-content {
            max-width: 850px;
        }

        .hero h1 {
            font-size: clamp(45px, 8vw, 85px);
            line-height: 1;
            margin-bottom: 25px;
            text-shadow: 3px 4px 10px rgba(0,0,0,0.35);
        }

        .hero h1 span {
            color: #ffd98b;
        }

        .hero p {
            font-size: 19px;
            max-width: 680px;
            margin: auto;
        }

        .btn {
            display: inline-block;
            margin-top: 30px;
            padding: 14px 28px;
            background: #e1a548;
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            background: #176b57;
            transform: translateY(-4px);
            box-shadow: 0 8px 20px rgba(0,0,0,0.2);
        }

        /* =========================
           GENERAL SECTIONS
        ========================= */

        section {
            padding: 90px 7%;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 38px;
            color: #176b57;
            margin-bottom: 10px;
        }

        .section-title p {
            color: #68756e;
        }

        /* =========================
           ABOUT
        ========================= */

        .about {
            background: white;
        }

        .about-container {
            max-width: 1100px;
            margin: auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-image {
            min-height: 420px;
            border-radius: 25px;
            background:
                url("https://images.unsplash.com/photo-1493976040374-85c8e12f0c0e?auto=format&fit=crop&w=1000&q=80")
                center/cover;
            box-shadow: 15px 15px 0 #dce9e1;
        }

        .about-text h3 {
            font-size: 30px;
            color: #24332b;
            margin-bottom: 20px;
        }

        .about-text p {
            color: #637067;
            margin-bottom: 18px;
        }

        /* =========================
           DESTINATIONS
        ========================= */

        .destinations {
            background: #eef5f0;
        }

        .destination-grid {
            max-width: 1200px;
            margin: auto;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .destination-card {
            background: white;
            border-radius: 20px;
            overflow: hidden;
          
