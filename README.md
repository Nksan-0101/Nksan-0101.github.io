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
            height: 100vh;
            overflow: hidden;
            color: var(--primary-color);
        }
        .sidebar {
            background-color: var(--light-bg-color);
            width: 25%;
            padding: 20px;
            box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .main-content {
            background-color: var(--card-bg-color);
            width: 75%;
            padding: 40px;
            overflow-y: auto;
            box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.05);
        }
        h1, h2, h3 {
            color: var(--primary-color);
            margin-bottom: 10px;
        }
        .profile-img {
            width: 150px;
            height: 150px;
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
            transition: transform 0.2s, box-shadow 0.2s;
        }
        .post-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        .tag-input {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid var(--accent-color);
            border-radius: 5px;
            outline: none;
            transition: border-color 0.3s;
        }
        .tag-input:focus {
            border-color: var(--primary-color);
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
