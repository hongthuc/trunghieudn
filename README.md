<!-- 
  WEBSITE: TRUNGHIEUDN.COM - CÔNG TY TNHH TRUNG HIẾU ĐN
  CHUYÊN VẬN CHUYỂN XE CƠ GIỚI - MÁY CÔNG TRÌNH BẮC TRUNG NAM
  GIAO DIỆN CHUẨN FLATSOME ĐƠN GIẢN - TỐI ƯU 95% MÀN HÌNH MÁY TÍNH & 2 CỘT ĐIỆN THOẠI
  (Đã xóa dòng khai báo doctype theo đúng yêu cầu)
-->
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">
  <title>CÔNG TY TNHH TRUNG HIẾU ĐN | Chuyên Vận Chuyển Xe Cơ Giới - trunghieudn.com</title>
  <meta name="description" content="CÔNG TY TNHH TRUNG HIẾU ĐN (trunghieudn.com) chuyên vận chuyển xe cơ giới, máy công trình, máy xúc, máy đào, xe lu, máy ủi, cẩu bánh xích bằng xe fooc lùn, moóc rút chuyên dụng tại Đà Nẵng và Bắc - Nam. Hotline: 0961.797.119">
  
  <!-- Open Graph / Thumbnail là ảnh Logo trang web khi gửi link chia sẻ -->
  <meta property="og:type" content="website">
  <meta property="og:url" content="https://trunghieudn.com/">
  <meta property="og:title" content="CÔNG TY TNHH TRUNG HIẾU ĐN - Chuyên Vận Chuyển Xe Cơ Giới">
  <meta property="og:description" content="Đội xe Fooc lùn, Moóc rút chuyên chở xe cơ giới, máy xúc, xe đào, xe lu, hàng siêu trường siêu trọng toàn quốc. Đ/c: 58 Nguyễn Hữu Hào, P. Ngũ Hành Sơn, TP Đà Nẵng. ĐT: 0961.797.119">
  <meta property="og:image" id="og-logo-meta" content="https://drive.google.com/thumbnail?id=1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD&sz=w800">
  <link rel="image_src" id="link-logo-thumb" href="https://drive.google.com/thumbnail?id=1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD&sz=w800">

  <!-- Google Fonts: Inter chuẩn Flatsome hiện đại -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">
  
  <!-- FontAwesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <!-- Tailwind CSS -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
          },
          colors: {
            brand: {
              dark: '#0a2540',     /* Xanh Navy đậm theo màu Logo */
              primary: '#0f3e78',  /* Xanh Công nghiệp chủ đạo theo Logo */
              light: '#1d5ba6',    /* Xanh sáng */
              accent: '#f59e0b',   /* Vàng Cam cơ giới theo màu Logo */
              orange: '#ea580c',   /* Cam đậm điểm nhấn */
              bg: '#f4f6f9'        /* Nền xám sáng chuẩn Flatsome */
            }
          }
        }
      }
    }
  </script>

  <style>
    /* Khóa tràn viền ngang tuyệt đối - Không lệch phải trên mọi thiết bị */
    *, *::before, *::after {
      box-sizing: border-box;
    }
    html, body {
      width: 100%;
      max-width: 100%;
      overflow-x: hidden;
      margin: 0;
      padding: 0;
      font-family: 'Inter', sans-serif;
      background-color: #f4f6f9;
      color: #1e293b;
      scroll-behavior: smooth;
    }

    /* Container chuẩn Flatsome: 95% chiều ngang trên máy tính, căn giữa tuyệt đối */
    .flatsome-container {
      width: 96%;
      max-width: 96%;
      margin-left: auto;
      margin-right: auto;
    }
    @media (min-width: 1024px) {
      .flatsome-container {
        width: 95%;
        max-width: 95%;
        margin-left: auto;
        margin-right: auto;
      }
    }

    /* Tiêu đề Section chuẩn Flatsome UX Builder (Section Title Normal / Center) */
    .flatsome-section-title {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: space-between;
      border-bottom: 2px solid #e2e8f0;
      margin-bottom: 1rem;
      padding-bottom: 0.5rem;
    }
    .flatsome-section-title h2 {
      position: relative;
      font-weight: 800;
      text-transform: uppercase;
      color: #0f3e78;
      margin: 0;
    }
    .flatsome-section-title h2::after {
      content: '';
      position: absolute;
      bottom: -0.6rem;
      left: 0;
      width: 100%;
      height: 3px;
      background-color: #f59e0b;
    }

    /* Danh mục chữ nhỏ gọn, tuyệt đối không xuống dòng bên trong tên danh mục */
    .cat-pill-item {
      white-space: nowrap !important;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      transition: all 0.2s ease;
      line-height: 1.2;
    }
    .cat-pill-item.active,
    .cat-pill-item:hover {
      background-color: #0f3e78;
      color: #ffffff;
      border-color: #0f3e78;
    }

    /* Tên sản phẩm: hiển thị đầy đủ 100% chữ, tự xuống dòng gọn trong khung, không bị cắt chữ (...) và không tràn viền */
    .product-title-full {
      word-break: break-word;
      overflow-wrap: break-word;
      white-space: normal;
      line-height: 1.38;
      display: block;
    }

    /* Hiệu ứng rung nhẹ cho nút Hotline nổi */
    @keyframes phoneRing {
      0%, 100% { transform: rotate(0deg) scale(1); }
      15% { transform: rotate(-14deg) scale(1.06); }
      30% { transform: rotate(14deg) scale(1.06); }
      45% { transform: rotate(-10deg) scale(1.04); }
      60% { transform: rotate(10deg) scale(1.04); }
      75% { transform: rotate(0deg) scale(1); }
    }
    .animate-ring {
      animation: phoneRing 2.2s infinite ease-in-out;
    }
  </style>
