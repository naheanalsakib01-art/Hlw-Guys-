<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hlw Guys 么 - Official Page</title>
    <style>
        :root {
            --royal-red: #D40000;
            --pure-white: #FFFFFF;
            --soft-gray: #f0f2f5;
        }

        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            background-color: var(--soft-gray);
            color: #1c1e21;
        }

        /* ১. লোগো ও নামের এনিমেশন পপআপ */
        #splash-screen {
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: var(--royal-red);
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            z-index: 9999;
            animation: fadeOut 3.5s forwards;
        }

        .logo-circle {
            width: 120px; height: 120px;
            background: white;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 45px;
            font-weight: bold;
            color: var(--royal-red);
            box-shadow: 0 0 30px rgba(0,0,0,0.5);
            animation: bounceIn 1.5s ease;
        }

        .brand-name {
            color: white;
            font-size: 2rem;
            margin-top: 20px;
            letter-spacing: 2px;
            animation: fadeInUp 2s ease;
        }

        @keyframes bounceIn {
            0% { transform: scale(0.3); opacity: 0; }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); opacity: 1; }
        }

        @keyframes fadeInUp {
            from { transform: translateY(30px); opacity: 0; }
            to { transform: translateY(0); opacity: 1; }
        }

        @keyframes fadeOut {
            80% { opacity: 1; visibility: visible; }
            100% { opacity: 0; visibility: hidden; }
        }

        /* ২. হেডার */
        header {
            background: var(--royal-red);
            color: white;
            padding: 60px 20px;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }

        /* ৩. নেভিগেশন */
        .nav-bar {
            display: flex;
            justify-content: center;
            background: white;
            padding: 15px;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .btn {
            padding: 10px 25px;
            margin: 0 10px;
            border-radius: 20px;
            border: none;
            cursor: pointer;
            font-weight: bold;
            text-decoration: none;
            transition: 0.3s;
        }

        .btn-about { background: var(--royal-red); color: white; }
        .btn-follow { background: #1877F2; color: white; }

        /* ৪. মিম পোস্ট কার্ড */
        .feed-container { max-width: 550px; margin: 30px auto; padding: 0 15px; }

        .post-card {
            background: white;
            border-radius: 10px;
            margin-bottom: 25px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
            border: 1px solid #ddd;
        }

        .post-header { padding: 12px; display: flex; align-items: center; }
        .post-pfp { width: 40px; height: 40px; background: #ddd; border-radius: 50%; margin-right: 10px; border: 2px solid var(--royal-red); }
        
        .post-img-demo {
            width: 100%;
            height: 350px;
            background: #f9f9f9;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #888;
            border-top: 1px solid #eee;
            border-bottom: 1px solid #eee;
        }

        .post-footer { padding: 12px; }
        .love-icon { color: #ff304f; font-size: 24px; cursor: pointer; }

        /* ৫. এবাউট স্লাইড (Modal) */
        #about-slide {
            display: none;
            position: fixed;
            top: 50%; left: 50%;
            transform: translate(-50%, -50%);
            background: white;
            width: 90%; max-width: 400px;
            border-radius: 20px;
            padding: 30px;
            z-index: 9999;
            text-align: center;
            box-shadow: 0 0 50px rgba(0,0,0,0.5);
        }

        .owner-img {
            width: 130px; height: 130px;
            border-radius: 50%;
            border: 5px solid var(--royal-red);
            object-fit: cover;
            margin-bottom: 15px;
        }

        .red-tik { color: red; font-size: 20px; margin-left: 5px; }
        .close-btn { margin-top: 20px; color: gray; cursor: pointer; display: block; }

        .overlay-bg {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.7);
            z-index: 9998;
        }
    </style>
</head>
<body>

    <div id="splash-screen">
        <div class="logo-circle">HG</div>
        <div class="brand-name">Hlw Guys 么</div>
    </div>

    <header>
        <h1>Welcome to Hlw Guys 么</h1>
        <p>হাসি আর বিনোদনের এক অন্য জগত!</p>
    </header>

    <div class="nav-bar">
        <button class="btn btn-about" onclick="toggleAbout(true)">About Owner</button>
        <a href="https://www.facebook.com/share/184KgF9MYT/" target="_blank" class="btn btn-follow">Follow Page</a>
    </div>

    <div class="feed-container">
        <div class="post-card">
            <div class="post-header">
                <div class="post-pfp"></div>
                <div><strong>Hlw Guys 么</strong><br><small>Just now • Public</small></div>
            </div>
            <div class="post-img-demo">
                [Demo Meme Image 1]
            </div>
            <div class="post-footer">
                <span class="love-icon">❤️</span> <strong>1.2K</strong>
            </div>
        </div>

        <div class="post-card">
            <div class="post-header">
                <div class="post-pfp"></div>
                <div><strong>Hlw Guys 么</strong><br><small>2 hours ago • Public</small></div>
            </div>
            <div class="post-img-demo">
                [Demo Meme Image 2]
            </div>
            <div class="post-footer">
                <span class="love-icon">❤️</span> <strong>850</strong>
            </div>
        </div>
    </div>

    <div class="overlay-bg" id="bg-overlay" onclick="toggleAbout(false)"></div>
    <div id="about-slide">
        <img src="https://via.placeholder.com/150/0000FF/FFFFFF?text=Rich+Businessman" alt="Owner" class="owner-img">
        <h2>NAHEAN AL SAKIB <span class="red-tik">✔</span></h2>
        <p style="color: var(--royal-red); font-weight: bold;">Admin (Rich Business Man)</p>
        <p><strong>Permanent Address:</strong> Dhaka, Bangladesh</p>
        <p><strong>Present Address:</strong> Bogura, Bangladesh</p>
        <hr>
        <p>This is a funny meme page to make you smile!</p>
        <a href="https://www.facebook.com/share/184KgF9MYT/" class="btn btn-follow" style="display:inline-block; margin-top:10px;">Visit Profile</a>
        <span class="close-btn" onclick="toggleAbout(false)">[ Close ]</span>
    </div>

    <script>
        function toggleAbout(show) {
            const display = show ? 'block' : 'none';
            document.getElementById('about-slide').style.display = display;
            document.getElementById('bg-overlay').style.display = display;
        }
    </script>

</body>
</html>
