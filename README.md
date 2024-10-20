<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Stylish Blog</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #F5D1D1; /* 柔和的粉色背景 */
            margin: 0;
            padding: 0;
            display: flex;
            height: 100vh;
            overflow: hidden;
            color: #5F4B4B; /* 深灰色字体 */
        }
        .sidebar {
            background-color: #FAE6E6; /* 更柔和的浅粉色 */
            width: 25%;
            padding: 20px;
            box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .main-content {
            background-color: #FFF8F8; /* 柔和的白粉色 */
            width: 75%;
            padding: 40px;
            overflow-y: auto;
            box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.05);
        }
        h1, h2, h3 {
            color: #854848; /* 深粉灰色字体 */
            margin: 0 0 10px;
        }
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            margin-bottom: 20px;
            border: 2px solid #D8A7A7; /* 柔和的粉色 */
        }
        .post-list {
            margin-bottom: 40px;
        }
        .post-item {
            background-color: #FAE6E6; /* 更柔和的浅粉色 */
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
            padding: 20px;
            margin-bottom: 20px;
            transition: transform 0.2s;
        }
        .post-item:hover {
            transform: translateY(-5px);
        }
        .tag-input {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #D8A7A7;
            border-radius: 5px;
            outline: none;
        }
        .add-btn {
            padding: 10px;
            background-color: #D8A7A7; /* 柔和的粉色 */
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .add-btn:hover {
            background-color: #B38383; /* 深一点的粉色 */
        }
        footer {
            text-align: center;
            margin-top: 40px;
            color: #854848;
        }
    </style>
</head>
<body>
    <div class="sidebar">
        <h2>About Me</h2>
        <img src="profile.jpg" alt="Profile Picture" class="profile-img">
        <p>Hello, I'm [Your Name]. I love writing and sharing my thoughts on various topics. Welcome to my archive!</p>
    </div>

    <div class="main-content">
        <h1>Article Archive</h1>
        
        <section class="post-list">
            <h2>Articles</h2>
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
            <!-- More articles can be added here -->
        </section>

        <section class="tag-management">
            <h2>Add Tags & Archive</h2>
            <input type="text" class="tag-input" placeholder="Add new tag">
            <button class="add-btn">Add Tag</button>
        </section>

        <footer>
            <p>&copy; 2024 My Stylish Blog. All rights reserved.</p>
        </footer>
    </div>

    <script>
        // JavaScript to handle adding tags (basic example)
        document.querySelector('.add-btn').addEventListener('click', function() {
            const tagInput = document.querySelector('.tag-input');
            if (tagInput.value.trim()) {
                alert('Tag added: ' + tagInput.value);
                tagInput.value = ''; // Clear input after adding tag
            }
        });
    </script>
</body>
</html>
