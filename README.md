
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>清朗学风·学润德馨</title>
    <style>
                * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Microsoft YaHei", "SimSun", sans-serif;
        }

        body {
            background: #f8f9fa;
            color: #333;
            line-height: 1.8;
        }

        .container {
            width: 85%;
            max-width: 1200px;
            margin: 0 auto;
        }

      
        header {
            background: linear-gradient(135deg, #2c3e50, #3498db);
            padding: 1rem 0;
            box-shadow: 0 2px 15px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            color: white;
        }

        .logo img {
            width: 60px;
            margin-right: 15px;
        }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            padding: 5px 10px;
            border-radius: 4px;
            transition: all 0.3s;
        }

        .nav-links a:hover {
            background: rgba(255,255,255,0.2);
        }

       
        .banner {
            height: 500px;
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
                        url('https://images.unsplash.com/photo-1581726707445-75cbe4efc586') center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
        }

        .banner-content h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
        }

        
        .section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 2.5rem;
            color: #2c3e50;
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background: #3498db;
        }

        .content-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .content-img {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .content-img img {
            width: 100%;
            height: auto;
            display: block;
            transition: transform 0.5s;
        }

        .content-img:hover img {
            transform: scale(1.05);
        }

        
        .timeline {
            position: relative;
            padding: 50px 0;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 50%;
            width: 4px;
            height: 100%;
            background: #3498db;
        }

        .timeline-item {
            width: 45%;
            padding: 20px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            margin: 20px 0;
            position: relative;
        }

        .timeline-item:nth-child(odd) {
            margin-left: 55%;
        }

        .timeline-item:nth-child(even) {
            margin-right: 55%;
        }

        .timeline-date {
            position: absolute;
            top: 20px;
            color: #3498db;
            font-weight: bold;
        }

        .timeline-item:nth-child(odd) .timeline-date {
            right: calc(100% + 30px);
        }

        .timeline-item:nth-child(even) .timeline-date {
            left: calc(100% + 30px);
        }

      
        .card-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-10px);
        }

        .card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .card-content {
            padding: 20px;
        }

        .card-tag {
            display: inline-block;
            background: #3498db;
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            margin-bottom: 15px;
        }

       
        footer {
            background: #2c3e50;
            color: white;
            padding: 60px 0 20px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
        }

        .footer-section h3 {
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid #3498db;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-links a {
            width: 40px;
            height: 40px;
            background: #34495e;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: all 0.3s;
        }

        .social-links a:hover {
            background: #3498db;
        }

        
        @media (max-width: 768px) {
            .content-grid {
                grid-template-columns: 1fr;
            }

            .nav-links {
                display: none;
            }

            .timeline::before {
                left: 20px;
            }

            .timeline-item {
                width: calc(100% - 40px);
                margin: 20px 0 !important;
            }

            .timeline-date {
                position: static;
                margin-bottom: 10px;
            }
        }
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <header>
        <div class="container">
            <nav>
                <div class="logo">
                    <img src="https://tse1-mm.cn.bing.net/th/id/OIP-C.YcgKnleNsDPXNEisoUliowHaHa?w=171&h=180&c=7&r=0&o=5&dpr=1.5&pid=1.7.png" alt="校徽">
                    <h1>清朗学风</h1>
                </div>
                <div class="nav-links">
                    <a href="#home">首页</a>
                    <a href="#about">建设方案</a>
                    <a href="#activity">学术活动</a>
                    <a href="#culture">文化传承</a>
                </div>
            </nav>
        </div>
    </header>

    <!-- 横幅区 -->
    <section class="banner" id="home">
        <div class="container">
            <div class="banner-content">
                <h1>清朗学风 · 学润德馨</h1>
                <p>营造良好学术生态，培育德才兼备人才</p>
            </div>
        </div>
    </section>

    <!-- 建设方案 -->
    <section class="section" id="about">
        <div class="container">
            <div class="section-title">
                <h2>学风建设方案</h2>
                <p>构建四位一体的学风建设体系</p>
            </div>

            <div class="content-grid">
                <div class="content-img">
                    <img src="https://tse2-mm.cn.bing.net/th/id/OIP-C.-I5wX02h2gJ_09TKblyjzgHaLH?w=202&h=303&c=7&r=0&o=5&dpr=1.5&pid=1.7.jpg" alt="学风建设">
                </div>
                <div class="content-text">
                    <h3>建设目标</h3>
                    <p>通过"制度保障、文化浸润、实践养成、榜样引领"四大工程，打造求真务实的廉洁学术环境：</p>
                    <ul>
                        <li>建立学术诚信档案系统</li>
                        <li>开设诚信文化必修课程</li>
                        <li>实施廉洁创新培育计划</li>
                        <li>开展"廉洁之星"评选活动</li>
                    </ul>
                    <button class="btn">查看详情</button>
                </div>
            </div>
        </div>
    </section>

    <!-- 时间轴 -->
    <section class="section timeline-section">
        <div class="container">
            <div class="section-title">
                <h2>建设进程</h2>
                <p>2024-2025学年学风建设路线图</p>
            </div>

            <div class="timeline">
                <div class="timeline-item">
                    <div class="timeline-date">2024.09</div>
                    <h3>廉洁教育月</h3>
                    <p>开展学术规范专题讲座，建立学生学术诚信档案</p>
                </div>

                <div class="timeline-item">
                    <div class="timeline-date">2024.11</div>
                    <h3>文化传承季</h3>
                    <p>举办国学经典诵读大赛、传统文化工作坊</p>
                </div>

                <div class="timeline-item">
                    <div class="timeline-date">2025.03</div>
                    <h3>廉洁创新实践周</h3>
                    <p>开展跨学科廉洁创新项目，举办科研成果展</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 成果展示 -->
    <section class="section" id="activity">
        <div class="container">
            <div class="section-title">
                <h2>成果展示</h2>
                <p>近期学术活动剪影</p>
            </div>

            <div class="card-container">
                <div class="card">
                    <img src="https://tse2-mm.cn.bing.net/th/id/OIP-C.4Th9pwof21UNnEemVoTNpgHaEK?w=306&h=180&c=7&r=0&o=5&dpr=1.5&pid=1.7.jpg" alt="学术讲座">
                    <div class="card-content">
                        <span class="card-tag">学术讲座</span>
                        <h3>学术规范与论文写作</h3>
                        <p>特邀知名学者讲解学术研究方法论</p>
                    </div>
                </div>

                <div class="card">
                    <img src="https://tse3-mm.cn.bing.net/th/id/OIP-C.EwdTrQiWKXpfZtqXbAdiWQHaFj?w=225&h=180&c=7&r=0&o=5&dpr=1.5&pid=1.7.jpg" alt="文化展览">
                    <div class="card-content">
                        <span class="card-tag">文化展览</span>
                        <h3>传统典籍特展</h3>
                        <p>展出明清古籍善本及现代研究成果</p>
                    </div>
                </div>

                <div class="card">
                    <img src="https://tse1-mm.cn.bing.net/th/id/OIP-C.NSDa67_4O-ntZ93yBliEmgHaDt?w=338&h=175&c=7&r=0&o=5&dpr=1.5&pid=1.7.jpg" alt="科研实践">
                    <div class="card-content">
                        <span class="card-tag">科研实践</span>
                        <h3>实验开放日</h3>
                        <p>展示最廉洁新科研成果，体验前沿科技与人文情怀</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>联系我们</h3>
                    <p>地址：安徽师范大学计算机与信息学院</p>
                    <p>电话：19719853767</p>
                    <p>邮箱：2823423720@qq.com</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-weixin"></i></a>
                        <a href="#"><i class="fab fa-weibo"></i></a>
                        <a href="#"><i class="fab fa-qq"></i></a>
                    </div>
                </div>

                <div class="footer-section">
                    <h3>快速链接</h3>
                    <ul>
                        <li><a href="#home">学风建设规范</a></li>
                        <li><a href="#activity">学术活动日历</a></li>
                        <li><a href="#culture">文化传承资源</a></li>
                    </ul>
                </div>

                <div class="footer-section">
                    <h3>合作伙伴</h3>
                    <ul>
                        <li>国家教育发展中心</li>
                        <li>高校学术联盟</li>
                        <li>传统文化研究会</li>
                    </ul>
                </div>
            </div>
            <div class="copyright">
                <p>© 2025 计信学院 版权所有</p>
            </div>
        </div>
    </footer>

    <!-- Font Awesome -->
    <script src="https://kit.fontawesome.com/your-kit-code.js"></script>
</body>
</html>
