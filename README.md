<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Stylish Blog</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --main-bg-color: #F5D1D1; /* 柔和的粉色背景 */
            --light-bg-color: #FFF1F1; /* 浅粉色 */
            --card-bg-color: #FFFFFF; /* 卡片背景 */
            --primary-color: #854848; /* 深粉灰色 */
            --accent-color: #D8A7A7; /* 辅助粉色 */
            --shadow-color: rgba(0, 0, 0, 0.1); /* 阴影颜色 */
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'PingFang SC', 'Roboto', sans-serif;
            background: linear-gradient(135deg, var(--main-bg-color), #f8e6e6);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            color: var(--primary-color);
        }
        .container {
            display: flex;
            flex: 1;
            flex-direction: row;
            margin: 20px;
        }
        .sidebar {
            background-color: var(--light-bg-color);
            width: 25%;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 2px 2px 10px var(--shadow-color);
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .main-content {
            background-color: var(--card-bg-color);
            width: 75%;
            margin-left: 20px;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 2px 2px 10px var(--shadow-color);
            overflow-y: auto;
        }
        h1, h2, h3 {
            color: var(--primary-color);
            margin-bottom: 15px;
        }
        .profile-img {
            width: 100%;
            max-width: 150px;
            border-radius: 50%;
            margin-bottom: 20px;
            border: 3px solid var(--accent-color);
            transition: transform 0.3s;
        }
        .profile-img:hover {
            transform: scale(1.05);
        }
        .post-list {
            margin-bottom: 40px;
        }
        .post-item {
            background-color: var(--light-bg-color);
            border-radius: 8px;
            box-shadow: 0 2px 4px var(--shadow-color);
            padding: 20px;
            margin-bottom: 20px;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .post-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 8px var(--shadow-color);
        }
        .tag-input {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid var(--accent-color);
            border-radius: 5px;
            outline: none;
        }
        .add-btn {
            padding: 10px;
            background-color: var(--accent-color);
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.2s;
        }
        .add-btn:hover {
            background-color: #B38383;
        }
        .add-btn:active {
            transform: scale(0.98);
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: var(--light-bg-color);
            border-top: 1px solid var(--accent-color);
            border-radius: 0 0 10px 10px;
        }
        @media (max-width: 768px) {
            .container {
                flex-direction: column;
            }
            .sidebar {
                width: 100%;
                margin-bottom: 20px;
            }
            .main-content {
                width: 100%;
                margin-left: 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>My Stylish Blog</h1>
    </header>

    <div class="container">
        <aside class="sidebar">
            <h2>About Me</h2>
            <img src="profile.jpg" alt="Profile Picture" class="profile-img">
            <p>Hello, I'm [Your Name]. I love writing and sharing my thoughts on various topics. Welcome to my archive!</p>
        </aside>

        <main class="main-content">
            <h2>Article Archive</h2>
            
            <section class="post-list">
                <div class="post-item">
                    <h3>Article 1</h3>
                    <p>Category: Fiction</p>
                    <p>Tags: Story, Adventure</p>
                </div>
                <div class="post-item">
                    <h3>Article 2</h3>
                    <p>Category: Non-fiction</p>
                    <p>Tags: History, Analysis</p>
                </div>
            </section>

            <section class="tag-management">
                <h2>Add Tags & Archive</h2>
                <input type="text" class="tag-input" placeholder="Add new tag">
                <button class="add-btn">Add Tag</button>
            </section>
        </main>
    </div>

    <footer>
        <p>&copy; 2024 My Stylish Blog. All rights reserved.</p>
    </footer>

    <script>
        document.querySelector('.add-btn').addEventListener('click', function() {
            const tagInput = document.querySelector('.tag-input');
            if (tagInput.value.trim()) {
                alert('Tag added: ' + tagInput.value);
                tagInput.value = '';
            }
        });
    </script>
</body>
</html>
