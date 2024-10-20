<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Elegant Diary</title>
    <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&family=Noto+Sans+JP:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Sans JP', sans-serif;
            background: linear-gradient(135deg, #FFE4E1, #FFF0F5);
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding-top: 20px;
            background-image: url('https://www.transparenttextures.com/patterns/little-pluses.png'); /* 背景图案 */
        }
        h1 {
            font-family: 'Dancing Script', cursive;
            font-size: 48px;
            color: #FF69B4;
            text-shadow: 2px 2px rgba(255, 182, 193, 0.5);
            margin-bottom: 20px;
        }
        .container {
            width: 90%;
            max-width: 800px;
            background-color: #FFF;
            border: 1px solid #FFC0CB;
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.1);
        }
        .profile {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        .profile-img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 2px solid #FF69B4;
            margin-right: 15px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .intro {
            font-size: 16px;
            color: #555;
        }
        .post {
            border-top: 2px solid #FFC0CB;
            margin-top: 20px;
            padding-top: 15px;
        }
        .post-title {
            font-family: 'Dancing Script', cursive;
            font-size: 28px;
            color: #FF69B4;
            margin-bottom: 5px;
        }
        .post-content {
            font-size: 16px;
            line-height: 1.8;
            margin-bottom: 10px;
            color: #666;
        }
        .date {
            font-size: 12px;
            color: #999;
            margin-bottom: 10px;
        }
        .button {
            display: inline-block;
            background-color: #FF69B4;
            color: #FFF;
            padding: 10px 20px;
            border-radius: 20px;
            text-decoration: none;
            box-shadow: 0 4px #C71585;
            transition: all 0.3s;
            font-size: 14px;
        }
        .button:hover {
            background-color: #C71585;
            box-shadow: 0 2px #C71585;
            transform: translateY(-2px);
        }
        .footer {
            margin-top: 30px;
            font-size: 12px;
            color: #999;
        }
        .gif-icon {
            width: 50px;
            margin: 5px;
        }
    </style>
</head>
<body>
    <h1>My Elegant Diary ✨</h1>

    <div class="container">
        <div class="profile">
            <img src="https://i.ibb.co/72G6trd/IMG-3534.jpg" alt="Profile Picture" class="profile-img">
            <div class="intro">
                <p>こんにちは！私は奈子です！日常生活やお気に入りのことについて書いています。どうぞ楽しんでくださいね！😊</p>
            </div>
        </div>

        <div class="post">
            <h2 class="post-title">🌸 今日のランチ 🌸</h2>
            <p class="date">2024年10月20日</p>
            <p class="post-content">今日はお友達とカフェでランチをしました！美味しいパフェとパンケーキが最高でした。また行きたいなぁ〜！💗</p>
            <img src="https://ibb.co/nmNvz1h" alt="Cute Icon" class="gif-icon">
        </div>

        <div class="post">
            <h2 class="post-title">✨ 新しいドレス ✨</h2>
            <p class="date">2024年10月19日</p>
            <p class="post-content">昨日、ずっと欲しかったドレスを買いました！色はパステルピンクで、リボンがいっぱいついてて可愛いです。今度写真を載せますね！📷</p>
            <img src="https://ibb.co/jvM1gQs" alt="Cute Icon" class="gif-icon">
        </div>

        <a href="#" class="button">日記を書く</a>
    </div>

    <div class="footer">
        <p>&copy; 2024 My Elegant Diary. All rights reserved.</p>
    </div>
</body>
</html>
