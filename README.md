THIẾT KẾ WEBSITE TIN TỨC VỀ GAME VÀ CÔNG NGHỆ:

CÔNG CỤ THIẾT KẾ: FIGMA

MỤC TIÊU:

CẬP NHẬT THÔNG TIN VỀ CÔNG NGHỆ VÀ GAME

TRANG CHỦ HIỂN THỊ TIN TỨC MỚI, LỊCH SỬ ĐỌC HIỂN THỊ NHỮNG TIN ĐÃ ĐỌC

<img width="779" height="796" alt="image" src="https://github.com/user-attachments/assets/7b88bf71-083b-470d-a789-f098dbcb3f12" />

CÔNG CỤ A.I HỖ TRỢ: GG STUDIO

Promp: "dựa vào ảnh giao diện và đoạn code html sau, giúp tôi thêm đoạn code css vào để có giao diện giống nhất với giao diện mẫu"
```
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Social Feed - Trang Chủ</title>
    <!-- GIỮ NGUYÊN: Các liên kết thư viện và CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="./css/style.css">
</head>
<body>

    <header id="main-header">
        <!-- GIỮ NGUYÊN: Thanh tìm kiếm -->
        <div class="search-bar">
            <i class="fa fa-search"></i>
            <input type="text" placeholder="Search">
            <kbd>Ctrl + K</kbd>
        </div>
        
        <nav class="user-nav">
            <!-- GIỮ NGUYÊN: Nút chuông thông báo -->
            <button class="btn-bell">
                <i class="fa-regular fa-bell"></i>
                <span class="notification-badge">1</span>
            </button>

            <div class="status-capsule">
                <!-- GIỮ NGUYÊN: Các chỉ số Streak, Credits, Energy -->
                <div class="status-item">
                    <img src="./img/SVG.png" alt="streak" class="status-icon">
                    <span class="status-value color-pink">0</span>
                </div>
                <div class="status-item">
                    <img src="./img/icon.png" alt="credits" class="status-icon">
                    <span class="status-value">0</span>
                </div>
                <div class="status-item">
                    <img src="./img/icon2.png" alt="energy" class="status-icon">
                    <span class="status-value">10</span>
                </div>

                <!-- THÊM VÀO: Thẻ <a> bao quanh Avatar để nhấp vào sang trang cá nhân -->
                <a href="thongtin.html" class="user-avatar-wrapper">
                    <img src="./img/avt.png" alt="user" class="user-avatar">
                    <span class="online-dot"></span>
                </a>
            </div>
        </nav>
    </header>

    <div class="app-container">
        <!-- GIỮ NGUYÊN: Toàn bộ Sidebar trái -->
        <aside id="left-sidebar">
            <button class="btn-new-post">+ New post</button>
            <nav class="menu-section">
                <a href="trangchu.html" class="menu-item active"><i class="fa fa-home"></i> For You</a>
                <a href="#" class="menu-item"><i class="fa fa-users"></i> Following</a>
                <a href="#" class="menu-item"><i class="fa fa-clock-rotate-left"></i> History</a>
            </nav>
            <section class="menu-section">
                <p class="section-title">Groups</p>
                <a href="#" class="menu-item">Game Developers</a>
                <a href="#" class="menu-item">Machine Learning News</a>
            </section>
        </aside>

        <main id="main-feed">
            <div class="feed-wrapper">
                <!-- GIỮ NGUYÊN: Header của Feed -->
                <header class="feed-header">
                    <h3>For you</h3>
                    <button class="btn-settings">Feed settings <i class="fa fa-sliders"></i></button>
                </header>

                <section class="posts-list">
                    <!-- BÀI VIẾT 1 -->
                    <article class="post-card">
                        <div class="post-user">
                            <!-- THÊM VÀO: Thẻ <a> bọc avatar nhỏ trong bài viết -->
                            <a href="thongtin.html">
                                <div class="avatar-small"></div>
                            </a>
                            <div class="user-info">
                                <h4>Tên người đăng</h4>
                                <time>Thời gian đăng</time>
                            </div>
                        </div>

                        <div class="post-body">
                            <div class="post-content">
                                <!-- THÊM VÀO: Thẻ <a> bọc tiêu đề h2 để sang baiviet.html -->
                                <h2><a href="baiviet.html">Bài viết 1</a></h2>
                            </div>
                            
                            <!-- THÊM VÀO: Thẻ <a> bọc ảnh bài viết để sang baiviet.html -->
                            <a href="baiviet.html" class="post-img-link">
                                <img src="./img/Post image.png" alt="Post 1" class="post-image">
                            </a>
                        </div>
                    </article>

                        <!-- BÀI VIẾT 2 -->
                    <article class="post-card">
                        <div class="post-user">
                            <!-- THÊM VÀO: Thẻ <a> bọc avatar nhỏ trong bài viết -->
                            <a href="thongtin.html">
                                <div class="avatar-small"></div>
                            </a>
                            <div class="user-info">
                                <h4>Tên người đăng</h4>
                                <time>Thời gian đăng</time>
                            </div>
                        </div>

                        <div class="post-body">
                            <div class="post-content">
                                <!-- THÊM VÀO: Thẻ <a> bọc tiêu đề h2 để sang baiviet.html -->
                                <h2><a href="baiviet.html">Bài viết 2</a></h2>
                            </div>
                            
                            <!-- THÊM VÀO: Thẻ <a> bọc ảnh bài viết để sang baiviet.html -->
                            <a href="baiviet.html" class="post-img-link">
                                <img src="./img/Post image.png" alt="Post 1" class="post-image">
                            </a>
                        </div>

                        <!-- GIỮ NGUYÊN: Các nút tương tác Upvote, Comment... -->
                        <footer class="post-actions">
                            <div class="action-item"><i class="fa fa-arrow-up"></i> 45 <i class="fa fa-arrow-down"></i></div>
                            <div class="action-item"><i class="fa-regular fa-comment"></i></div>
                            <div class="action-item"><i class="fa-regular fa-bookmark"></i></div>
                            <div class="action-item"><i class="fa-share-nodes"></i></div>
                        </footer>
                    </article>
                </section>
            </div>
        </main>
    </div>
    
    <!-- GIỮ NGUYÊN: Nút cuộn lên đầu trang -->
    <div class="scroll-top"><i class="fa fa-chevron-up"></i></div>

</body>
</html>
```
<img width="779" height="796" alt="image" src="https://github.com/user-attachments/assets/1be9b232-43d3-40db-b594-e386e02b3085" />

link: https://nptb.github.io/myweb.github.io/myweb/trangchu.html
