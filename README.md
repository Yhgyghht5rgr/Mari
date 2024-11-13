<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A&M HEALTH</title>
    <link rel="manifest" href="manifest.json">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #2a9d8f;
            color: white;
            padding: 30px 0;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        header h1 {
            font-size: 36px;
            margin-bottom: 10px;
        }
        header p {
            font-size: 18px;
        }
        nav {
            background-color: #264653;
            padding: 15px 0;
            text-align: center;
            position: sticky;
            top: 0;
        }
        nav a {
            color: white;
            padding: 12px 20px;
            text-decoration: none;
            margin: 0 15px;
            font-size: 18px;
            transition: background-color 0.3s ease;
        }
        nav a:hover {
            background-color: #2a9d8f;
        }
        .container {
            padding: 20px;
        }
        .section-title {
            font-size: 28px;
            margin-bottom: 15px;
            color: #333;
            text-align: center;
            transition: color 0.3s ease;
        }
        .section-title:hover {
            color: #2a9d8f;
        }
        .section {
            background-color: white;
            padding: 25px;
            margin-bottom: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        .news-item, .tip-item {
            margin-bottom: 20px;
        }
        .news-image, .tip-image {
            width: 100%;
            max-width: 500px;
            height: auto;
            display: block;
            margin: 0 auto 15px;
            border-radius: 8px;
        }
        footer {
            background-color: #2a9d8f;
            color: white;
            padding: 15px 0;
            text-align: center;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

    <!-- Header Section -->
    <header>
        <h1>A&M HEALTH</h1>
        <p>Your Guide to a Healthier Life</p>
    </header>

    <!-- Navigation Bar -->
    <nav>
        <a href="#news">Health News</a>
        <a href="#tips">Health Tips</a>
        <a href="#nutrition">Nutrition</a>
        <a href="#fitness">Fitness</a>
    </nav>

    <!-- Main Content -->
    <div class="container">
        <!-- Health News Section -->
        <section id="news" class="section">
            <h2 class="section-title">Latest Health News</h2>
            <div class="news-item">
                <img src="https://images.unsplash.com/photo-1503676260728-1c00da094a0b" alt="Meditation" class="news-image">
                <h3>New Study Shows Benefits of Meditation</h3>
                <p>A recent study confirms the long-term health benefits of daily meditation...</p>
            </div>
            <div class="news-item">
                <img src="https://images.unsplash.com/photo-1554284126-6f121c15bcb5" alt="Exercise" class="news-image">
                <h3>Exercise Improves Mental Health</h3>
                <p>Regular physical activity has been shown to boost mood and reduce anxiety...</p>
            </div>
        </section>

        <!-- Health Tips Section -->
        <section id="tips" class="section">
            <h2 class="section-title">Health Tips</h2>
            <div class="tip-item">
                <img src="https://images.unsplash.com/photo-1528909514045-2fa4ac7a08ba" alt="Drink Water" class="tip-image">
                <p>Drink plenty of water throughout the day to stay hydrated.</p>
            </div>
            <div class="tip-item">
                <img src="https://images.unsplash.com/photo-1541698444083-023c97d3f4b6" alt="Sleep" class="tip-image">
                <p>Sleep 7-9 hours every night for optimal health.</p>
            </div>
        </section>
    </div>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2024 A&M HEALTH. All rights reserved.</p>
    </footer>

    <script>
        if ('serviceWorker' in navigator) {
            navigator.serviceWorker.register('/service-worker.js').then(() => {
                console.log('Service Worker Registered');
            });
        }
    </script>

</body>
</html>
