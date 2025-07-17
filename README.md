<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Profil Biodata</title>
  <style>
    /* Reset & Base */
    *, *::before, *::after {
      box-sizing: border-box;
    }
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      background-color: #f8f9ff;
      color: #333;
      line-height: 1.4;
    }
    a {
      text-decoration: none;
      color: inherit;
    }
    /* Container with blue border and radius like example */
    .container {
      max-width: 960px;
      margin: 2rem auto;
      border: 15px solid #4f5bd5; /* vibrant blue */
      border-radius: 25px;
      background-color: white;
      padding: 0 1.5rem 2rem 1.5rem;
      box-shadow: 0 12px 20px rgb(79 91 213 / 0.2);
    }
    /* Section 1: Menu header */
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 20px;
      padding: 1rem 0;
      border-bottom: 2px solid #dee2e6;
      font-weight: 600;
      font-size: 1.1rem;
      background-color: #f0f1f9;
      border-radius: 20px 20px 0 0;
    }
    header nav a {
      padding: 0.45rem 0.8rem;
      color: #4f5bd5;
      border-radius: 8px;
      transition: background-color 0.3s ease;
    }
    header nav a:hover,
    header nav a:focus {
      background-color: #d6dbfd;
      outline: none;
    }
    /* Section 2 - Table layout: Left = text block, Right = image box */
    section#intro {
      margin-top: 1rem;
    }
    #intro table {
      border-collapse: collapse;
      width: 100%;
      margin-bottom: 2rem;
    }
    #intro table td {
      vertical-align: top;
      padding: 0.5rem 1rem;
    }
    #intro .text-left {
      font-size: 1.1rem;
      font-weight: 600;
      color: #4f5bd5;
      line-height: 1.3;
      max-width: 55ch;
      user-select: none;
    }
    #intro .text-left small {
      font-weight: 400;
      font-size: 0.9rem;
      color: #666;
      display: block;
      margin-top: 0.2rem;
    }
    #intro .image-right {
      text-align: right;
    }
    #intro .image-right img {
      max-width: 100%;
      height: auto;
      border-radius: 12px;
      box-shadow: 0 5px 12px rgb(79 91 213 / 0.3);
      user-select: none;
    }
    /* Section 3: Biodata with 6 boxes in a table */
    section#biodata {
      text-align: center;
      margin-bottom: 2rem;
    }
    section#biodata h2 {
      font-weight: 700;
      color: #2e2e59;
      margin-bottom: 0.3rem;
      font-size: 1.8rem;
      user-select: none;
    }
    section#biodata p.subtitle {
      font-size: 0.95rem;
      color: #7b7b9e;
      margin: 0 0 1.5rem 0;
      user-select: none;
      font-weight: 500;
    }
    #biodata table {
      width: 100%;
      border-collapse: collapse;
      table-layout: fixed;
      border-radius: 14px;
      overflow: hidden;
      box-shadow: 0 6px 18px rgb(79 91 213 / 0.12);
      background-color: white;
      user-select: none;
    }
    #biodata td {
      background-color: #e6e9fe;
      padding: 1rem 0;
      border-right: 1px solid white;
      font-weight: 600;
      font-size: 1rem;
      color: #414170;
    }
    #biodata td:last-child {
      border-right: 0;
    }
    /* Section 4: Portfolio */
    section#portfolio {
      user-select: none;
    }
    section#portfolio h2 {
      font-weight: 700;
      color: #2e2e59;
      margin-bottom: 1rem;
      font-size: 1.8rem;
      text-align: center;
    }
    #portfolio table {
      width: 100%;
      border-collapse: separate;
      border-spacing: 0 1rem;
    }
    #portfolio td {
      background-color: #f0f1f9;
      border-radius: 16px;
      vertical-align: top;
      padding: 0.75rem;
      width: 33.33%;
      box-shadow: 0 6px 15px rgb(79 91 213 / 0.1);
      text-align: center;
      font-weight: 600;
      color: #3a3a6b;
      font-size: 1rem;
      user-select: none;
    }
    #portfolio .image-box {
      width: 100%;
      height: auto;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgb(79 91 213 / 0.15);
      margin-bottom: 0.7rem;
      object-fit: cover;
      aspect-ratio: 350 / 200;
      background-color: #d0d4ff;
    }
    #portfolio .desc {
      font-weight: 500;
      font-size: 0.93rem;
      color: #60608e;
    }
    /* Responsive */
    @media (max-width: 768px) {
      #intro table {
        display: block;
      }
      #intro td {
        display: block;
        padding: 0.5rem 0;
        text-align: center;
      }
      #intro .image-right {
        margin-top: 1rem;
      }
      #portfolio table, #portfolio td {
        display: block;
        width: 100%;
      }
      #portfolio td {
        margin-bottom: 1rem;
      }
    }
  </style>
