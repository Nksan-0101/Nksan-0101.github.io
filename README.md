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
            --light-bg-color: #FAE6E6; /* 浅粉色 */
            --card-bg-color: #FFF8F8; /* 卡片背景 */
            --primary-color: #854848; /* 深粉灰色 */
            --accent-color: #D8A7A7; /* 辅助粉色 */
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Roboto', sans-serif;
            background-color: var(--main-bg-color);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
            color: var(--primary-color);
        }
        .container {
            display: flex;
            flex: 1;
            flex-direction: row;
        }
        .sidebar {
            background-color: var(--light-bg-color);
            width: 25%;
            padding: 20px;
            box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
        }
        .main-content {
            background-color: var(--card-bg-color);
            width: 75%;
            padding: 40px;
            overflow-y: auto;
        }
        h1, h2, h3 {
            color: var(--primary-color);
            margin-bottom: 10px;
        }
        .profile-img {
            width: 100%;
            max-width: 150px;
            border-radius: 50%;
            margin-bottom: 20px;
            border: 2px solid var(--accent-color);
        }
        .post-list {
            margin-bottom: 40px;
        }
        .post-item {
            background-color: var(--light-bg-color);
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
            padding: 20px;
            margin-bottom: 20px;
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
            transition: background-color 0.3s;
        }
        .add-btn:hover {
            background-color: #B38383;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: var(--light-bg-color);
            border-top: 1px solid var(--accent-color);
        }
        @media (max-width: 768px) {
            .container {
                flex-direction: column;
            }
            .sidebar {
                width: 100%;
                padding: 10px;
            }
            .main-content {
                width: 100%;
                padding: 20px;
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
