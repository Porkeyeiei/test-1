<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>All Institute</title>
    <style>
        /* Reset some default styles */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Sarabun', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f1f8e9;
            color: #2e7d32;
        }

        header {
            background-color: #388e3c;
            color: white;
            text-align: center;
            padding: 1.5rem;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }

        header h1 {
            font-size: 2.5rem;
            animation: slideIn 1.5s ease-in-out;
        }

        @keyframes slideIn {
            from {
                transform: translateY(-100%);
            }
            to {
                transform: translateY(0);
            }
        }

        /* Navigation Bar */
        nav {
            background-color: #66bb6a;
            padding: 0.8rem;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
        }

        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        nav ul li {
            display: inline;
            margin-right: 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 1.2rem;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        nav ul li a:hover {
            color: #004d40;
        }

        main {
            padding: 20px;
            max-width: 1200px;
            margin: 20px auto;
        }

        h2 {
            font-size: 2rem;
            color: #43a047;
            border-bottom: 3px solid #43a047;
            margin-bottom: 20px;
        }

        /* Institution Cards */
        .institution {
            background-color: white;
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 25px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .institution h3 {
            color: #2e7d32;
            font-size: 1.8rem;
            margin-bottom: 10px;
            position: relative;
            z-index: 2;
        }

        .institution ul {
            padding-left: 20px;
            font-size: 1.1rem;
            z-index: 2;
            position: relative;
        }

        .institution:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
        }

        /* Floating animation */
        .institution::before {
            content: '';
            background-image: url('https://www.example.com/bg-pattern.svg');
            background-size: cover;
            background-position: center;
            position: absolute;
            top: -50px;
            left: -50px;
            width: 150px;
            height: 150px;
            opacity: 0.2;
            transform: rotate(45deg);
            z-index: 1;
        }

        footer {
            background-color: #43a047;
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 40px;
            position: relative;
            bottom: 0;
            width: 100%;
            box-shadow: 0px -2px 6px rgba(0, 0, 0, 0.1);
        }

        footer p {
            margin: 0;
            font-size: 1rem;
        }

        .section-container {
            margin-top: 40px;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }

            nav ul li {
                display: block;
                margin-bottom: 10px;
            }

            .institution {
                padding: 15px;
            }

            .institution h3 {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>ค้นหาจุดสีเขียว</h1>
    </header>

    <nav>
        <ul>
            <li><a href="#">หน้าแรก</a></li>
            <li><a href="#universities">รายชื่อมหาวิทยาลัย</a></li>
            <li><a href="#schools">รายชื่อโรงเรียน</a></li>
            <li><a href="#">เกี่ยวกับเรา</a></li>
            <li><a href="#">ติดต่อ</a></li>
        </ul>
    </nav>

    <main>
        <!-- หมวดหมู่มหาวิทยาลัย -->
        <div class="section-container" id="universities">
            <h2>รายชื่อมหาวิทยาลัย</h2>

            <div class="institution">
                <h3>มหาวิทยาลัยธรรมศาสตร์</h3>
                <ul>
                    <li><strong>ที่อยู่:</strong> 99 หมู่ 18 ถ.พหลโยธิน ต.คลองหนึ่ง อ.คลองหลวง จ.ปทุมธานี 12121</li>
                    <li><strong>เว็บไซต์:</strong> <a href="https://www.tu.ac.th" target="_blank">www.tu.ac.th</a></li>
                </ul>
            </div>

            <div class="institution">
                <h3>มหาวิทยาลัยเชียงใหม่</h3>
                <ul>
                    <li><strong>ที่อยู่:</strong> 239 ถ.ห้วยแก้ว ต.สุเทพ อ.เมืองเชียงใหม่ จ.เชียงใหม่ 50200</li>
                    <li><strong>เว็บไซต์:</strong> <a href="https://www.cmu.ac.th" target="_blank">www.cmu.ac.th</a></li>
                </ul>
            </div>

            <div class="institution">
                <h3>มหาวิทยาลัยมหิดล</h3>
                <ul>
                    <li><strong>ที่อยู่:</strong> 999 ถ.พุทธมณฑลสาย 4 ต.ศาลายา อ.พุทธมณฑล จ.นครปฐม 73170</li>
                    <li><strong>เว็บไซต์:</strong> <a href="https://www.mahidol.ac.th" target="_blank">www.mahidol.ac.th</a></li>
                </ul>
            </div>
        </div>

        <!-- หมวดหมู่โรงเรียน -->
        <div class="section-container" id="schools">
            <h2>รายชื่อโรงเรียน</h2>

            <div class="institution">
                <h3>โรงเรียนสวนกุหลาบวิทยาลัย</h3>
                <ul>
                    <li><strong>ที่อยู่:</strong> 88 ถ.ตรีเพชร แขวงวังบูรพาภิรมย์ เขตพระนคร กรุงเทพฯ 10200</li>
                    <li><strong>เว็บไซต์:</strong> <a href="https://www.sk.ac.th" target="_blank">www.sk.ac.th</a></li>
                </ul>
            </div>

            <div class="institution">
                <h3>โรงเรียนเตรียมอุดมศึกษา</h3>
                <ul>
                    <li><strong>ที่อยู่:</strong> 227 ถ.พญาไท แขวงปทุมวัน เขตปทุมวัน กรุงเทพฯ 10330</li>
                    <li><strong>เว็บไซต์:</strong> <a href="https://www.triamudom.ac.th" target="_blank">www.triamudom.ac.th</a></li>
                </ul>
            </div>

            <div class="institution">
                <h3>โรงเรียนอัสสัมชัญ</h3>
                <ul>
                    <li><strong>ที่อยู่:</strong> 26 ซอยสาทร 11 ถ.สาทรใต้ แขวงยานนาวา เขตสาทร กรุงเทพฯ 10120</li>
                    <li><strong>เว็บไซต์:</strong> <a href="
