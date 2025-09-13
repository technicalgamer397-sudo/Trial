<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>আমার প্রথম ওয়েবসাইট</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 40px 0;
            text-align: center;
            border-bottom-left-radius: 10px;
            border-bottom-right-radius: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }
        
        header h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
        }
        
        header p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto;
        }
        
        nav {
            background-color: #fff;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            justify-content: center;
        }
        
        nav ul li {
            padding: 15px 0;
        }
        
        nav ul li a {
            text-decoration: none;
            color: #333;
            padding: 15px 20px;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        nav ul li a:hover {
            color: #2575fc;
        }
        
        section {
            padding: 50px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            color: #2575fc;
            position: relative;
        }
        
        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: linear-gradient(to right, #6a11cb, #2575fc);
            border-radius: 2px;
        }
        
        .about-content, .services-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }
        
        .about-text, .services-list {
            flex: 1;
            min-width: 300px;
        }
        
        .service-card {
            background: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            margin-bottom: 20px;
            transition: transform 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-5px);
        }
        
        .service-card h3 {
            color: #2575fc;
            margin-bottom: 15px;
        }
        
        .btn {
            display: inline-block;
            background: linear-gradient(to right, #6a11cb, #2575fc);
            color: white;
            padding: 12px 25px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 500;
            margin-top: 20px;
            transition: all 0.3s ease;
        }
        
        .btn:hover {
            opacity: 0.9;
            transform: translateY(-2px);
        }
        
        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 30px 0;
            margin-top: 50px;
        }
        
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            header h1 {
                font-size: 2.2rem;
            }
            
            .about-content, .services-content {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>আমার প্রথম ওয়েবসাইট</h1>
            <p>HTML এবং CSS দিয়ে তৈরি একটি সহজ কিন্তু সুন্দর ওয়েবসাইট</p>
        </div>
    </header>
    
    <nav>
        <ul>
            <li><a href="#home">হোম</a></li>
            <li><a href="#about">আমার সম্পর্কে</a></li>
            <li><a href="#services">সেবাসমূহ</a></li>
            <li><a href="#contact">যোগাযোগ</a></li>
        </ul>
    </nav>
    
    <div class="container">
        <section id="about">
            <h2 class="section-title">আমার সম্পর্কে</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>আমি একজন ওয়েব ডেভেলপমেন্ট এ আগ্রহী ব্যক্তি। আমি HTML, CSS এবং JavaScript শিখছি এবং প্রাকটিস করছি। এই ওয়েবসাইটটি是我 তৈরী করা আমার প্রথম প্রজেক্ট।</p>
                    <p>ওয়েব ডেভেলপমেন্ট是一个很有趣的技能，যা দিয়ে আমি আমার চিন্তাভাবনা বাস্তবে রূপান্তর করতে পারি।</p>
                    <a href="#contact" class="btn">আমার সাথে যোগাযোগ করুন</a>
                </div>
            </div>
        </section>
        
        <section id="services">
            <h2 class="section-title">আমার সেবাসমূহ</h2>
            <div class="services-content">
                <div class="services-list">
                    <div class="service-card">
                        <h3>ওয়েব ডিজাইন</h3>
                        <p>আধুনিক এবং রেস্পন্সিভ ওয়েবসাইট ডিজাইন করি। ইউজার এক্সপেরিয়েন্স এবং ইউজার ইন্টারফেস ডিজাইনে বিশেষ গুরুত্ব দেই।</p>
                    </div>
                    <div class="service-card">
                        <h3>ফ্রন্টএন্ড ডেভেলপমেন্ট</h3>
                        <p>HTML, CSS এবং JavaScript ব্যবহার করে ওয়েবসাইটের ফ্রন্টএন্ড部分 ডেভেলপ করি।</p>
                    </div>
                    <div class="service-card">
                        <h3>ওয়েবসাইট মেইনটেনেন্স</h3>
                        <p>বিদ্যমান ওয়েবসাইট আপডেট, পরিবর্তন এবং রক্ষণাবেক্ষণের কাজ করি।</p>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="contact">
            <h2 class="section-title">যোগাযোগ</h2>
            <div class="contact-content">
                <p>আমার সাথে যোগাযোগ করতে নিচের ফর্মটি পূরণ করুন অথবা ইমেইল করুন: email@example.com</p>
                <form style="margin-top: 20px;">
                    <div style="margin-bottom: 15px;">
                        <input type="text" placeholder="আপনার নাম" style="width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 4px;">
                    </div>
                    <div style="margin-bottom: 15px;">
                        <input type="email" placeholder="আপনার ইমেইল" style="width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 4px;">
                    </div>
                    <div style="margin-bottom: 15px;">
                        <textarea placeholder="আপনার মেসেজ" rows="5" style="width: 100%; padding: 12px; border: 1px solid #ddd; border-radius: 4px;"></textarea>
                    </div>
                    <button type="submit" class="btn">মেসেজ পাঠান</button>
                </form>
            </div>
        </section>
    </div>
    
    <footer>
        <div class="container">
            <p>&copy; ২০২৩ - আমার প্রথম ওয়েবসাইট। সকল অধিকার সংরক্ষিত।</p>
        </div>
    </footer>
</body>
</html>
