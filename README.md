<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Portfolio | ณฐพร รัศมิทัต</title> 

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Arial", sans-serif;
        }

        body {
            background-color: #f1f8f1;
            color: #234d20;
        }

        /* แถบเมนู */
        nav {
            background-color: #2e7d32;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav h2 {
            color: white;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin-left: 25px;
            font-weight: bold;
        }

        nav a:hover {
            color: #dcedc8;
        }

        /* หน้าหลัก */
        .hero {
            min-height: 90vh;
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 40px 20px;
            background: linear-gradient(
                135deg,
                #e8f5e9,
                #c8e6c9
            );
        }

        .hero-content {
            max-width: 800px;
        }

        .profile-img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            border: 6px solid #2e7d32;
            margin-bottom: 25px;
        }

        .hero h1 {
            font-size: 42px;
            color: #1b5e20;
            margin-bottom: 15px;
        }

        .hero h3 {
            font-size: 22px;
            color: #388e3c;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 18px;
            line-height: 1.8;
        }

        .btn {
            display: inline-block;
            margin-top: 25px;
            padding: 12px 28px;
            background-color: #2e7d32;
            color: white;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
        }

        .btn:hover {
            background-color: #1b5e20;
        }

        /* ส่วนต่าง ๆ */
        section {
            padding: 70px 10%;
        }

        section h2 {
            text-align: center;
            color: #1b5e20;
            font-size: 32px;
            margin-bottom: 40px;
        }

        /* เกี่ยวกับฉัน */
        .about {
            background-color: white;
        }

        .about-box {
            max-width: 850px;
            margin: auto;
            background-color: #f1f8f1;
            padding: 35px;
            border-radius: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
            text-align: center;
            line-height: 2;
            font-size: 18px;
        }

        /* เป้าหมายการศึกษา */
        .education {
            background-color: #e8f5e9;
        }

        .education-box {
            max-width: 850px;
            margin: auto;
            background: white;
            padding: 35px;
            border-left: 8px solid #2e7d32;
            border-radius: 15px;
            line-height: 2;
            font-size: 18px;
        }

        .education-box strong {
            color: #1b5e20;
        }

        /* ความสามารถและงานอดิเรก */
        .skills {
            background-color: white;
        }

        .card-container {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
        }

        .card {
            width: 260px;
            padding: 30px 20px;
            text-align: center;
            background-color: #f1f8f1;
            border-radius: 20px;
            border: 2px solid #a5d6a7;
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 8px 20px rgba(46,125,50,0.2);
        }

        .card .icon {
            font-size: 45px;
            margin-bottom: 15px;
        }

        .card h3 {
            color: #2e7d32;
            margin-bottom: 10px;
        }

        /* เป้าหมาย */
        .goal {
            background-color: #e8f5e9;
            text-align: center;
        }

        .goal p {
            max-width: 750px;
            margin: auto;
            font-size: 19px;
            line-height: 2;
        }

        /* Footer */
        footer {
            background-color: #1b5e20;
            color: white;
            text-align: center;
            padding: 25px;
        }

        /* รองรับมือถือ */
        @media (max-width: 768px) {

            nav {
                flex-direction: column;
                gap: 10px;
            }

            nav a {
                margin-left: 10px;
                margin-right: 10px;
            }

            .hero h1 {
                font-size: 32px;
            }

            .hero h3 {
                font-size: 18px;
            }

            section {
                padding: 50px 6%;
            }
        }
    </style>
</head>

