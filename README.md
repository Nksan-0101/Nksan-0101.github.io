<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Cute Diary</title>
    <link href="https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Permanent Marker', cursive;
            background-color: #FFE4E1;
            color: #333;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding-top: 20px;
            background-image: url('https://www.transparenttextures.com/patterns/little-pluses.png'); /* 背景纹理 */
        }
        h1 {
            font-size: 36px;
            color: #FF69B4;
            text-shadow: 2px 2px #FFB6C1;
        }
        .container {
            width: 90%;
            max-width: 800px;
            background-color: #FFF;
            border: 3px solid #FF69B4;
            border-radius: 15px;
            padding: 20px;
            box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
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
        }
        .intro {
            font-size: 16px;
        }
        .post {
            border-top: 2px dashed #FF69B4;
            margin-top: 20px;
            padding-top: 10px;
        }
        .post-title {
            font-size: 24px;
            color: #FF69B4;
            margin-bottom: 5px;
        }
        .post-content {
            font-size: 16px;
            line-height: 1.6;
            margin-bottom: 10px;
        }
        .date {
            font-size: 12px;
            color: #777;
        }
        .button {
            display: inline-block;
            background-color: #FFB6C1;
            color: #FFF;
            padding: 10px 20px;
            border-radius: 10px;
            text-decoration: none;
            box-shadow: 0 4px #FF69B4;
            transition: all 0.2s;
            font-size: 14px;
        }
        .button:hover {
            background-color: #FF69B4;
            box-shadow: 0 2px #FF69B4;
        }
        .footer {
            margin-top: 30px;
            font-size: 12px;
            color: #777;
        }
    </style>
</head>
<body>
    <h1>My Cute Diary 💖</h1>

    <div class="container">
        <div class="profile">
            <img src="profile-pic.png" alt="Profile Picture" class="profile-img">
            <div class="intro">
                <p>こんにちは！私は[名前]です！💫 日常の出来事や好きなことを書いています。楽しんでくださいね！😊</p>
            </div>
        </div>

        <div class="post">
            <h2 class="post-title">🌸 今日のランチ 🌸</h2>
            <p class="date">2024年10月20日</p>
            <p class="post-content">今日はお友達とカフェでランチをしました！美味しいパフェとパンケーキが最高でした。💗 また行きたいなぁ〜！</p>
        </div>

        <div class="post">
            <h2 class="post-title">✨ 新しいドレス ✨</h2>
            <p class="date">2024年10月19日</p>
            <p class="post-content">昨日、ついにずっと欲しかったドレスを買いました！色はパステルピンクで、リボンがいっぱいついてて可愛い〜！今度写真を載せますね！📷</p>
        </div>

        <a href="#" class="button">日記を書く</a>
    </div>

    <div class="footer">
        <p>&copy; 2024 My Cute Diary. All rights reserved.</p>
    </div>
</body>
</html>
