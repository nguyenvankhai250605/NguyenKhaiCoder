<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Đăng nhập tài khoản</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.13.1/font/bootstrap-icons.min.css"&gt;
    <style>
        /* CSS tương tự các trang trước */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }

        .banner {
            display: flex;
            justify-content: space-between;
            gap: 10px;
            background-color: whitesmoke;
            margin: 0;
            padding: 10px 20px;
        }

            .banner img {
                width: 400px;
                height: 70px;
                margin-top: 30px;
            }

        .contact {
            line-height: 0.5;
        }

            .contact p {
                font-size: 15px;
            }

        .banner2 {
            display: flex;
            justify-content: space-between;
            padding: 5px 10px;
            gap: 10px;
            background-color: #99CC33;
        }

            .banner2 ul {
                list-style: none;
                display: flex;
                justify-content: space-between;
            }

                .banner2 ul li {
                    margin-top: 5px;
                }

                    .banner2 ul li a {
                        text-decoration: none;
                        font-size: 20px;
                        margin-right: 40px;
                        padding: 5px 10px;
                        color: black;
                    }

                .banner2 ul a i {
                    background-color: white;
                    font-size: 30px;
                    color: #ccc;
                    padding: 5px 15px;
                    margin-right: 20px;
                }

                .banner2 ul li a:hover {
                    background-color: #8EB22D;
                    transition: 0.3s;
                    border-radius: 5px;
                    color: white;
                }

        .searchbox {
            display: flex;
            gap: 5px;
            max-width: 250px;
            padding: 15px 20px;
        }

            .searchbox input {
                border: none;
                border-radius: 3px;
                flex-grow: 1;
                overflow: hidden;
                outline: none;
                padding-left: 10px;
            }

            .searchbox button {
                border: 1px solid black;
                border-radius: 3px;
                background-color: #99CC33;
                cursor: pointer;
            }

                .searchbox button:hover {
                    background-color: #8EB22D;
                    transition: 0.3s;
                    color: white;
                }

        .container {
            display: flex;
            justify-content: space-between;
            gap: 10px;
            margin: 10px;
        }

        .main-content {
            flex-grow: 1;
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        .form-group {
            margin-bottom: 15px;
        }

            .form-group label {
                display: block;
                margin-bottom: 5px;
                font-weight: bold;
            }

            .form-group input[type="text"],
            .form-group input[type="email"],
            .form-group input[type="password"],
            .form-group select {
                width: 100%;
                padding: 8px;
                box-sizing: border-box;
                border: 1px solid #ccc;
                border-radius: 4px;
            }

            .form-group button {
                background-color: #4169E1;
                color: white;
                padding: 10px 20px;
                border: none;
                border-radius: 5px;
                cursor: pointer;
                font-size: 16px;
            }

                .form-group button:hover {
                    background-color: #3A5FCD;
                    transition: 0.3s;
                }

        .sidebar {
            width: 250px;
        }

        .sidebar-info h4 {
            background-color: #99CC33;
            color: white;
            font-weight: bold;
            border-radius: 2px;
            padding: 10px;
            margin-bottom: 10px;
        }

        .sidebar-info ul {
            display: flex;
            flex-direction: column;
            margin: 0;
            padding: 0;
        }

            .sidebar-info ul li {
                list-style: none;
                padding: 10px;
                border-top: none;
                border-bottom: 1px solid #ccc;
                background-color: whitesmoke;
            }

                .sidebar-info ul li a {
                    text-decoration: none;
                    color: #1E90FF;
                    display: block;
                    font-size: 16px;
                }

        .sidebar-info li:hover {
            background-color: #f1f1f1;
        }

        .footer {
            background-color: #99CC33;
            padding: 5px;
            line-height: 0.5;
            text-align: center;
        }

            .footer p {
                color: white;
            }
    </style>
</head>
<body>
    <div style="max-width: 1200px; margin:auto">
        <div class="banner">
            <img src="/images/logo.png" alt="Logo">
            <div class="contact">
                <h5>Hà Nội</h5>
                <p>Điện thoại: 024.73007.008 - 093.4647.172</p>
                <p>Địa chỉ: Số 63/445, Lạc Long Quân, Tây Hồ, Hà Nội</p>
                <p>Email: hn@dienhoa24h.com</p>
            </div>
            <div class="contact">
                <h5>TP.Hồ Chí Minh</h5>
                <p>Điện thoại: 028.73007.008 - 094.7723.444</p>
                <p>Địa chỉ: 189 XVN Tinh, P.17, Q. Bình Thạnh</p>
                <p>Email: hcm@dienhoa24h.com</p>
            </div>
        </div>
        <div class="banner2">
            <ul>
                <li><a href="#"><i class="bi bi-house-fill"></i></a></li>
                <li><a href="#">Trang chủ</a></li>
                <li><a href="#">Đăng ký</a></li>
                <li><a href="#">Đăng nhập</a></li>
                <li><a href="#">Liên hệ</a></li>
            </ul>
            <div class="searchbox">
                <input type="text" placeholder="Search">
                <button type="submit">Search</button>
            </div>
        </div>
        <div class="container">
            <div class="main-content">
                <h2 style="text-align: center;">ĐĂNG NHẬP</h2>
                <hr />
                <form action="#" method="post">
                    <div class="form-group">
                        <label for="username">Username</label>
                        <input type="text" id="username" name="username" placeholder="Enter your username" required>
                        <p style="color: red; font-size: 0.8em; margin-top: 5px;">Must to enter your username</p>
                    </div>
                    <div class="form-group">
                        <label for="password">Password</label>
                        <input type="password" id="password" name="password" required>
                        <p style="color: red; font-size: 0.8em; margin-top: 5px;">Password include 8-16 character!</p>
                    </div>
                    <div class="form-group">
                        <label>
                            <input type="checkbox" name="remember"> Remember Password
                        </label>
                    </div>
                    <div class="form-group">
                        <button type="submit">ĐĂNG NHẬP</button>
                    </div>
                </form>
            </div>
            <div class="sidebar">
                <div class="sidebar-info">
                    <h4>HOA THEO CHỦ ĐỀ</h4>
                    <ul>
                        <li><a href="#">HOA SINH NHẬT</a></li>
                        <li><a href="#">HOA KHAI TRƯƠNG</a></li>
                        <li><a href="#">LAN HỒ ĐIỆP</a></li>
                        <li><a href="#">HOA CƯỚI</a></li>
                        <li><a href="#">HOA LAN</a></li>
                        <li><a href="#">HOA CHIA BUỒN</a></li>
                        <li><a href="#">QUÀ TẶNG</a></li>
                        <li><a href="#">TRÁI CÂY</a></li>
                    </ul>
                </div>
                <div class="sidebar-info">
                    <h4>CHỌN THEO GIÁ</h4>
                    <ul>
                        <li><a href="#">250.000đ trở xuống</a></li>
                        <li><a href="#">250.000đ - 400.000đ</a></li>
                        <li><a href="#">400.000đ - 600.000đ</a></li>
                        <li><a href="#">600.000đ - 900.000đ</a></li>
                        <li><a href="#">Trên 1.000.000đ</a></li>
                    </ul>
                </div>
            </div>
        </div>
        <footer class="footer">
            <p>Liên hệ: Khoa Công Nghệ Thông Tin - Trường Đại Học Công Nghiệp Thực Phẩm Tp.HCM Link: fanpage và link: youtube</p>
            <p>Địa chỉ: 140 Lê Trọng Tấn, Phường Tây Thạnh, Quận Tân Phú, Tp.HCM. ĐT: (028) 38161673 (ext 136) Mail: kcntt@hufi.edu.vn</p>
        </footer>
        </div>
</body>
</html>
