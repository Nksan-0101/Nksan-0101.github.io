<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alexander's Conspiracy Page</title>
    <style>
        body {
            font-family: 'Courier New', monospace;
            background-color: #FF00FF;
            color: #00FFFF;
            margin: 0;
            padding: 0;
            display: flex;
            height: 100vh;
            background-image: url('https://www.transparenttextures.com/patterns/noise-lines.png'); /* 像素背景纹理 */
        }
        .sidebar {
            width: 20%;
            background-color: #00FF00;
            padding: 10px;
            border-right: 6px solid #000;
            display: flex;
            flex-direction: column;
            align-items: center;
            box-shadow: inset -4px -4px 0px #FFF, inset 4px 4px 0px #000;
        }
        .main-content {
            width: 80%;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
        }
        .window {
            width: 90%;
            background-color: #FF0000;
            border: 10px solid #000;
            box-shadow: 6px 6px 0px #000, -6px -6px 0px #FFF;
            image-rendering: pixelated;
            margin-bottom: 20px;
        }
        .window-header {
            background-color: #FFFF00;
            color: #000;
            padding: 5px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            font-size: 18px;
        }
        .window-header .title {
            font-size: 18px;
        }
        .window-header .buttons span {
            width: 16px;
            height: 16px;
            background-color: #C0C0C0;
            border: 3px solid #000;
            display: inline-block;
            margin-right: 3px;
            image-rendering: pixelated;
        }
        .window-content {
            padding: 15px;
            background-color: #000;
            color: #FFF;
            height: 300px;
            overflow-y: auto;
            font-size: 18px;
            image-rendering: pixelated;
        }
        .profile-img {
            width: 100%;
            max-width: 120px;
            image-rendering: pixelated;
            margin-bottom: 15px;
            border: 6px solid #FFF;
        }
        .button {
            width: 120px;
            padding: 8px;
            margin-top: 15px;
            text-align: center;
            background-color: #0000FF;
            border: 3px solid #000;
            cursor: pointer;
            box-shadow: 6px 6px 0px #000;
            font-size: 14px;
            image-rendering: pixelated;
        }
        .button:hover {
            background-color: #000080;
        }
        .radio-station {
            margin-top: 30px;
            background-color: #00FFFF;
            padding: 15px;
            border: 6px solid #000;
            text-align: center;
            font-size: 18px;
            width: 100%;
            box-shadow: 3px 3px 0px #000;
        }
    </style>
</head>
<body>
    <div class="sidebar">
        <h2>About Me</h2>
        <img src="/mnt/data/A_pixelated_avatar_of_a_scruffy_white_middle-aged_.png" alt="Profile Picture" class="profile-img">
        <p>Name: Alexander</p>
        <p>Age: 45</p>
        <p>I am Alexander, the truth seeker! I’ve uncovered the secrets they don’t want you to know—lizard people, mutants, and the REAL shape of our planet. If you dare, contact me at alexander@conspiracy.net, or visit my HQ at 123 Unknown Street, Nowhereville. Don’t let them silence you!</p>
    </div>

    <div class="main-content">
        <div class="window">
            <div class="window-header">
                <div class="title">My Beliefs and Research</div>
                <div class="buttons">
                    <span></span>
                    <span></span>
                    <span></span>
                </div>
            </div>
            <div class="window-content">
                <p>Welcome! I am Alexander, and I have dedicated my life to exposing the TRUTH. The government, the media, and even your neighbors are hiding things from you. Did you know that lizard people are walking among us, controlling every aspect of society? I have proof, but they want to silence me.</p>
                <p>Mutants? Yes, they are REAL. The government has been conducting experiments for years, and some of us know too much. As for the Earth? It’s flat—don’t be fooled by the lies of ‘science’ and ‘astronauts’. I’ve done the research, I’ve connected the dots, and I am here to share the REAL story with you.</p>
                <p>Follow me, and together we will unveil the mysteries of the universe. The truth is out there, and it’s time for us to take it back!</p>
            </div>
        </div>
        
        <div class="radio-station">
            <p>Broadcasting Live: Alexander's Conspiracy Radio - Tune in and hear the TRUTH they don’t want you to know!</p>
        </div>
    </div>
</body>
</html>