</head>
<body>
  <div class="container" role="main" aria-label="Halaman Profil Biodata">
    <!-- SECTION 1: MENU HEADER -->
    <header aria-label="Navigasi utama">
      <div class="brand" aria-label="Brand Website" style="font-weight:700; font-size:1.3rem; color:#4f5bd5; user-select:none;">Brams.web</div>
      <nav role="navigation" aria-label="Menu utama">
        <a href="#intro" tabindex="0" aria-current="page">Header</a>
        <a href="#biodata" tabindex="0">Biodata</a>
        <a href="#portfolio" tabindex="0">Portofolio</a>
      </nav>
    </header>

    <!-- SECTION 2: JUDUL DI KIRI DAN GAMBAR DI KANAN -->
    <section id="intro" aria-label="Bagian pengenalan">
      <table role="presentation" aria-hidden="true">
        <tbody>
          <tr>
            <td class="text-left" style="width:55%;">
              Selamat Datang di Website Saya
              <small>
              Ini adalah contoh website yang saya buat menggunakan promt AI (BlackBox AI)
              </small>
            </td>
            <td class="image-right" style="width:45%;">
              <img 
                src="https://p4.wallpaperbetter.com/wallpaper/264/666/478/3-316-16-9-aspect-ratio-s-sfw-wallpaper-preview.jpg" width="300px"
                alt="Gambar Orang berdiri"
                onerror="this.onerror=null;this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/afd64d17-20fe-410e-b524-8a6b8363d249.png';"
                loading="lazy"
              />
            </td>
          </tr>
        </tbody>
      </table>
    </section>

    <!-- SECTION 3: BIODATA 6 BOX -->
    <section id="biodata" aria-label="Biodata pribadi">
      <h2>Tentang Saya</h2>
      <p class="subtitle">Perkenalan diri dan apa yang saya lakukan</p>
      <table role="grid" aria-readonly="true" aria-label="Tabel biodata 6 kolom">
        <tbody>
          <tr>
            <td scope="row" aria-label="Full Name">
            Full Name
            <p> Bramastyo Trihasta Mardika
            </td>
            
            <td aria-label="Education">
            Education
            <p> SMK/SMA sederajat
            </td>
            <td aria-label="Occupation">
            Pekerjaan
            <p>Belum Bekerja
            </td>
          </tr>
          <tr>
            <td aria-label="Contact">
            Contact
            <p> Bramastyo08@gmail.com
           </td>
            <td aria-label="Hobbies">
            Hobi
            <p>Mendengar Musik, Bermain Game, Gym
            </td>
            <td aria-label="Address">
            Alamat
            <p>Indonesia Jakarta Timur
            </td>
          </tr>
        </tbody>
      </table>
    </section>

    <!-- SECTION 4: PORTOFOLIO -->
    <section id="portfolio" aria-label="Portofolio pekerjaan dan contoh hasil">
      <h2>Portofolio</h2>
      <table role="list" aria-label="Daftar portofolio">
        <tbody>
          <tr>
            <td role="listitem" tabindex="0" aria-label="Proyek 1 dengan deskripsi Deskripsi proyek 1">
              <img 
                class="image-box" 
                src="https://png.pngtree.com/png-clipart/20210829/original/pngtree-children-and-teenagers-hand-drawn-illustration-elements-png-image_6677053.jpg" 
                alt="Gambar Proyek 1"
                onerror="this.onerror=null;this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/833fa897-6a16-4982-a9a4-fbd3f54bb055.png';"
                loading="lazy"
              />
              <div class="desc">Proyek 1<br />Tiga orang sedang bermain</div>
            </td>
            <td role="listitem" tabindex="0" aria-label="Proyek 2 dengan deskripsi Deskripsi proyek 2">
              <img 
                class="image-box" 
                src="
                https://www.duniasantri.co/wp-content/uploads/2021/07/gradasi-burung.jpg" 
                alt="Gambar proyek 2"
                onerror="this.onerror=null;this.src='https://placehold.co/350x200?text=Image+Not+Found';"
                loading="lazy"
              />
              <div class="desc">Proyek 2<br />Gambar gradasi</div>
            </td>
            <td role="listitem" tabindex="0" aria-label="Proyek 3 dengan deskripsi Deskripsi proyek 3">
              <img 
                class="image-box" 
                src="https://superlive.id/storage/superadventure/2018/05/14/17cc2a0c28a6.jpg" 
                alt="Gambar persegi panjang vertikal berwarna abu-abu muda dengan teks Proyek 3 sebagai placeholder untuk portofolio proyek 3"
                onerror="this.onerror=null;this.src='https://placehold.co/350x200?text=Image+Not+Found';"
                loading="lazy"
              />
              <div class="desc">Proyek 3<br />Pemandangan dari Gunung Prau</div>
            </td>
          </tr>
        </tbody>
      </table>
    </section>
  </div>
</body>
</html>