</head>
<body class="min-h-screen flex flex-col justify-between">

  <!-- ==================== TOP BAR ĐƠN GIẢN CHUẨN FLATSOME ==================== -->
  <div class="bg-brand-dark text-white text-[11px] sm:text-xs py-1.5 border-b border-brand-light/30">
    <div class="flatsome-container flex flex-wrap items-center justify-between gap-2">
      <div class="flex items-center gap-2 truncate">
        <i class="fa-solid fa-location-dot text-brand-accent shrink-0"></i>
        <span class="truncate">Đ/c: 58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng</span>
      </div>
      <div class="hidden md:flex items-center gap-4 shrink-0">
        <span><i class="fa-solid fa-globe text-brand-accent mr-1"></i>Website: <strong>trunghieudn.com</strong></span>
        <span><i class="fa-solid fa-phone-volume text-brand-accent mr-1"></i>Hotline/Zalo: <strong class="text-brand-accent">0961.797.119</strong></span>
      </div>
    </div>
  </div>

  <!-- ==================== HEADER CHÍNH (LOGO GỌN NHỎ - MENU 1 HÀNG - KHÔNG ĐỂ NÚT GỌI NGAY) ==================== -->
  <header class="bg-white sticky top-0 z-40 shadow-sm border-b border-slate-200">
    <div class="flatsome-container py-2 flex items-center justify-between gap-2">
      
      <!-- LOGO CHUYÊN NGHIỆP - CHỈNH GỌN NHỎ LẠI -->
      <a href="#trang-chu" class="flex items-center gap-2 shrink-0 group focus:outline-none">
        <div class="w-9 h-9 sm:w-10 sm:h-10 rounded-lg bg-brand-primary flex items-center justify-center border-2 border-brand-accent shadow-sm shrink-0 overflow-hidden">
          <!-- Vector Logo Xe Fooc Lùn Chở Xe Cơ Giới Trung Hiếu ĐN -->
          <svg class="w-7 h-7" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
            <rect width="64" height="64" rx="10" fill="#0f3e78"/>
            <!-- Cần máy xúc cơ giới màu vàng cam -->
            <path d="M16 36L24 20L36 16L40 24L30 27" stroke="#f59e0b" stroke-width="4" stroke-linecap="round" stroke-linejoin="round"/>
            <rect x="13" y="30" width="14" height="9" rx="2" fill="#f59e0b"/>
            <!-- Thân xe đầu kéo & Fooc lùn -->
            <path d="M8 43H44V39H54L58 44V48H8V43Z" fill="#ffffff"/>
            <rect x="45" y="31" width="9" height="8" rx="1.5" fill="#38bdf8"/>
            <!-- Bánh xe cơ giới -->
            <circle cx="16" cy="49" r="4" fill="#f59e0b" stroke="#0a2540" stroke-width="2"/>
            <circle cx="28" cy="49" r="4" fill="#f59e0b" stroke="#0a2540" stroke-width="2"/>
            <circle cx="49" cy="49" r="4" fill="#f59e0b" stroke="#0a2540" stroke-width="2"/>
          </svg>
        </div>
        <div class="leading-tight">
          <span class="block text-[13px] sm:text-[15px] font-black tracking-tight text-brand-primary">TRUNG HIẾU ĐN</span>
          <span class="block text-[9.5px] sm:text-[10.5px] font-semibold text-brand-orange uppercase tracking-wider">trunghieudn.com</span>
        </div>
      </a>

      <!-- MENU DANH MỤC TRÊN MÁY TÍNH: VIẾT LIỀN TRÊN 1 HÀNG, CHỮ NHỎ GỌN, KHÔNG XUỐNG DÒNG -->
      <nav class="hidden lg:flex items-center justify-end flex-wrap gap-x-1 xl:gap-x-1.5">
        <a href="#trang-chu" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-bold text-brand-primary hover:text-brand-orange rounded transition">TRANG CHỦ</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('all')" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">VẬN CHUYỂN MÁY XÚC - MÁY ĐÀO</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('xe-lu-may-ui')" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">VẬN CHUYỂN XE LU - MÁY ỦI</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('xe-cau-dong-coc')" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">XE CẨU - MÁY ĐÓNG CỌC</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('fooc-lun-mooc-rut')" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">FOOC LÙN - MOÓC RÚT</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('sieu-truong-sieu-trong')" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">SIÊU TRƯỜNG SIÊU TRỌNG</a>
        <a href="#form-bao-gia" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">BÁO GIÁ</a>
        <a href="#tin-tuc" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">BÀI VIẾT</a>
        <a href="#lien-he-bando" class="whitespace-nowrap px-2 py-1.5 text-[11.5px] xl:text-[12.5px] font-semibold text-slate-700 hover:text-brand-primary rounded transition">LIÊN HỆ</a>
      </nav>

      <!-- NÚT MỞ MENU TRÊN ĐIỆN THOẠI (KHÔNG ĐỂ NÚT GỌI NGAY ĐỂ TRÁNH TRÀN VIỀN) -->
      <button id="mobile-menu-btn" type="button" onclick="toggleMobileMenu()" aria-label="Mở danh mục" class="lg:hidden inline-flex items-center justify-center p-2 rounded-md text-brand-primary hover:bg-slate-100 border border-slate-200 focus:outline-none">
        <i id="mobile-menu-icon" class="fa-solid fa-bars text-base"></i>
        <span class="ml-1.5 text-xs font-bold">DANH MỤC</span>
      </button>
    </div>

    <!-- MENU XỔ XUỐNG TRÊN ĐIỆN THOẠI -->
    <div id="mobile-menu-drawer" class="hidden lg:hidden bg-white border-t border-slate-200 shadow-lg">
      <div class="flatsome-container py-2.5 grid grid-cols-2 gap-1.5">
        <a href="#trang-chu" onclick="toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-bold bg-slate-50 text-brand-primary rounded border border-slate-200">Trang Chủ</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('may-xuc-may-dao'); toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-semibold bg-slate-50 text-slate-700 rounded border border-slate-200">Chở Máy Xúc - Đào</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('xe-lu-may-ui'); toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-semibold bg-slate-50 text-slate-700 rounded border border-slate-200">Chở Xe Lu - Máy Ủi</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('xe-cau-dong-coc'); toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-semibold bg-slate-50 text-slate-700 rounded border border-slate-200">Chở Xe Cẩu - Đóng Cọc</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('fooc-lun-mooc-rut'); toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-semibold bg-slate-50 text-slate-700 rounded border border-slate-200">Fooc Lùn - Moóc Rút</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('sieu-truong-sieu-trong'); toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-semibold bg-slate-50 text-slate-700 rounded border border-slate-200">Siêu Trường Siêu Trọng</a>
        <a href="#danh-muc-san-pham" onclick="filterCategory('bac-nam'); toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-semibold bg-slate-50 text-slate-700 rounded border border-slate-200">Cơ Giới Bắc - Nam</a>
        <a href="#form-bao-gia" onclick="toggleMobileMenu()" class="whitespace-nowrap px-2.5 py-2 text-[11.5px] font-semibold bg-amber-50 text-brand-orange rounded border border-amber-200">Yêu Cầu Báo Giá</a>
      </div>
    </div>
  </header>

  <!-- ==================== MAIN CONTENT ==================== -->
  <main id="trang-chu" class="flex-grow">

    <!-- ==================== SECTION 1: 2 ẢNH BANNER TỰ TRƯỢT BẰNG NHAU (RIÊNG CHO MÁY TÍNH & ĐIỆN THOẠI) ==================== -->
    <section class="py-3">
      <div class="flatsome-container">
        <div class="relative w-full overflow-hidden rounded-xl shadow-md border border-slate-200 bg-brand-dark">

          <!-- ========== SLIDE 1 ========== -->
          <div class="banner-slide block transition-opacity duration-500" data-slide="0">
            
            <!-- 1A. ẢNH BANNER MÁY TÍNH SỐ 1 (Kích thước chuẩn đồng nhất h-[340px] lg:h-[380px]) -->
            <div class="hidden md:grid grid-cols-12 items-center w-full h-[340px] lg:h-[380px] relative overflow-hidden bg-gradient-to-r from-[#071c34] via-[#0f3e78] to-[#154c8f]">
              <!-- Khối chữ bên trái: Chữ nhỏ gọn nằm hoàn toàn bên trong khung ảnh banner -->
              <div class="col-span-7 pl-10 pr-4 py-6 z-10 text-white">
                <p class="text-brand-accent font-bold text-xs uppercase tracking-widest mb-1.5">
                  CÔNG TY TNHH TRUNG HIẾU ĐN • TRUNGHIEUDN.COM
                </p>
                <h1 class="text-xl lg:text-2xl xl:text-[26px] font-black leading-snug uppercase mb-2.5 text-white">
                  CHUYÊN VẬN CHUYỂN XE CƠ GIỚI & MÁY CÔNG TRÌNH TOÀN QUỐC
                </h1>
                <p class="text-xs lg:text-[13px] text-slate-200 leading-relaxed mb-3 max-w-xl">
                  Đội xe Fooc lùn, Sơ mi rơ moóc rút sàn chuyên chở máy xúc, máy đào, xe lu, máy ủi, xe cẩu bánh xích và thiết bị cơ giới nặng Đà Nẵng đi Bắc - Trung - Nam an toàn, đúng tiến độ.
                </p>
                <div class="grid grid-cols-2 gap-2 text-[11.5px] text-slate-100 mb-4 max-w-lg">
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-circle-check text-brand-accent"></i><span>Đội xe Fooc lùn 30 - 100 tấn</span></div>
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-circle-check text-brand-accent"></i><span>Bảo hiểm thiết bị cơ giới 100%</span></div>
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-location-dot text-brand-accent"></i><span>58 Nguyễn Hữu Hào, TP Đà Nẵng</span></div>
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-phone text-brand-accent"></i><span>Hotline/Zalo: 0961.797.119</span></div>
                </div>
                <div class="flex items-center gap-3">
                  <a href="#form-bao-gia" class="px-4 py-2 rounded-lg bg-brand-accent hover:bg-amber-400 text-brand-dark font-extrabold text-xs uppercase transition shadow">
                    Nhận Báo Giá Vận Chuyển
                  </a>
                  <a href="#danh-muc-san-pham" class="px-4 py-2 rounded-lg bg-white/10 hover:bg-white/20 text-white font-semibold text-xs border border-white/25 transition">
                    Xem Dịch Vụ Cơ Giới
                  </a>
                </div>
              </div>
              <!-- Khối ảnh thực tế bên phải -->
              <div class="col-span-5 h-full relative p-4 flex items-center justify-center">
                <div class="w-full h-[280px] lg:h-[310px] rounded-xl overflow-hidden border-2 border-brand-accent/80 shadow-xl bg-slate-900">
                  <img 
                    src="https://drive.google.com/thumbnail?id=1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD&sz=w1000" 
                    onerror="handleDriveImg(this, '1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD', 'Vận Chuyển Xe Cơ Giới Trung Hiếu ĐN')"
                    alt="Vận chuyển xe cơ giới Trung Hiếu ĐN" 
                    class="w-full h-full object-cover">
                </div>
              </div>
            </div>

            <!-- 1B. ẢNH BANNER ĐIỆN THOẠI SỐ 1 (Thiết kế riêng cho ĐT: h-[250px], chữ nhỏ gọn nằm trọn trong ảnh, không tràn viền) -->
            <div class="block md:hidden w-full h-[250px] relative overflow-hidden bg-gradient-to-b from-[#08203e] to-[#0f3e78]">
              <img 
                src="https://drive.google.com/thumbnail?id=1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD&sz=w800" 
                onerror="handleDriveImg(this, '1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD', 'Vận Chuyển Xe Cơ Giới')"
                alt="Banner điện thoại 1 - Trung Hiếu ĐN" 
                class="absolute inset-0 w-full h-full object-cover opacity-30">
              <div class="relative z-10 w-full h-full px-5 py-3.5 flex flex-col justify-center items-center text-center text-white">
                <span class="text-[10px] font-bold text-brand-accent uppercase tracking-wider mb-1">
                  CÔNG TY TNHH TRUNG HIẾU ĐN (TRUNGHIEUDN.COM)
                </span>
                <h2 class="text-[14px] font-extrabold uppercase leading-snug text-white mb-1.5 px-1">
                  CHUYÊN VẬN CHUYỂN XE CƠ GIỚI & MÁY CÔNG TRÌNH
                </h2>
                <p class="text-[11px] text-slate-200 leading-tight mb-2 px-2">
                  Chuyên chở máy xúc, xe đào, xe lu, máy ủi, xe cẩu bằng Fooc lùn, Moóc rút Bắc - Nam an toàn.
                </p>
                <div class="text-[10.5px] text-amber-200 font-medium mb-2.5 px-2 leading-tight">
                  <div>Đ/c: 58 Nguyễn Hữu Hào, P. Ngũ Hành Sơn, Đà Nẵng</div>
                  <div>Hotline / Zalo: <strong class="text-white">0961.797.119</strong></div>
                </div>
                <a href="#form-bao-gia" class="px-3.5 py-1.5 rounded-md bg-brand-accent text-brand-dark font-bold text-[11px] uppercase shadow">
                  Gửi Yêu Cầu Báo Giá
                </a>
              </div>
            </div>

          </div>

          <!-- ========== SLIDE 2 ========== -->
          <div class="banner-slide hidden transition-opacity duration-500" data-slide="1">
            
            <!-- 2A. ẢNH BANNER MÁY TÍNH SỐ 2 (Kích thước chuẩn đồng nhất h-[340px] lg:h-[380px]) -->
            <div class="hidden md:grid grid-cols-12 items-center w-full h-[340px] lg:h-[380px] relative overflow-hidden bg-gradient-to-r from-[#0a2540] via-[#124582] to-[#0c3262]">
              <!-- Khối chữ bên trái: Chữ nhỏ gọn nằm hoàn toàn bên trong khung ảnh banner -->
              <div class="col-span-7 pl-10 pr-4 py-6 z-10 text-white">
                <p class="text-brand-accent font-bold text-xs uppercase tracking-widest mb-1.5">
                  ĐỘI XE FOOC LÙN - MOÓC RÚT - SƠ MI RƠ MOÓC SÀN CHUYÊN DỤNG
                </p>
                <h2 class="text-xl lg:text-2xl xl:text-[26px] font-black leading-snug uppercase mb-2.5 text-white">
                  VẬN TẢI HÀNG SIÊU TRƯỜNG SIÊU TRỌNG ĐÀ NẴNG - BẮC NAM
                </h2>
                <p class="text-xs lg:text-[13px] text-slate-200 leading-relaxed mb-3 max-w-xl">
                  Giải pháp vận chuyển trọn gói xe cuốc, máy đóng cọc, cẩu bánh xích, trạm trộn bê tông và thiết bị dự án. Khảo sát lộ trình miễn phí, cước phí tối ưu nhất cho chủ đầu tư và nhà thầu.
                </p>
                <div class="grid grid-cols-2 gap-2 text-[11.5px] text-slate-100 mb-4 max-w-lg">
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-truck-moving text-brand-accent"></i><span>Moóc lùn 40ft & Moóc sàn 45ft</span></div>
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-shield-halved text-brand-accent"></i><span>Giấy phép lưu hành quá khổ tải</span></div>
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-map-location-dot text-brand-accent"></i><span>Vận chuyển 63 tỉnh thành</span></div>
                  <div class="flex items-center gap-1.5"><i class="fa-solid fa-headset text-brand-accent"></i><span>Điều độ 24/7: 0961.797.119</span></div>
                </div>
                <div class="flex items-center gap-3">
                  <a href="#form-bao-gia" class="px-4 py-2 rounded-lg bg-brand-accent hover:bg-amber-400 text-brand-dark font-extrabold text-xs uppercase transition shadow">
                    Tư Vấn Lộ Trình & Giá Cước
                  </a>
                  <a href="#lien-he-bando" class="px-4 py-2 rounded-lg bg-white/10 hover:bg-white/20 text-white font-semibold text-xs border border-white/25 transition">
                    Xem Bản Đồ Công Ty
                  </a>
                </div>
              </div>
              <!-- Khối ảnh thực tế bên phải -->
              <div class="col-span-5 h-full relative p-4 flex items-center justify-center">
                <div class="w-full h-[280px] lg:h-[310px] rounded-xl overflow-hidden border-2 border-brand-accent/80 shadow-xl bg-slate-900">
                  <img 
                    src="https://drive.google.com/thumbnail?id=1cPb85DEWun5lAOBwzuptYebi-W5XNLS7&sz=w1000" 
                    onerror="handleDriveImg(this, '1cPb85DEWun5lAOBwzuptYebi-W5XNLS7', 'Đội Xe Fooc Lùn Trung Hiếu ĐN')"
                    alt="Đội xe Fooc lùn Trung Hiếu ĐN" 
                    class="w-full h-full object-cover">
                </div>
              </div>
            </div>

            <!-- 2B. ẢNH BANNER ĐIỆN THOẠI SỐ 2 (Thiết kế riêng cho ĐT: h-[250px], chữ nhỏ gọn nằm trọn trong ảnh, không tràn viền) -->
            <div class="block md:hidden w-full h-[250px] relative overflow-hidden bg-gradient-to-b from-[#0a2540] to-[#15457d]">
              <img 
                src="https://drive.google.com/thumbnail?id=1cPb85DEWun5lAOBwzuptYebi-W5XNLS7&sz=w800" 
                onerror="handleDriveImg(this, '1cPb85DEWun5lAOBwzuptYebi-W5XNLS7', 'Đội Xe Fooc Lùn Moóc Rút')"
                alt="Banner điện thoại 2 - Trung Hiếu ĐN" 
                class="absolute inset-0 w-full h-full object-cover opacity-30">
              <div class="relative z-10 w-full h-full px-5 py-3.5 flex flex-col justify-center items-center text-center text-white">
                <span class="text-[10px] font-bold text-brand-accent uppercase tracking-wider mb-1">
                  ĐỘI XE FOOC LÙN & MOÓC RÚT CHUYÊN DỤNG
                </span>
                <h2 class="text-[14px] font-extrabold uppercase leading-snug text-white mb-1.5 px-1">
                  VẬN CHUYỂN CƠ GIỚI NẶNG BẮC - TRUNG - NAM
                </h2>
                <p class="text-[11px] text-slate-200 leading-tight mb-2 px-2">
                  Nhận chở thiết bị siêu trường siêu trọng, máy công trình giao tận chân dự án đúng tiến độ, giá cước cạnh tranh.
                </p>
                <div class="text-[10.5px] text-amber-200 font-medium mb-2.5 px-2 leading-tight">
                  <div>Website: <strong class="text-white">trunghieudn.com</strong></div>
                  <div>Báo giá 24/7: <strong class="text-white">0961.797.119</strong></div>
                </div>
                <a href="#danh-muc-san-pham" class="px-3.5 py-1.5 rounded-md bg-brand-accent text-brand-dark font-bold text-[11px] uppercase shadow">
                  Xem Phương Tiện & Dịch Vụ
                </a>
              </div>
            </div>

          </div>

          <!-- Nút chuyển trái/phải và chấm chỉ báo Slide -->
          <button type="button" onclick="changeSlide(-1)" aria-label="Banner trước" class="absolute left-2 top-1/2 -translate-y-1/2 w-7 h-7 sm:w-8 sm:h-8 rounded-full bg-black/40 hover:bg-black/65 text-white flex items-center justify-center z-20 transition">
            <i class="fa-solid fa-chevron-left text-xs"></i>
          </button>
          <button type="button" onclick="changeSlide(1)" aria-label="Banner tiếp" class="absolute right-2 top-1/2 -translate-y-1/2 w-7 h-7 sm:w-8 sm:h-8 rounded-full bg-black/40 hover:bg-black/65 text-white flex items-center justify-center z-20 transition">
            <i class="fa-solid fa-chevron-right text-xs"></i>
          </button>
          <div class="absolute bottom-2 left-1/2 -translate-x-1/2 flex items-center gap-2 z-20">
            <button type="button" onclick="goToSlide(0)" class="banner-dot w-6 h-1.5 rounded-full bg-brand-accent transition-all" aria-label="Slide 1"></button>
            <button type="button" onclick="goToSlide(1)" class="banner-dot w-2.5 h-1.5 rounded-full bg-white/60 transition-all" aria-label="Slide 2"></button>
          </div>

        </div>
      </div>
    </section>

    <!-- ==================== SECTION 2: THANH CAM KẾT DỊCH VỤ CHUẨN MẪU VANCHUYENMAYCONGTRINH.COM ==================== -->
    <section class="py-2">
      <div class="flatsome-container">
        <div class="grid grid-cols-2 lg:grid-cols-4 gap-2.5">
          <div class="bg-white p-3 rounded-lg border border-slate-200 shadow-sm flex items-center gap-2.5">
            <div class="w-9 h-9 rounded-lg bg-brand-primary/10 text-brand-primary flex items-center justify-center shrink-0">
              <i class="fa-solid fa-truck-ramp-box text-base"></i>
            </div>
            <div>
              <h3 class="text-xs sm:text-[13px] font-bold text-brand-dark">Đội Xe Fooc Lùn Chuyên Dụng</h3>
              <p class="text-[11px] text-slate-500">Đầy đủ Moóc lùn, Moóc rút, Moóc sàn</p>
            </div>
          </div>
          <div class="bg-white p-3 rounded-lg border border-slate-200 shadow-sm flex items-center gap-2.5">
            <div class="w-9 h-9 rounded-lg bg-brand-primary/10 text-brand-primary flex items-center justify-center shrink-0">
              <i class="fa-solid fa-shield-check text-base"></i>
            </div>
            <div>
              <h3 class="text-xs sm:text-[13px] font-bold text-brand-dark">Bảo Hiểm Hàng Hóa 100%</h3>
              <p class="text-[11px] text-slate-500">An toàn tuyệt đối cho xe cơ giới</p>
            </div>
          </div>
          <div class="bg-white p-3 rounded-lg border border-slate-200 shadow-sm flex items-center gap-2.5">
            <div class="w-9 h-9 rounded-lg bg-brand-primary/10 text-brand-primary flex items-center justify-center shrink-0">
              <i class="fa-solid fa-route text-base"></i>
            </div>
            <div>
              <h3 class="text-xs sm:text-[13px] font-bold text-brand-dark">Vận Chuyển Bắc - Trung - Nam</h3>
              <p class="text-[11px] text-slate-500">Giao nhận tận chân công trình</p>
            </div>
          </div>
          <div class="bg-white p-3 rounded-lg border border-slate-200 shadow-sm flex items-center gap-2.5">
            <div class="w-9 h-9 rounded-lg bg-brand-primary/10 text-brand-primary flex items-center justify-center shrink-0">
              <i class="fa-solid fa-hand-holding-dollar text-base"></i>
            </div>
            <div>
              <h3 class="text-xs sm:text-[13px] font-bold text-brand-dark">Giá Cước Tối Ưu Nhất</h3>
              <p class="text-[11px] text-slate-500">Khảo sát miễn phí, báo giá nhanh</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ==================== SECTION 3: DANH MỤC SẢN PHẨM & DỊCH VỤ (CHỮ NHỎ GỌN, 1 HÀNG TRÊN PC, 2 CỘT TRÊN ĐT, KHÔNG NHÃN DÁN) ==================== -->
    <section id="danh-muc-san-pham" class="py-5">
      <div class="flatsome-container">
        
        <!-- Tiêu đề Flatsome -->
        <div class="flatsome-section-title">
          <h2 class="text-sm sm:text-base md:text-lg">DANH MỤC DỊCH VỤ VẬN CHUYỂN XE CƠ GIỚI</h2>
          <span class="text-[11px] sm:text-xs text-slate-500 font-medium hidden sm:inline">CÔNG TY TNHH TRUNG HIẾU ĐN - 0961.797.119</span>
        </div>

        <!-- Thanh Danh Mục:
             - Trên máy tính: chữ nhỏ gọn (text-[11.5px]), nằm liền trên 1 hàng hoặc xuống hàng 2 nguyên cụm, tuyệt đối KHÔNG xuống dòng bên trong tên danh mục (whitespace-nowrap).
             - Trên điện thoại: chia lưới 2 cột đều đẹp, chữ nhỏ gọn không tràn viền. -->
        <div class="mb-4">
          <div class="grid grid-cols-2 sm:flex sm:flex-wrap items-center justify-start gap-1.5">
            <button type="button" onclick="filterCategory('all')" data-cat-btn="all" class="cat-pill-item active px-2.5 py-1.5 rounded border border-slate-300 bg-white text-slate-700 text-[11px] xl:text-[12px] font-semibold shadow-sm">
              Tất Cả Dịch Vụ (12)
            </button>
            <button type="button" onclick="filterCategory('may-xuc-may-dao')" data-cat-btn="may-xuc-may-dao" class="cat-pill-item px-2.5 py-1.5 rounded border border-slate-300 bg-white text-slate-700 text-[11px] xl:text-[12px] font-semibold shadow-sm">
              Vận Chuyển Máy Xúc - Máy Đào
            </button>
            <button type="button" onclick="filterCategory('xe-lu-may-ui')" data-cat-btn="xe-lu-may-ui" class="cat-pill-item px-2.5 py-1.5 rounded border border-slate-300 bg-white text-slate-700 text-[11px] xl:text-[12px] font-semibold shadow-sm">
              Vận Chuyển Xe Lu - Máy Ủi
            </button>
            <button type="button" onclick="filterCategory('xe-cau-dong-coc')" data-cat-btn="xe-cau-dong-coc" class="cat-pill-item px-2.5 py-1.5 rounded border border-slate-300 bg-white text-slate-700 text-[11px] xl:text-[12px] font-semibold shadow-sm">
              Vận Chuyển Xe Cẩu - Máy Đóng Cọc
            </button>
            <button type="button" onclick="filterCategory('fooc-lun-mooc-rut')" data-cat-btn="fooc-lun-mooc-rut" class="cat-pill-item px-2.5 py-1.5 rounded border border-slate-300 bg-white text-slate-700 text-[11px] xl:text-[12px] font-semibold shadow-sm">
              Sơ Mi Rơ Moóc Lùn - Moóc Rút
            </button>
            <button type="button" onclick="filterCategory('sieu-truong-sieu-trong')" data-cat-btn="sieu-truong-sieu-trong" class="cat-pill-item px-2.5 py-1.5 rounded border border-slate-300 bg-white text-slate-700 text-[11px] xl:text-[12px] font-semibold shadow-sm">
              Vận Chuyển Siêu Trường Siêu Trọng
            </button>
            <button type="button" onclick="filterCategory('bac-nam')" data-cat-btn="bac-nam" class="cat-pill-item col-span-2 sm:col-span-1 px-2.5 py-1.5 rounded border border-slate-300 bg-white text-slate-700 text-[11px] xl:text-[12px] font-semibold shadow-sm">
              Vận Chuyển Xe Cơ Giới Bắc - Nam
            </button>
          </div>
        </div>

        <!-- LƯỚI SẢN PHẨM / DỊCH VỤ:
             - Điện thoại: CHIA THÀNH 2 CỘT (grid-cols-2)
             - Máy tính: 4 cột chuẩn Flatsome (lg:grid-cols-4)
             - KHÔNG để các nhãn dán (badge/sticker) trên ảnh
             - Tên sản phẩm hiển thị ĐẦY ĐỦ 100%, không bị cắt chữ hoặc tràn ra ngoài -->
        <div id="product-grid" class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-2.5 sm:gap-4">
          <!-- Được render tự động từ mảng 12 dịch vụ sử dụng 10 ảnh thực tế Google Drive bên dưới -->
        </div>

      </div>
    </section>

    <!-- ==================== SECTION 4: TIỆN ÍCH TƯ VẤN CHỌN XE & TÍNH KHỐI LƯỢNG (THEO WEB MẪU VANCHUYENMAYCONGTRINH.COM) ==================== -->
    <section class="py-4">
      <div class="flatsome-container">
        <div class="bg-white rounded-xl border border-slate-200 p-4 sm:p-5 shadow-sm">
          <div class="flatsome-section-title">
            <h2 class="text-sm sm:text-base md:text-lg">CÔNG CỤ TƯ VẤN CHỌN XE FOOC LÙN - MOÓC RÚT PHÙ HỢP</h2>
            <span class="text-xs text-brand-primary font-semibold hidden md:inline">Tiện ích tra cứu nhanh chuẩn Logistics</span>
          </div>

          <div class="grid grid-cols-1 lg:grid-cols-12 gap-4 items-center">
            <div class="lg:col-span-7 grid grid-cols-1 sm:grid-cols-3 gap-3">
              <div>
                <label class="block text-xs font-semibold text-slate-700 mb-1">Loại thiết bị cơ giới</label>
                <select id="calc-type" class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none">
                  <option value="Máy xúc / Xe đào bánh xích">Máy xúc / Xe đào bánh xích</option>
                  <option value="Xe lu rung / Máy ủi công trình">Xe lu rung / Máy ủi công trình</option>
                  <option value="Xe cẩu bánh xích / Máy khoan cọc nhồi">Xe cẩu bánh xích / Máy khoan cọc nhồi</option>
                  <option value="Máy biến áp / Kết cấu siêu trường">Máy biến áp / Kết cấu siêu trường</option>
                </select>
              </div>
              <div>
                <label class="block text-xs font-semibold text-slate-700 mb-1">Trọng lượng máy (Tấn)</label>
                <input id="calc-weight" type="number" value="22" min="1" max="200" class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none" placeholder="VD: 22">
              </div>
              <div>
                <label class="block text-xs font-semibold text-slate-700 mb-1">Chiều cao máy (Mét)</label>
                <input id="calc-height" type="number" step="0.1" value="3.1" min="1" max="6" class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none" placeholder="VD: 3.1">
              </div>
            </div>

            <div class="lg:col-span-5 flex flex-col sm:flex-row items-stretch sm:items-center justify-between gap-3 bg-slate-50 p-3 rounded-lg border border-slate-200">
              <div id="calc-result" class="text-xs text-slate-700 leading-relaxed">
                <strong class="text-brand-primary block">Phương tiện khuyến nghị:</strong>
                Xe Fooc lùn 3 trục (Sơ mi rơ moóc lùn 40 feet) - Chuyên chở an toàn máy 20 - 35 tấn, gầm thấp qua cầu vượt dễ dàng.
              </div>
              <button type="button" onclick="runVehicleAdvisor()" class="shrink-0 px-3.5 py-2 rounded-lg bg-brand-primary hover:bg-brand-dark text-white font-bold text-xs transition">
                Tra Cứu Xe
              </button>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- ==================== SECTION 5: FORM YÊU CẦU VÀ BÁO GIÁ TRANG CHỦ ==================== -->
    <section id="form-bao-gia" class="py-5">
      <div class="flatsome-container">
        <div class="bg-white rounded-xl border border-slate-200 shadow-sm overflow-hidden">
          <div class="grid grid-cols-1 lg:grid-cols-12">
            
            <!-- Cột thông tin quy trình & cam kết báo giá -->
            <div class="lg:col-span-5 bg-brand-primary text-white p-5 sm:p-6 flex flex-col justify-between">
              <div>
                <h2 class="text-base sm:text-lg font-extrabold uppercase text-brand-accent mb-2">
                  NHẬN BÁO GIÁ VẬN CHUYỂN XE CƠ GIỚI NHANH
                </h2>
                <p class="text-xs sm:text-[13px] text-slate-200 leading-relaxed mb-4">
                  Quý khách hàng, nhà thầu xây dựng cần vận chuyển máy xúc, xe đào, xe lu, máy ủi, cẩu bánh xích hoặc hàng quá khổ quá tải vui lòng điền thông tin bên cạnh. Phòng điều vận <strong>CÔNG TY TNHH TRUNG HIẾU ĐN</strong> sẽ phản hồi báo giá trong 5 phút!
                </p>

                <div class="space-y-2.5 text-xs">
                  <div class="flex items-start gap-2.5 bg-white/10 p-2.5 rounded-lg">
                    <i class="fa-solid fa-building text-brand-accent mt-0.5"></i>
                    <div>
                      <strong class="block text-white">Đơn vị vận tải:</strong>
                      <span>CÔNG TY TNHH TRUNG HIẾU ĐN (MST: 0402271218)</span>
                    </div>
                  </div>
                  <div class="flex items-start gap-2.5 bg-white/10 p-2.5 rounded-lg">
                    <i class="fa-solid fa-location-dot text-brand-accent mt-0.5"></i>
                    <div>
                      <strong class="block text-white">Địa chỉ trụ sở:</strong>
                      <span>58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng</span>
                    </div>
                  </div>
                  <div class="flex items-start gap-2.5 bg-white/10 p-2.5 rounded-lg">
                    <i class="fa-solid fa-phone-volume text-brand-accent mt-0.5"></i>
                    <div>
                      <strong class="block text-white">Hotline / Zalo điều xe 24/7:</strong>
                      <span class="text-brand-accent font-extrabold text-sm">0961.797.119</span>
                    </div>
                  </div>
                </div>
              </div>

              <div class="mt-4 pt-3 border-t border-white/15 text-[11px] text-slate-300 flex items-center justify-between">
                <span>Website: <strong>trunghieudn.com</strong></span>
                <span>Hỗ trợ xuất hóa đơn VAT đầy đủ</span>
              </div>
            </div>

            <!-- Cột Form Yêu Cầu & Báo Giá -->
            <div class="lg:col-span-7 p-5 sm:p-6">
              <form id="quote-request-form" onsubmit="submitQuoteForm(event)" class="space-y-3">
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                  <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Họ và tên / Tên công ty <span class="text-red-500">*</span></label>
                    <input id="q-name" type="text" required placeholder="Nhập họ tên hoặc tên đơn vị..." class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none">
                  </div>
                  <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Số điện thoại / Zalo <span class="text-red-500">*</span></label>
                    <input id="q-phone" type="tel" required placeholder="Nhập số điện thoại liên hệ..." class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none">
                  </div>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                  <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Danh mục xe cơ giới cần chở <span class="text-red-500">*</span></label>
                    <select id="q-service" class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none">
                      <option value="Vận chuyển Máy xúc, Máy đào, Xe cuốc">Vận chuyển Máy xúc, Máy đào, Xe cuốc</option>
                      <option value="Vận chuyển Xe lu, Máy ủi, Máy san gạt">Vận chuyển Xe lu, Máy ủi, Máy san gạt</option>
                      <option value="Vận chuyển Xe cẩu bánh xích, Máy đóng cọc">Vận chuyển Xe cẩu bánh xích, Máy đóng cọc</option>
                      <option value="Thuê xe Fooc lùn, Sơ mi rơ moóc rút">Thuê xe Fooc lùn, Sơ mi rơ moóc rút</option>
                      <option value="Vận chuyển hàng Siêu trường siêu trọng">Vận chuyển hàng Siêu trường siêu trọng</option>
                      <option value="Vận chuyển Xe cơ giới Bắc - Trung - Nam">Vận chuyển Xe cơ giới Bắc - Trung - Nam</option>
                    </select>
                  </div>
                  <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Trọng lượng / Model máy (nếu có)</label>
                    <input id="q-model" type="text" placeholder="VD: Máy đào Kobelco SK200, Xe lu 12 tấn..." class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none">
                  </div>
                </div>

                <div class="grid grid-cols-1 sm:grid-cols-2 gap-3">
                  <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Địa điểm nhận hàng (Bốc máy) <span class="text-red-500">*</span></label>
                    <input id="q-from" type="text" required placeholder="VD: Đà Nẵng / KCN Hòa Khánh..." class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none">
                  </div>
                  <div>
                    <label class="block text-xs font-bold text-slate-700 mb-1">Địa điểm giao hàng (Hạ máy) <span class="text-red-500">*</span></label>
                    <input id="q-to" type="text" required placeholder="VD: Quảng Ngãi / Hà Nội / TP.HCM..." class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none">
                  </div>
                </div>

                <div>
                  <label class="block text-xs font-bold text-slate-700 mb-1">Ghi chú yêu cầu thêm</label>
                  <textarea id="q-note" rows="2" placeholder="Nhập thời gian dự kiến bốc hàng hoặc yêu cầu đặc biệt..." class="w-full rounded-lg border border-slate-300 px-3 py-2 text-xs focus:border-brand-primary focus:outline-none"></textarea>
                </div>

                <div class="flex flex-wrap items-center justify-between gap-2 pt-1">
                  <button type="submit" class="px-5 py-2.5 rounded-lg bg-brand-orange hover:bg-orange-700 text-white font-extrabold text-xs uppercase tracking-wide shadow transition flex items-center gap-2">
                    <i class="fa-solid fa-paper-plane"></i>
                    <span>Gửi Yêu Cầu Báo Giá Ngay</span>
                  </button>
                  <a href="https://zalo.me/0961797119" target="_blank" rel="noopener noreferrer" class="px-4 py-2.5 rounded-lg bg-slate-100 hover:bg-slate-200 text-brand-primary font-bold text-xs transition flex items-center gap-1.5">
                    <i class="fa-solid fa-comment-dots"></i>
                    <span>Chat Zalo: 0961.797.119</span>
                  </a>
                </div>

                <!-- Thông báo kết quả gửi form (thay thế hoàn toàn alert) -->
                <div id="quote-feedback" class="hidden rounded-lg bg-emerald-50 border border-emerald-300 p-3 text-xs text-emerald-800"></div>
              </form>
            </div>

          </div>
        </div>
      </div>
    </section>

    <!-- ==================== SECTION 6: DANH MỤC CÁC BÀI VIẾT TRANG CHỦ ==================== -->
    <section id="tin-tuc" class="py-5">
      <div class="flatsome-container">
        <div class="flatsome-section-title">
          <h2 class="text-sm sm:text-base md:text-lg">DANH MỤC BÀI VIẾT & KINH NGHIỆM VẬN CHUYỂN</h2>
          <span class="text-xs text-slate-500 hidden sm:inline">Kiến thức vận tải cơ giới & dự án thực tế</span>
        </div>

        <!-- Danh mục lọc bài viết chữ nhỏ gọn, nằm trên 1 hàng -->
        <div class="flex flex-wrap items-center gap-1.5 mb-4">
          <button type="button" onclick="filterPosts('all')" data-post-btn="all" class="post-cat-btn cat-pill-item active px-2.5 py-1 rounded border border-slate-300 bg-white text-slate-700 text-[11px] font-semibold">
            Tất Cả Bài Viết
          </button>
          <button type="button" onclick="filterPosts('phuong-tien')" data-post-btn="phuong-tien" class="post-cat-btn cat-pill-item px-2.5 py-1 rounded border border-slate-300 bg-white text-slate-700 text-[11px] font-semibold">
            Phương Tiện Fooc Lùn - Moóc Rút
          </button>
          <button type="button" onclick="filterPosts('kinh-nghiem')" data-post-btn="kinh-nghiem" class="post-cat-btn cat-pill-item px-2.5 py-1 rounded border border-slate-300 bg-white text-slate-700 text-[11px] font-semibold">
            Kinh Nghiệm Vận Chuyển Cơ Giới
          </button>
          <button type="button" onclick="filterPosts('du-an')" data-post-btn="du-an" class="post-cat-btn cat-pill-item px-2.5 py-1 rounded border border-slate-300 bg-white text-slate-700 text-[11px] font-semibold">
            Dự Án Vận Tải Bắc - Nam
          </button>
        </div>

        <!-- Lưới bài viết: 2 cột trên điện thoại, 4 cột trên máy tính -->
        <div id="blog-grid" class="grid grid-cols-2 lg:grid-cols-4 gap-2.5 sm:gap-4">
          <!-- Render tự động từ dữ liệu bài viết bên dưới -->
        </div>
      </div>
    </section>

    <!-- ==================== SECTION 7: DANH MỤC CÁC ĐỐI TÁC TIÊU BIỂU ==================== -->
    <section id="doi-tac" class="py-5">
      <div class="flatsome-container">
        <div class="flatsome-section-title">
          <h2 class="text-sm sm:text-base md:text-lg">ĐỐI TÁC & KHÁCH HÀNG TIÊU BIỂU</h2>
          <span class="text-xs text-slate-500 hidden sm:inline">Đồng hành cùng các nhà thầu xây dựng & công trình lớn</span>
        </div>

        <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-2.5">
          <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center shadow-sm hover:border-brand-primary transition">
            <span class="text-sm font-black text-brand-primary tracking-wider">HÒA PHÁT</span>
            <span class="text-[10.5px] text-slate-500 mt-0.5">Tập Đoàn Công Nghiệp</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center shadow-sm hover:border-brand-primary transition">
            <span class="text-sm font-black text-brand-primary tracking-wider">SUN GROUP</span>
            <span class="text-[10.5px] text-slate-500 mt-0.5">Dự Án Hạ Tầng Đà Nẵng</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center shadow-sm hover:border-brand-primary transition">
            <span class="text-sm font-black text-brand-primary tracking-wider">ĐÈO CẢ GROUP</span>
            <span class="text-[10.5px] text-slate-500 mt-0.5">Hạ Tầng Giao Thông</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center shadow-sm hover:border-brand-primary transition">
            <span class="text-sm font-black text-brand-primary tracking-wider">KOMATSU</span>
            <span class="text-[10.5px] text-slate-500 mt-0.5">Máy Công Trình Cơ Giới</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center shadow-sm hover:border-brand-primary transition">
            <span class="text-sm font-black text-brand-primary tracking-wider">DOOSAN</span>
            <span class="text-[10.5px] text-slate-500 mt-0.5">Thiết Bị Cơ Giới Nặng</span>
          </div>
          <div class="bg-white rounded-lg border border-slate-200 p-3 flex flex-col items-center justify-center text-center shadow-sm hover:border-brand-primary transition">
            <span class="text-sm font-black text-brand-primary tracking-wider">VINACONEX</span>
            <span class="text-[10.5px] text-slate-500 mt-0.5">Tổng Công Ty Xây Dựng</span>
          </div>
        </div>
      </div>
    </section>

    <!-- ==================== SECTION 8: ĐƯA ẢNH GOOGLE MAP & FANPAGE RA NGOÀI TRANG CHỦ ==================== -->
    <section id="lien-he-bando" class="py-5">
      <div class="flatsome-container">
        <div class="flatsome-section-title">
          <h2 class="text-sm sm:text-base md:text-lg">BẢN ĐỒ GOOGLE MAPS & FANPAGE TRUNG HIẾU ĐN</h2>
          <span class="text-xs text-slate-500 hidden sm:inline">58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng</span>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-4">
          
          <!-- CỘT TRÁI (7 CỘT): BẢN ĐỒ GOOGLE MAPS TRỰC TIẾP TRÊN TRANG CHỦ -->
          <div class="lg:col-span-7 bg-white rounded-xl border border-slate-200 p-3 sm:p-4 shadow-sm flex flex-col justify-between">
            <div>
              <div class="flex flex-wrap items-center justify-between gap-2 mb-2.5">
                <div>
                  <h3 class="text-xs sm:text-sm font-extrabold text-brand-primary uppercase">
                    <i class="fa-solid fa-map-location-dot text-brand-orange mr-1"></i>
                    VỊ TRÍ TRỤ SỞ TRÊN GOOGLE MAPS
                  </h3>
                  <p class="text-[11.5px] text-slate-600">
                    Địa chỉ: <strong>58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng</strong>
                  </p>
                </div>
                <a href="https://www.google.com/maps/search/?api=1&query=58+Nguyen+Huu+Hao+Ngu+Hanh+Son+Da+Nang" target="_blank" rel="noopener noreferrer" class="px-3 py-1.5 rounded-lg bg-brand-primary hover:bg-brand-dark text-white text-[11px] font-bold transition flex items-center gap-1.5">
                  <i class="fa-solid fa-diamond-turn-right"></i>
                  <span>Mở Chỉ Đường Google Maps</span>
                </a>
              </div>

              <!-- Khung Bản Đồ Google Maps Nhúng + Sơ đồ vị trí trực quan ngoài trang chủ -->
              <div class="w-full h-[260px] sm:h-[300px] rounded-lg overflow-hidden border border-slate-300 relative bg-slate-100">
                <iframe 
                  title="Bản đồ Công Ty TNHH Trung Hiếu ĐN - 58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng"
                  src="https://maps.google.com/maps?q=58%20Nguy%E1%BB%85n%20H%E1%BB%AFu%20H%C3%A0o,%20Ng%C5%A9%20H%C3%A0nh%20S%C6%A1n,%20%C4%90%C3%A0%20N%E1%BA%B5ng&t=&z=15&ie=UTF8&iwloc=&output=embed"
                  class="w-full h-full border-0"
                  loading="lazy"
                  referrerpolicy="no-referrer-when-downgrade">
                </iframe>
              </div>
            </div>

            <div class="mt-3 pt-2.5 border-t border-slate-100 flex flex-wrap items-center justify-between gap-2 text-[11.5px] text-slate-600">
              <span><i class="fa-solid fa-circle-check text-emerald-600 mr-1"></i>Bãi xe & văn phòng điều vận tại Ngũ Hành Sơn, TP Đà Nẵng</span>
              <span class="font-bold text-brand-primary">Hotline: 0961.797.119</span>
            </div>
          </div>

          <!-- CỘT PHẢI (5 CỘT): FANPAGE FACEBOOK ĐƯA RA NGOÀI TRANG CHỦ -->
          <div class="lg:col-span-5 bg-white rounded-xl border border-slate-200 p-3 sm:p-4 shadow-sm flex flex-col justify-between">
            <div>
              <h3 class="text-xs sm:text-sm font-extrabold text-brand-primary uppercase mb-2.5">
                <i class="fa-brands fa-facebook text-[#1877F2] mr-1"></i>
                FANPAGE FACEBOOK CHÍNH THỨC
              </h3>

              <!-- Khung Fanpage Facebook trực quan ngoài trang chủ -->
              <div class="rounded-lg border border-slate-200 overflow-hidden bg-slate-50">
                <!-- Ảnh bìa Fanpage lấy từ ảnh thực tế xe cơ giới Trung Hiếu ĐN -->
                <div class="relative h-36 w-full bg-brand-dark overflow-hidden">
                  <img 
                    src="https://drive.google.com/thumbnail?id=16YQK-FMH3RgiVSClNUMFytvywuwvXIHh&sz=w800" 
                    onerror="handleDriveImg(this, '16YQK-FMH3RgiVSClNUMFytvywuwvXIHh', 'Fanpage Trung Hiếu ĐN')"
                    alt="Fanpage Công Ty TNHH Trung Hiếu ĐN" 
                    class="w-full h-full object-cover opacity-75">
                  <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/30 to-transparent"></div>
                  
                  <div class="absolute bottom-3 left-3 right-3 flex items-end justify-between gap-2">
                    <div class="flex items-center gap-2.5">
                      <div class="w-12 h-12 rounded-lg bg-brand-primary border-2 border-white flex items-center justify-center shadow shrink-0">
                        <span class="text-white font-black text-xs">THĐN</span>
                      </div>
                      <div class="text-white">
                        <h4 class="text-xs sm:text-[13px] font-bold leading-tight">Công Ty TNHH Trung Hiếu ĐN</h4>
                        <p class="text-[10.5px] text-slate-200">Chuyên vận chuyển xe cơ giới • 4.8K người theo dõi</p>
                      </div>
                    </div>
                  </div>
                </div>

                <!-- Các nút tương tác Fanpage -->
                <div class="p-3 bg-white border-b border-slate-200 flex items-center justify-between gap-2">
                  <a href="https://www.facebook.com" target="_blank" rel="noopener noreferrer" class="flex-1 py-1.5 px-3 rounded bg-[#1877F2] hover:bg-blue-700 text-white text-xs font-bold text-center transition">
                    <i class="fa-brands fa-facebook-f mr-1"></i> Theo Dõi Fanpage
                  </a>
                  <a href="https://zalo.me/0961797119" target="_blank" rel="noopener noreferrer" class="flex-1 py-1.5 px-3 rounded bg-slate-100 hover:bg-slate-200 text-slate-800 text-xs font-bold text-center transition">
                    <i class="fa-brands fa-facebook-messenger text-[#1877F2] mr-1"></i> Nhắn Tin Ngay
                  </a>
                </div>

                <!-- Bài đăng mới nhất trên Fanpage -->
                <div class="p-3 space-y-2 text-xs text-slate-700">
                  <p class="leading-relaxed text-[11.5px]">
                    <strong>CÔNG TY TNHH TRUNG HIẾU ĐN</strong> chuyên nhận hợp đồng vận chuyển xe cơ giới, xe đào, xe lu, máy ủi, xe cẩu bánh xích bằng Fooc lùn chuyên dụng từ Đà Nẵng đi toàn quốc.
                  </p>
                  <div class="grid grid-cols-3 gap-1.5 pt-1">
                    <img src="https://drive.google.com/thumbnail?id=15lYy2e1L8_iQ-WwQTIbgHs0zob9_CzXq&sz=w400" onerror="handleDriveImg(this, '15lYy2e1L8_iQ-WwQTIbgHs0zob9_CzXq', 'Ảnh 1')" alt="Hoạt động 1" class="w-full h-16 object-cover rounded border border-slate-200">
                    <img src="https://drive.google.com/thumbnail?id=1sJGbX7PTuN2BSAaTzNgr6T3aUmJ4Pwpx&sz=w400" onerror="handleDriveImg(this, '1sJGbX7PTuN2BSAaTzNgr6T3aUmJ4Pwpx', 'Ảnh 2')" alt="Hoạt động 2" class="w-full h-16 object-cover rounded border border-slate-200">
                    <img src="https://drive.google.com/thumbnail?id=17yMvyEgj250at_NS2Qd_8OgFaXLAOoYw&sz=w400" onerror="handleDriveImg(this, '17yMvyEgj250at_NS2Qd_8OgFaXLAOoYw', 'Ảnh 3')" alt="Hoạt động 3" class="w-full h-16 object-cover rounded border border-slate-200">
                  </div>
                </div>
              </div>
            </div>

            <div class="mt-3 pt-2.5 border-t border-slate-100 flex items-center justify-between text-[11.5px] text-slate-600">
              <span>Website: <strong>trunghieudn.com</strong></span>
              <span>Zalo/ĐT: <strong class="text-brand-orange">0961.797.119</strong></span>
            </div>
          </div>

        </div>
      </div>
    </section>

  </main>

  <!-- ==================== FOOTER CHUẨN FLATSOME ==================== -->
  <footer class="bg-brand-dark text-slate-200 pt-8 pb-6 border-t-4 border-brand-accent mt-4">
    <div class="flatsome-container">
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-12 gap-6 pb-6 border-b border-white/10">
        
        <!-- Cột 1: Thông tin công ty -->
        <div class="lg:col-span-5 space-y-2.5">
          <div class="flex items-center gap-2.5">
            <div class="w-9 h-9 rounded-lg bg-brand-primary flex items-center justify-center border border-brand-accent shrink-0">
              <i class="fa-solid fa-truck-front text-brand-accent text-sm"></i>
            </div>
            <div>
              <h3 class="text-sm font-black text-white uppercase">CÔNG TY TNHH TRUNG HIẾU ĐN</h3>
              <p class="text-[11px] text-brand-accent font-semibold">CHUYÊN VẬN CHUYỂN XE CƠ GIỚI - MÁY CÔNG TRÌNH</p>
            </div>
          </div>
          <p class="text-xs text-slate-300 leading-relaxed">
            Đơn vị uy tín hàng đầu tại Đà Nẵng và miền Trung chuyên cung cấp dịch vụ vận chuyển xe cơ giới, máy xúc, máy đào, xe lu, máy ủi, xe cẩu, thiết bị siêu trường siêu trọng bằng đội xe Fooc lùn, Moóc rút hiện đại.
          </p>
          <ul class="text-xs space-y-1.5 text-slate-200 pt-1">
            <li><i class="fa-solid fa-location-dot text-brand-accent w-5"></i><strong>Địa chỉ:</strong> 58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng</li>
            <li><i class="fa-solid fa-phone-volume text-brand-accent w-5"></i><strong>Điện thoại / Zalo:</strong> <a href="tel:0961797119" class="text-brand-accent font-bold">0961.797.119</a></li>
            <li><i class="fa-solid fa-globe text-brand-accent w-5"></i><strong>Website:</strong> <a href="https://trunghieudn.com" class="hover:underline">trunghieudn.com</a></li>
            <li><i class="fa-solid fa-id-card text-brand-accent w-5"></i><strong>Mã số thuế:</strong> 0402271218</li>
          </ul>
        </div>

        <!-- Cột 2: Danh mục dịch vụ -->
        <div class="lg:col-span-4 space-y-2">
          <h4 class="text-xs font-extrabold uppercase text-brand-accent tracking-wider pb-1 border-b border-white/10">
            DANH MỤC DỊCH VỤ CHÍNH
          </h4>
          <ul class="text-xs space-y-1.5 text-slate-300">
            <li><a href="#danh-muc-san-pham" onclick="filterCategory('may-xuc-may-dao')" class="hover:text-white transition">→ Vận chuyển máy xúc, máy đào, xe cuốc</a></li>
            <li><a href="#danh-muc-san-pham" onclick="filterCategory('xe-lu-may-ui')" class="hover:text-white transition">→ Vận chuyển xe lu rung, máy ủi công trình</a></li>
            <li><a href="#danh-muc-san-pham" onclick="filterCategory('xe-cau-dong-coc')" class="hover:text-white transition">→ Vận chuyển xe cẩu bánh xích, máy đóng cọc</a></li>
            <li><a href="#danh-muc-san-pham" onclick="filterCategory('fooc-lun-mooc-rut')" class="hover:text-white transition">→ Dịch vụ xe Fooc lùn 40ft, Moóc sàn 45ft, Moóc rút</a></li>
            <li><a href="#danh-muc-san-pham" onclick="filterCategory('sieu-truong-sieu-trong')" class="hover:text-white transition">→ Vận chuyển thiết bị siêu trường siêu trọng</a></li>
            <li><a href="#danh-muc-san-pham" onclick="filterCategory('bac-nam')" class="hover:text-white transition">→ Vận chuyển xe cơ giới Bắc - Trung - Nam</a></li>
          </ul>
        </div>

        <!-- Cột 3: Hỗ trợ khách hàng -->
        <div class="lg:col-span-3 space-y-2">
          <h4 class="text-xs font-extrabold uppercase text-brand-accent tracking-wider pb-1 border-b border-white/10">
            HỖ TRỢ & CAM KẾT
          </h4>
          <ul class="text-xs space-y-1.5 text-slate-300">
            <li>✓ Khảo sát lộ trình miễn phí 100%</li>
            <li>✓ Bảo hiểm hàng hóa thiết bị cơ giới</li>
            <li>✓ Hợp đồng vận chuyển & Hóa đơn VAT</li>
            <li>✓ Phục vụ 24/7 kể cả ngày lễ, Chủ nhật</li>
          </ul>
          <div class="pt-2">
            <a href="#form-bao-gia" class="inline-block w-full text-center py-2 px-3 rounded-lg bg-brand-accent text-brand-dark font-extrabold text-xs uppercase hover:bg-amber-400 transition">
              Gửi Yêu Cầu Báo Giá
            </a>
          </div>
        </div>

      </div>

      <div class="pt-4 flex flex-col sm:flex-row items-center justify-between text-[11px] text-slate-400 gap-2 text-center">
        <p>© Bản quyền thuộc về <strong>CÔNG TY TNHH TRUNG HIẾU ĐN (trunghieudn.com)</strong>.</p>
        <p>Đ/c: 58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng • ĐT: 0961.797.119</p>
      </div>
    </div>
  </footer>

  <!-- ==================== CÁC NÚT LIÊN HỆ NỔI BẬT (ZALO, FACEBOOK, HOTLINE) TƯƠNG THÍCH MÁY TÍNH & ĐIỆN THOẠI ==================== -->
  <div class="fixed bottom-4 right-3 z-50 flex flex-col items-end gap-2.5">
    
    <!-- Nút Facebook Fanpage -->
    <a href="#lien-he-bando" title="Fanpage Facebook Trung Hiếu ĐN" class="flex items-center gap-2 bg-[#1877F2] hover:bg-blue-700 text-white px-3 py-2 rounded-full shadow-lg border border-white/30 transition transform hover:scale-105">
      <i class="fa-brands fa-facebook-f text-sm w-4 text-center"></i>
      <span class="text-[11px] font-bold hidden sm:inline">Facebook</span>
    </a>

    <!-- Nút Chat Zalo nổi bật -->
    <a href="https://zalo.me/0961797119" target="_blank" rel="noopener noreferrer" title="Chat Zalo: 0961.797.119" class="flex items-center gap-2 bg-[#0068ff] hover:bg-blue-600 text-white px-3 py-2 rounded-full shadow-lg border border-white/30 transition transform hover:scale-105">
      <span class="font-black text-[11px] bg-white text-[#0068ff] px-1.5 py-0.5 rounded-full leading-none">Zalo</span>
      <span class="text-[11px] font-bold hidden sm:inline">0961.797.119</span>
    </a>

    <!-- Nút Gọi Hotline nổi bật -->
    <a href="tel:0961797119" title="Gọi ngay: 0961.797.119" class="flex items-center gap-2 bg-red-600 hover:bg-red-700 text-white px-3.5 py-2.5 rounded-full shadow-xl border-2 border-amber-300 transition transform hover:scale-105">
      <i class="fa-solid fa-phone-volume text-sm animate-ring"></i>
      <span class="text-xs font-extrabold tracking-wide">0961.797.119</span>
    </a>

  </div>

  <!-- ==================== MODAL XEM CHI TIẾT SẢN PHẨM / BÀI VIẾT ==================== -->
  <div id="detail-modal" class="fixed inset-0 z-50 hidden bg-black/65 flex items-center justify-center p-3">
    <div class="bg-white rounded-xl max-w-xl w-full overflow-hidden shadow-2xl border border-slate-200">
      <div class="bg-brand-primary text-white px-4 py-3 flex items-center justify-between">
        <h3 id="modal-title" class="text-xs sm:text-sm font-bold uppercase pr-2">Chi Tiết Dịch Vụ Vận Chuyển</h3>
        <button type="button" onclick="closeModal()" class="text-white hover:text-brand-accent text-lg leading-none">&times;</button>
      </div>
      <div class="p-4 space-y-3 max-h-[80vh] overflow-y-auto">
        <img id="modal-img" src="" alt="Chi tiết dịch vụ" class="w-full h-52 sm:h-64 object-cover rounded-lg border border-slate-200">
        <p id="modal-desc" class="text-xs sm:text-[13px] text-slate-700 leading-relaxed"></p>
        <div class="bg-slate-50 p-3 rounded-lg border border-slate-200 text-xs space-y-1">
          <div><strong>Đơn vị thực hiện:</strong> CÔNG TY TNHH TRUNG HIẾU ĐN (trunghieudn.com)</div>
          <div><strong>Địa chỉ:</strong> 58 Nguyễn Hữu Hào, Phường Ngũ Hành Sơn, TP Đà Nẵng</div>
          <div><strong>Hotline / Zalo báo giá:</strong> <span class="text-brand-orange font-extrabold">0961.797.119</span></div>
        </div>
        <div class="flex items-center justify-end gap-2 pt-2">
          <button type="button" onclick="closeModal(); document.getElementById('form-bao-gia').scrollIntoView({behavior:'smooth'});" class="px-4 py-2 rounded-lg bg-brand-orange text-white font-bold text-xs">
            Nhận Báo Giá Dịch Vụ Này
          </button>
          <button type="button" onclick="closeModal()" class="px-4 py-2 rounded-lg bg-slate-200 text-slate-700 font-semibold text-xs">
            Đóng
          </button>
        </div>
      </div>
    </div>
  </div>

  <!-- ==================== JAVASCRIPT XỬ LÝ DỮ LIỆU, 10 ẢNH GOOGLE DRIVE & TƯƠNG TÁC ==================== -->
  <script>
    // Cơ chế tải 10 ảnh thực tế từ Google Drive an toàn với chuỗi dự phòng tự động
    function handleDriveImg(imgEl, fileId, labelText) {
      const step = parseInt(imgEl.getAttribute('data-fallback-step') || '0', 10);
      if (step === 0) {
        imgEl.setAttribute('data-fallback-step', '1');
        imgEl.src = 'https://lh3.googleusercontent.com/d/' + fileId + '=w1000';
      } else if (step === 1) {
        imgEl.setAttribute('data-fallback-step', '2');
        imgEl.src = 'https://drive.google.com/uc?export=view&id=' + fileId;
      } else {
        imgEl.onerror = null;
        const safeTitle = encodeURIComponent(labelText || 'TRUNG HIEU DN');
        imgEl.src = 'https://placehold.co/800x550/0f3e78/f59e0b?text=' + safeTitle;
      }
    }

    // Danh sách 12 sản phẩm/dịch vụ chuẩn theo web mẫu vanchuyenmaycongtrinh.com
    // Sử dụng đầy đủ 10 file ảnh thực tế từ Google Drive của khách hàng
    const PRODUCTS_DATA = [
      {
        id: 1,
        cat: 'may-xuc-may-dao',
        driveId: '1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD',
        title: 'Vận Chuyển Máy Xúc Đào Bánh Xích Bằng Xe Fooc Lùn Chuyên Dụng',
        spec: 'Chở xe cuốc Kobelco, Komatsu, Hitachi, Doosan từ 12 - 50 tấn',
        desc: 'Dịch vụ vận chuyển máy xúc đào bánh xích các dòng PC200, PC300, PC450, SK200, SK330 bằng xe Fooc lùn gầm thấp chuyên dụng, có cầu dẫn thủy lực lên xuống an toàn tuyệt đối.'
      },
      {
        id: 2,
        cat: 'bac-nam',
        driveId: '1cPb85DEWun5lAOBwzuptYebi-W5XNLS7',
        title: 'Vận Chuyển Xe Cơ Giới Nặng Đà Nẵng Đi Bắc - Trung - Nam',
        spec: 'Tuyến cố định Đà Nẵng - Hà Nội - TP.HCM & 63 tỉnh thành',
        desc: 'Chuyên nhận hợp đồng vận chuyển xe cơ giới nặng, máy công trình nguyên chiếc hoặc kết hợp ghép chuyến Bắc - Trung - Nam giúp tiết kiệm tối đa chi phí cho doanh nghiệp.'
      },
      {
        id: 3,
        cat: 'may-xuc-may-dao',
        driveId: '15lYy2e1L8_iQ-WwQTIbgHs0zob9_CzXq',
        title: 'Vận Chuyển Máy Đào Bánh Lốp & Xe Cuốc Công Trình Giao Thông',
        spec: 'Giao nhận tận chân công trình, hỗ trợ bốc dỡ 24/7',
        desc: 'Đội xe Fooc lùn, xe cứu hộ sàn trượt của Công Ty TNHH Trung Hiếu ĐN chuyên vận chuyển máy đào bánh lốp, máy xúc lật phục vụ thi công hạ tầng đô thị và cầu đường.'
      },
      {
        id: 4,
        cat: 'xe-lu-may-ui',
        driveId: '1sJGbX7PTuN2BSAaTzNgr6T3aUmJ4Pwpx',
        title: 'Vận Chuyển Xe Lu Rung, Xe Lu Tĩnh, Xe Lu Bánh Lốp Công Trình',
        spec: 'Chuyên chở xe lu Hamm, Sakai, Bomag, Dynapac 10 - 25 tấn',
        desc: 'Vận chuyển các dòng xe lu rung 1 cầu, 2 cầu, lu tĩnh, lu bánh thép đi các dự án cao tốc, khu công nghiệp tại Đà Nẵng, miền Trung và toàn quốc.'
      },
      {
        id: 5,
        cat: 'xe-lu-may-ui',
        driveId: '17yMvyEgj250at_NS2Qd_8OgFaXLAOoYw',
        title: 'Vận Chuyển Máy Ủi Bánh Xích Komatsu, Caterpillar, Máy San Gạt',
        spec: 'Sàn Fooc lùn chịu tải cao, xích chằng buộc lashing tiêu chuẩn',
        desc: 'Chuyên chở máy ủi D3, D4, D5, D6, D85 và máy san gạt công trình có lưỡi ủi rộng quá khổ bằng sơ mi rơ moóc lùn chuyên dụng.'
      },
      {
        id: 6,
        cat: 'xe-cau-dong-coc',
        driveId: '1G9EdD8GqOF5uQ-LHGUmFEj7iqiwXLBzf',
        title: 'Vận Chuyển Xe Cẩu Bánh Xích, Máy Khoan Cọc Nhồi & Búa Đóng Cọc',
        spec: 'Chở thân máy cẩu, đốt cần cẩu, búa rung, robot ép cọc',
        desc: 'Giải pháp vận tải đồng bộ cho tổ hợp máy khoan cọc nhồi, xe cẩu bánh xích, cẩu tháp và thiết bị thi công nền móng công trình lớn.'
      },
      {
        id: 7,
        cat: 'fooc-lun-mooc-rut',
        driveId: '16YQK-FMH3RgiVSClNUMFytvywuwvXIHh',
        title: 'Dịch Vụ Vận Tải Bằng Sơ Mi Rơ Moóc Lùn 40 Feet Chuyên Dụng',
        spec: 'Chiều cao sàn thấp, chuyên chở máy cơ giới cao quá khổ',
        desc: 'Sơ mi rơ moóc lùn 40 feet (Lowboy trailer) giúp hạ thấp trọng tâm máy công trình, di chuyển an toàn qua các hầm chui, cầu vượt và đường đèo dốc.'
      },
      {
        id: 8,
        cat: 'fooc-lun-mooc-rut',
        driveId: '1q8Zio2ZqQqZywYaPwUP3TdLlLQ_jdH84',
        title: 'Dịch Vụ Vận Chuyển Bằng Sơ Mi Rơ Moóc Sàn 45 Feet 3 Trục 12 Gù',
        spec: 'Chuyên chở thiết bị cơ khí, máy công trình & container flat rack',
        desc: 'Sơ mi rơ moóc sàn phẳng 45 feet 3 trục chịu tải lớn, phù hợp chở đồng thời nhiều thiết bị cơ giới, cấu kiện thép và máy móc công nghiệp.'
      },
      {
        id: 9,
        cat: 'sieu-truong-sieu-trong',
        driveId: '1QpsxxZnpFeH-n8e_TlTNm0kZSwumHfXM',
        title: 'Vận Chuyển Hàng Hóa Siêu Trường Siêu Trọng & Thiết Bị Dự Án',
        spec: 'Đầy đủ giấy phép lưu hành đặc biệt, xe hộ tống dẫn đường',
        desc: 'Nhận vận chuyển trọn gói các kiện hàng siêu trường siêu trọng, bồn công nghiệp, dầm cầu, máy nghiền đá, trạm trộn bê tông trên phạm vi toàn quốc.'
      },
      {
        id: 10,
        cat: 'sieu-truong-sieu-trong',
        driveId: '1A4h16Hil7sndoF-GK5DQRxVQ2xBo18Q8',
        title: 'Vận Chuyển Máy Trải Thảm Nhựa, Máy Cào Bóc & Thiết Bị Cầu Đường',
        spec: 'Chuyên chở máy rải thảm Vogele, Sumitomo, máy cào bóc Wirtgen',
        desc: 'Đội ngũ tài xế giàu kinh nghiệm vận hành lên xuống moóc an toàn cho các loại máy trải thảm bê tông nhựa nóng và thiết bị thi công mặt đường.'
      },
      {
        id: 11,
        cat: 'fooc-lun-mooc-rut',
        driveId: '1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD',
        title: 'Phương Tiện Vận Tải Moóc Rút Chuyên Dùng & Rơ Moóc Thủy Lực',
        spec: 'Kéo dài sàn linh hoạt cho hàng dài từ 14m - 25m',
        desc: 'Hệ thống moóc rút sàn và rơ moóc thủy lực đa trục chuyên phục vụ vận chuyển kết cấu thép, cánh điện gió, dầm cầu và thiết bị cơ giới đặc chủng.'
      },
      {
        id: 12,
        cat: 'bac-nam',
        driveId: '1G9EdD8GqOF5uQ-LHGUmFEj7iqiwXLBzf',
        title: 'Vận Chuyển Và Lắp Đặt Máy Biến Áp, Thiết Bị Cơ Khí Công Nghiệp',
        spec: 'Vận chuyển đa phương thức Bắc - Trung - Nam an toàn 100%',
        desc: 'Chuyên vận chuyển, hạ bãi và đưa vào vị trí lắp đặt các tổ hợp máy biến áp, máy phát điện công nghiệp, lò hơi và dây chuyền nhà máy.'
      }
    ];

    // Danh sách bài viết trang chủ (Lấy cảm hứng từ vanchuyenmaycongtrinh.com)
    const BLOG_POSTS = [
      {
        id: 101,
        cat: 'phuong-tien',
        driveId: '16YQK-FMH3RgiVSClNUMFytvywuwvXIHh',
        title: 'Tìm Hiểu Sơ Mi Rơ Moóc Lùn 40 Feet Và Moóc Sàn 45 Feet Chuyên Chở Cơ Giới',
        excerpt: 'Thông số kỹ thuật, tải trọng cho phép và ưu điểm của xe Fooc lùn 40 feet khi vận chuyển máy xúc, máy đào, xe lu qua các cung đường có giới hạn chiều cao.',
        content: 'Sơ mi rơ moóc lùn 40 feet là phương tiện chủ lực tại CÔNG TY TNHH TRUNG HIẾU ĐN dùng để chuyên chở các loại máy công trình có chiều cao và trọng lượng lớn. Nhờ thiết kế dầm võng hạ thấp mặt sàn, xe dễ dàng đi qua cầu vượt, dây điện và đảm bảo độ ổn định cao.'
      },
      {
        id: 102,
        cat: 'kinh-nghiem',
        driveId: '1XF5vR0mLhc1hJunOCwRuOGuRfRngdVoD',
        title: 'Quy Trình Chằng Buộc Lashing Và Vận Chuyển Máy Xúc, Xe Đào An Toàn',
        excerpt: 'Những nguyên tắc kỹ thuật bắt buộc khi đưa máy xúc bánh xích lên sàn Fooc lùn, khóa quay toa và chằng xích chịu lực chống xê dịch trên đường dài.',
        content: 'Để đảm bảo an toàn 100% trong suốt hành trình vận chuyển xe cơ giới Bắc - Nam, đội ngũ kỹ thuật của Trung Hiếu ĐN luôn tuân thủ quy trình 5 bước: khảo sát mặt bằng lên moóc, hạ cần tối đa, chèn lót bánh xích, chằng xích tăng đơ 4 góc và kiểm tra định kỳ trên đường.'
      },
      {
        id: 103,
        cat: 'du-an',
        driveId: '1cPb85DEWun5lAOBwzuptYebi-W5XNLS7',
        title: 'Kinh Nghiệm Vận Chuyển Xe Cơ Giới Bắc - Nam Tối Ưu Chi Phí Cho Nhà Thầu',
        excerpt: 'Cách lựa chọn phương tiện Fooc lùn hoặc ghép chuyến xe cơ giới từ Đà Nẵng đi Hà Nội, Sài Gòn giúp tiết kiệm 15 - 30% chi phí vận tải.',
        content: 'CÔNG TY TNHH TRUNG HIẾU ĐN (58 Nguyễn Hữu Hào, P. Ngũ Hành Sơn, TP Đà Nẵng) có lịch xe Fooc lùn chạy tuyến Bắc - Trung - Nam liên tục mỗi ngày, giúp quý nhà thầu chủ động tiến độ điều chuyển máy móc giữa các dự án với mức cước phí cạnh tranh nhất.'
      },
      {
        id: 104,
        cat: 'kinh-nghiem',
        driveId: '1QpsxxZnpFeH-n8e_TlTNm0kZSwumHfXM',
        title: 'Quy Định Về Vận Chuyển Hàng Siêu Trường Siêu Trọng & Quá Khổ Quá Tải',
        excerpt: 'Tổng hợp quy định kích thước, tải trọng và thủ tục cấp giấy phép lưu hành đặc biệt đối với xe chở máy công trình vượt khổ giới hạn đường bộ.',
        content: 'Khi vận chuyển các thiết bị cơ giới nặng trên 30 tấn hoặc chiều rộng vượt quá 2,5m, đơn vị vận tải phải trang bị xe Fooc lùn đa trục có giấy phép lưu hành đặc biệt. Liên hệ Hotline 0961.797.119 để được Trung Hiếu ĐN tư vấn phương án trọn gói.'
      }
    ];

    // Render lưới sản phẩm (Tuyệt đối không gắn nhãn dán trên ảnh, chia 2 cột trên điện thoại, tên đầy đủ không cắt chữ)
    function renderProducts(categoryFilter) {
      const grid = document.getElementById('product-grid');
      if (!grid) return;

      const filtered = categoryFilter === 'all'
        ? PRODUCTS_DATA
        : PRODUCTS_DATA.filter(item => item.cat === categoryFilter);

      grid.innerHTML = filtered.map(item => `
        <div class="bg-white rounded-lg border border-slate-200 shadow-sm hover:shadow-md transition flex flex-col justify-between overflow-hidden">
          <div>
            <!-- Khung ảnh thực tế từ Google Drive (Không để bất kỳ nhãn dán/sticker nào) -->
            <div class="w-full aspect-[4/3] bg-slate-100 overflow-hidden cursor-pointer" onclick="openProductModal(${item.id})">
              <img 
                src="https://drive.google.com/thumbnail?id=${item.driveId}&sz=w800" 
                onerror="handleDriveImg(this, '${item.driveId}', '${item.title.replace(/'/g, '')}')"
                alt="${item.title}" 
                class="w-full h-full object-cover hover:scale-105 transition duration-300">
            </div>

            <!-- Nội dung sản phẩm: Tên hiển thị đầy đủ 100%, không bị tràn viền hay thiếu chữ -->
            <div class="p-2.5 sm:p-3">
              <h3 onclick="openProductModal(${item.id})" class="product-title-full text-[12.5px] sm:text-[13.5px] font-bold text-brand-dark hover:text-brand-primary cursor-pointer mb-1">
                ${item.title}
              </h3>
              <p class="text-[11px] sm:text-xs text-slate-500 leading-snug">
                ${item.spec}
              </p>
            </div>
          </div>

          <!-- Chân thẻ sản phẩm đơn giản chuẩn Flatsome -->
          <div class="px-2.5 pb-2.5 sm:px-3 sm:pb-3 pt-1 border-t border-slate-100 flex items-center justify-between gap-1">
            <span class="text-[11px] sm:text-xs font-extrabold text-brand-orange">LH: 0961.797.119</span>
            <button type="button" onclick="openProductModal(${item.id})" class="px-2 py-1 rounded bg-brand-primary hover:bg-brand-dark text-white text-[10.5px] sm:text-[11px] font-semibold transition">
              Chi tiết
            </button>
          </div>
        </div>
      `).join('');
    }

    // Lọc danh mục sản phẩm
    function filterCategory(catKey) {
      document.querySelectorAll('[data-cat-btn]').forEach(btn => {
        if (btn.getAttribute('data-cat-btn') === catKey) {
          btn.classList.add('active');
        } else {
          btn.classList.remove('active');
        }
      });
      renderProducts(catKey);
    }

    // Render danh mục bài viết trang chủ
    function renderPosts(postCat) {
      const blogGrid = document.getElementById('blog-grid');
      if (!blogGrid) return;

      const filtered = postCat === 'all'
        ? BLOG_POSTS
        : BLOG_POSTS.filter(p => p.cat === postCat);

      blogGrid.innerHTML = filtered.map(post => `
        <article class="bg-white rounded-lg border border-slate-200 shadow-sm hover:shadow-md transition flex flex-col justify-between overflow-hidden">
          <div>
            <div class="w-full aspect-[16/10] bg-slate-100 overflow-hidden cursor-pointer" onclick="openPostModal(${post.id})">
              <img 
                src="https://drive.google.com/thumbnail?id=${post.driveId}&sz=w700" 
                onerror="handleDriveImg(this, '${post.driveId}', '${post.title.replace(/'/g, '')}')"
                alt="${post.title}" 
                class="w-full h-full object-cover hover:scale-105 transition duration-300">
            </div>
            <div class="p-2.5 sm:p-3">
              <h3 onclick="openPostModal(${post.id})" class="product-title-full text-[12.5px] sm:text-[13.5px] font-bold text-brand-dark hover:text-brand-primary cursor-pointer mb-1.5">
                ${post.title}
              </h3>
              <p class="text-[11px] sm:text-xs text-slate-600 leading-relaxed">
                ${post.excerpt}
              </p>
            </div>
          </div>
          <div class="px-2.5 pb-2.5 sm:px-3 sm:pb-3 pt-1">
            <button type="button" onclick="openPostModal(${post.id})" class="text-[11px] font-bold text-brand-primary hover:text-brand-orange">
              Đọc tiếp →
            </button>
          </div>
        </article>
      `).join('');
    }

    function filterPosts(postCat) {
      document.querySelectorAll('.post-cat-btn').forEach(btn => {
        if (btn.getAttribute('data-post-btn') === postCat) {
          btn.classList.add('active');
        } else {
          btn.classList.remove('active');
        }
      });
      renderPosts(postCat);
    }

    // Xem chi tiết Sản phẩm / Bài viết trong Modal
    function openProductModal(id) {
      const item = PRODUCTS_DATA.find(p => p.id === id);
      if (!item) return;
      document.getElementById('modal-title').textContent = item.title;
      const modalImg = document.getElementById('modal-img');
      modalImg.setAttribute('data-fallback-step', '0');
      modalImg.src = 'https://drive.google.com/thumbnail?id=' + item.driveId + '&sz=w1000';
      modalImg.onerror = function() { handleDriveImg(this, item.driveId, item.title); };
      document.getElementById('modal-desc').textContent = item.desc + ' (' + item.spec + ').';
      document.getElementById('detail-modal').classList.remove('hidden');
    }

    function openPostModal(id) {
      const post = BLOG_POSTS.find(p => p.id === id);
      if (!post) return;
      document.getElementById('modal-title').textContent = post.title;
      const modalImg = document.getElementById('modal-img');
      modalImg.setAttribute('data-fallback-step', '0');
      modalImg.src = 'https://drive.google.com/thumbnail?id=' + post.driveId + '&sz=w1000';
      modalImg.onerror = function() { handleDriveImg(this, post.driveId, post.title); };
      document.getElementById('modal-desc').textContent = post.content;
      document.getElementById('detail-modal').classList.remove('hidden');
    }

    function closeModal() {
      document.getElementById('detail-modal').classList.add('hidden');
    }

    // Đóng mở menu trên điện thoại
    function toggleMobileMenu() {
      const drawer = document.getElementById('mobile-menu-drawer');
      const icon = document.getElementById('mobile-menu-icon');
      if (drawer.classList.contains('hidden')) {
        drawer.classList.remove('hidden');
        icon.className = 'fa-solid fa-xmark text-base';
      } else {
        drawer.classList.add('hidden');
        icon.className = 'fa-solid fa-bars text-base';
      }
    }

    // Điều khiển 2 Banner tự trượt chuyên nghiệp
    let currentBannerIndex = 0;
    let bannerInterval = null;

    function showBannerSlide(idx) {
      const slides = document.querySelectorAll('.banner-slide');
      const dots = document.querySelectorAll('.banner-dot');
      if (!slides.length) return;

      currentBannerIndex = (idx + slides.length) % slides.length;
      slides.forEach((s, i) => {
        if (i === currentBannerIndex) {
          s.classList.remove('hidden');
          s.classList.add('block');
        } else {
          s.classList.remove('block');
          s.classList.add('hidden');
        }
      });

      dots.forEach((d, i) => {
        if (i === currentBannerIndex) {
          d.className = 'banner-dot w-6 h-1.5 rounded-full bg-brand-accent transition-all';
        } else {
          d.className = 'banner-dot w-2.5 h-1.5 rounded-full bg-white/60 transition-all';
        }
      });
    }

    function changeSlide(step) {
      showBannerSlide(currentBannerIndex + step);
      resetBannerTimer();
    }

    function goToSlide(idx) {
      showBannerSlide(idx);
      resetBannerTimer();
    }

    function resetBannerTimer() {
      if (bannerInterval) clearInterval(bannerInterval);
      bannerInterval = setInterval(() => {
        showBannerSlide(currentBannerIndex + 1);
      }, 5000);
    }

    // Công cụ tư vấn chọn xe tự động
    function runVehicleAdvisor() {
      const type = document.getElementById('calc-type').value;
      const weight = parseFloat(document.getElementById('calc-weight').value) || 20;
      const height = parseFloat(document.getElementById('calc-height').value) || 3.0;
      const resultBox = document.getElementById('calc-result');

      let recommendation = '';
      if (weight <= 15 && height <= 3.0) {
        recommendation = 'Xe Fooc lùn 2-3 trục hoặc Xe cứu hộ sàn trượt chuyên dụng (Tải trọng tối ưu, cơ động nhanh).';
      } else if (weight <= 40 && height <= 3.5) {
        recommendation = 'Sơ mi rơ moóc lùn 40 Feet 3-4 trục (Hạ thấp trọng tâm máy, qua cầu vượt an toàn).';
      } else {
        recommendation = 'Rơ moóc lùn siêu trường siêu trọng đa trục / Moóc rút thủy lực kèm giấy phép lưu hành đặc biệt.';
      }

      resultBox.innerHTML = `
        <strong class="text-brand-primary block">Kết quả tư vấn (${type} - ${weight} tấn, cao ${height}m):</strong>
        <span>${recommendation} Liên hệ điều độ <strong>0961.797.119</strong> để nhận báo giá ngay!</span>
      `;
    }

    // Xử lý gửi Form Yêu Cầu Báo Giá Trang Chủ
    function submitQuoteForm(e) {
      e.preventDefault();
      const name = document.getElementById('q-name').value.trim();
      const phone = document.getElementById('q-phone').value.trim();
      const service = document.getElementById('q-service').value;
      const model = document.getElementById('q-model').value.trim() || 'Trao đổi trực tiếp';
      const fromLoc = document.getElementById('q-from').value.trim();
      const toLoc = document.getElementById('q-to').value.trim();

      const feedback = document.getElementById('quote-feedback');
      feedback.classList.remove('hidden');
      feedback.innerHTML = `
        <div class="font-bold text-emerald-900 mb-1">
          <i class="fa-solid fa-circle-check mr-1"></i>Đã ghi nhận yêu cầu báo giá của quý khách: ${name} (${phone})
        </div>
        <div>
          Dịch vụ: <strong>${service}</strong> (${model}) • Tuyến: <strong>${fromLoc} → ${toLoc}</strong>.<br>
          Bộ phận điều vận <strong>CÔNG TY TNHH TRUNG HIẾU ĐN (0961.797.119)</strong> sẽ liên hệ báo giá ngay!
        </div>
      `;
      document.getElementById('quote-request-form').reset();
    }

    // Tạo ảnh Thumbnail Logo tự động cho thẻ og:image khi chia sẻ link trang web
    function generateLogoShareThumbnail() {
      try {
        const canvas = document.createElement('canvas');
        canvas.width = 600;
        canvas.height = 315;
        const ctx = canvas.getContext('2d');
        if (!ctx) return;

        ctx.fillStyle = '#0f3e78';
        ctx.fillRect(0, 0, 600, 315);
        ctx.strokeStyle = '#f59e0b';
        ctx.lineWidth = 10;
        ctx.strokeRect(10, 10, 580, 295);

        ctx.fillStyle = '#f59e0b';
        ctx.font = 'bold 34px Inter, sans-serif';
        ctx.textAlign = 'center';
        ctx.fillText('CÔNG TY TNHH TRUNG HIẾU ĐN', 300, 115);

        ctx.fillStyle = '#ffffff';
        ctx.font = 'bold 24px Inter, sans-serif';
        ctx.fillText('CHUYÊN VẬN CHUYỂN XE CƠ GIỚI', 300, 165);

        ctx.fillStyle = '#e2e8f0';
        ctx.font = '18px Inter, sans-serif';
        ctx.fillText('trunghieudn.com | Hotline: 0961.797.119', 300, 215);
        ctx.fillText('58 Nguyễn Hữu Hào, P. Ngũ Hành Sơn, TP Đà Nẵng', 300, 250);
      } catch (err) {
        // Fallback giữ nguyên link thumbnail mặc định
      }
    }

    window.onload = function() {
      renderProducts('all');
      renderPosts('all');
      resetBannerTimer();
      generateLogoShareThumbnail();
    };
  </script>
</body>
</html>
