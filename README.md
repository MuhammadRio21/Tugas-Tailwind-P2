# Tugas-Tailwind-P2
Muhammad Rio(2411102441270)

1. Konfigurasi Kolom untuk Tiap Breakpoint
Mobile (≤576px): 1 kolom (col-12)
Alasan:

Thumb reach zone: Pada mobile, area yang mudah dijangkau jempol adalah tengah layar
Cognitive load: 1 gambar per baris mengurangi beban kognitif, user fokus pada satu konten
Touch target: Gambar berukuran penuh lebih mudah di-tap (minimum 44px touch target)
Loading performance: Satu gambar per viewport mengurangi beban rendering

Tablet (576px-991px): 2-3 kolom (col-sm-6, col-md-4)
Alasan:

Screen real estate: Tablet memiliki ruang cukup untuk 2-3 kolom tanpa mengorbankan detail
Viewing distance: Tablet biasanya dipegang 40-60cm, optimal untuk scanning multiple items
Aspect ratio: Landscape tablet cocok untuk grid 3 kolom

Desktop (≥992px): 4 kolom (col-lg-3)
Alasan:

Desktop patterns: User desktop terbiasa dengan grid layout (seperti file explorer)
Mouse precision: Mouse memungkinkan interaksi dengan target kecil
Information density: Desktop dapat menampilkan lebih banyak informasi sekaligus

2. Strategi Tombol Follow/Edit Profile di Mobile
Pendekatan yang Digunakan:

Strategi Mobile-First:

Posisi Sentral: Tombol diletakkan di tengah layar, mudah dijangkau jempol
Vertical Stack: Menggunakan flex-column di mobile untuk stacking vertikal
Adequate Spacing: gap-2 memberikan jarak cukup antar tombol (minimum 8px)
Button Size: btn-sm dengan px-4 memberikan padding horizontal yang cukup
Visual Hierarchy: Primary button (Follow) dibedakan dengan warna

Potensi Masalah:

Performance Issues:

50 gambar = heavy page load
Memory consumption tinggi
Scroll performance menurun

Solusi
2. Performance Optimizations

Lazy Loading: Images dimuat hanya saat terlihat
Intersection Observer: Infinite scroll otomatis
Virtual Scrolling: Hanya render items yang visible
Image Compression: Ukuran berbeda untuk kategori berbeda
