# Penjelasan Source Kode
## index.html

### Bagian Head
```HTML
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Linktree | @ereanoor</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Playwrite+NZ+Basic&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
```
Fungsi: Menggunakan standar HTML5 dan mengintegrasikan library eksternal seperti FontAwesome untuk ikon sosial media serta Google Fonts untuk tipografi yang modern.

### Bagian Profil (Header)
```HTML
<header class="profil">
    <div class="potoprofil">
        <img src="pp.png" alt="R. Noor Fikhri"> 
    </div>
    <h1 class="username">@ereanoor</h1>
    <p class="bio">Informatics Student | G1A024075</p>
</header>
```
Fungsi: Menampilkan identitas utama pengguna. Kelas .potoprofil membungkus foto dalam bentuk lingkaran, diikuti dengan username menggunakan font khusus dan bio singkat sebagai informasi akademik.

### Navigasi Tautan (Social Links)
```HTML
<nav class="social-links">
    <div class="sosmed primary mysosmed">
        <i class="fa-solid fa-globe"></i>
        <span>My Social Media</span>
    </div>
    
    <a href="https://instagram.com/noorfikhri" target="_blank" class="sosmed">
        <i class="fa-brands fa-instagram"></i>
        <span>Instagram</span>
    </a>
    </nav>
```
Fungsi: Implementasi daftar tautan menggunakan elemen <nav>. Terdapat pembeda antara elemen judul (.mysosmed) yang bersifat statis dan elemen anchor (<a>) yang berfungsi sebagai navigasi ke platform eksternal seperti Instagram, GitHub, dan LinkedIn.

## style.css
File ini mengatur estetika visual dan pengalaman pengguna (UX).

### Efek Glassmorphism
```CSS
.container {
    background: rgba(16, 33, 65, 0.6);
    backdrop-filter: blur(12px);
    -webkit-backdrop-filter: blur(12px);
    border: 2px solid #3498db;
    border-radius: 30px;
}
```
Fungsi: Menciptakan efek "kaca transparan" dengan menggunakan backdrop-filter. Warna latar belakang menggunakan rgba dengan transparansi rendah agar elemen di belakangnya terlihat samar.

### Animasi Entrance
```CSS
@keyframes fadeInScale {
    from { 
        opacity: 0; 
        transform: scale(0.95) translateY(10px); 
    }
    to { 
        opacity: 1; 
        transform: scale(1) translateY(0); 
    }
}
```
Fungsi: Memberikan efek visual yang halus saat halaman dimuat, di mana container akan sedikit membesar dan muncul dari bawah secara perlahan.