<body>

    <!-- เมนู -->
    <nav>
        <h2>PORTFOLIO</h2>

        <div>
            <a href="#home">หน้าแรก</a>
            <a href="#about">เกี่ยวกับฉัน</a>
            <a href="#education">การศึกษา</a>
            <a href="#skills">ความสามารถ</a>
            <a href="#goal">เป้าหมาย</a>
        </div>
    </nav>


    <!-- หน้าแรก -->
    <section class="hero" id="home">

        <div class="hero-content">

            <!-- ถ้ามีรูปตัวเอง ให้เปลี่ยนชื่อไฟล์เป็นรูปของเรา -->
            <img src="profile.jpg" class="profile-img" alt="รูปณฐพร">

            <h1>นางสาวณฐพร รัศมิทัต</h1>

            <h3>นักเรียนชั้นมัธยมศึกษาปีที่ 6</h3>

            <p>
                โรงเรียนเซนต์โยเซฟทิพวัล
            </p>

            <p>
                Portfolio เพื่อศึกษาต่อ
                มหาวิทยาลัยเกษตรศาสตร์ บางเขน
            </p>

            <a href="#about" class="btn">รู้จักฉันมากขึ้น</a>

        </div>

    </section>


    <!-- เกี่ยวกับฉัน -->
    <section class="about" id="about">

        <h2>เกี่ยวกับฉัน</h2>

        <div class="about-box">

            <p>
                สวัสดีค่ะ ดิฉันชื่อ
                <strong>นางสาวณฐพร รัศมิทัต</strong>
            </p>

            <p>
                ปัจจุบันกำลังศึกษาอยู่ชั้นมัธยมศึกษาปีที่ 6
                โรงเรียนเซนต์โยเซฟทิพวัล
            </p>

            <p>
                ดิฉันเป็นคนที่มีความสนใจด้านการบริหารธุรกิจ
                และมีความตั้งใจที่จะศึกษาต่อในระดับมหาวิทยาลัย
                เพื่อพัฒนาความรู้และทักษะสำหรับการทำงานในอนาคต
            </p>

        </div>

    </section>


    <!-- การศึกษา -->
    <section class="education" id="education">

        <h2>เป้าหมายการศึกษาต่อ</h2>

        <div class="education-box">

            <p>
                <strong>มหาวิทยาลัยที่ต้องการเข้าศึกษา</strong><br>
                มหาวิทยาลัยเกษตรศาสตร์ วิทยาเขตบางเขน
            </p>

            <br>

            <p>
                <strong>คณะ</strong><br>
                คณะบริหารธุรกิจ
            </p>

            <br>

            <p>
                <strong>สาขาวิชา</strong><br>
                การบัญชี
            </p>

            <br>

            <p>
                <strong>ภาควิชา</strong><br>
                ภาควิชาบัญชี
            </p>

        </div>

    </section>


    <!-- ความสามารถและงานอดิเรก -->
    <section class="skills" id="skills">

        <h2>ความสามารถและงานอดิเรก</h2>

        <div class="card-container">

            <!-- ความสามารถพิเศษ -->
            <div class="card">

                <div class="icon">🧁</div>

                <h3>ความสามารถพิเศษ</h3>

                <p>
                    ทำขนม
                </p>

            </div>


            <!-- งานอดิเรก 1 -->
            <div class="card">

                <div class="icon">🎧</div>

                <h3>งานอดิเรก</h3>

                <p>
                    ฟังเพลง
                </p>

            </div>


            <!-- งานอดิเรก 2 -->
            <div class="card">

                <div class="icon">🎬</div>

                <h3>งานอดิเรก</h3>

                <p>
                    ดูหนัง
                </p>

            </div>

        </div>

    </section>


    <!-- เป้าหมาย -->
    <section class="goal" id="goal">

        <h2>เป้าหมายในอนาคต</h2>

        <p>
            ดิฉันมีความมุ่งมั่นที่จะเข้าศึกษาต่อ
            คณะบริหารธุรกิจ สาขาวิชาการบัญชี
            ภาควิชาบัญชี มหาวิทยาลัยเกษตรศาสตร์
            วิทยาเขตบางเขน เพื่อพัฒนาความรู้
            ความสามารถ และประสบการณ์ด้านการบัญชี
            และนำความรู้ไปประยุกต์ใช้ในการประกอบอาชีพในอนาคต
        </p>

    </section>


    <!-- ส่วนท้าย -->
    <footer>

        <p>
            © 2026 Portfolio | นางสาวณฐพร รัศมิทัต
        </p>

        <p>
            โรงเรียนเซนต์โยเซฟทิพวัล
        </p>

    </footer>

</body>
</html>
