<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Rey's Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Roboto', sans-serif;
      line-height: 1.6;
      background-color: #f9f9f9;
      color: #333;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 2rem;
    }
    header {
      text-align: center;
      margin-bottom: 2rem;
    }
    header h1 {
      font-size: 2.5rem;
      color: #2c3e50;
    }
    header p {
      font-size: 1.2rem;
      color: #7f8c8d;
    }
    .profile-picture {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      object-fit: cover;
      margin: 1rem 0;
    }
    .section {
      width: 100%;
      max-width: 800px;
      margin-bottom: 3rem;
      background: white;
      padding: 1.5rem;
      border-radius: 8px;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }
    .section h2 {
      color: #2c3e50;
      margin-bottom: 1rem;
    }
    .project {
      margin-bottom: 1.5rem;
    }
    .contact a {
      display: block;
      margin: 0.5rem 0;
      color: #2980b9;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <header>
    <h1>Rey - Portfolio</h1>
    <!-- Foto Profil -->
    <img src="profile.jpg" alt="Rey's Profile Picture" class="profile-picture">
    <p>Mahasiswa Informatika dengan minat besar pada Data Science dan Database Administration, serta memiliki antusiasme terhadap analisis data dan pengembangan teknologi.</p>
  </header>

  <section class="section">
    <h2>Tentang Saya</h2>
    <p>Saya Rey, seorang mahasiswa Informatika yang memiliki ketertarikan dalam bidang Data Science dan Database Administration. Saya memiliki pengalaman dalam analisis data untuk penelitian akademik dan pengembangan program berbasis AI.</p>
  </section>

  <section class="section">
    <h2>Proyek</h2>
    <div class="project">
      <h3>Analisis Data Pendidikan di Salatiga</h3>
      <p>Proyek analisis data yang bertujuan memahami pengaruh faktor sosial ekonomi terhadap akses pendidikan mahasiswa rantau.</p>
    </div>
    <div class="project">
      <h3>Object Detection Classification</h3>
      <p>Pengembangan program pendeteksi objek untuk mata kuliah Artificial Intelligence menggunakan Python dan OpenCV.</p>
    </div>
    <div class="project">
      <h3>Video Edukasi Pergaulan Sehat</h3>
      <p>Video pendek yang mempromosikan pergaulan positif dalam lingkungan perkuliahan, bekerja dalam tim untuk menyampaikan pesan edukatif.</p>
    </div>
  </section>

  <section class="section contact">
    <h2>Kontak</h2>
    <a href="mailto:reynerpallo08@gmail.com">Email: reynerpallo08@gmail.com</a>
    <a href="https://github.com/reynerpallo">GitHub : reynerpallo</a>
    <a href="https://www.tiktok.com/@treeunivers_">TikTok:@treeunivers</a>
    <a href="https://www.instagram.com/treeunivers/ ">Instagram :@treeunivers </a>
  </section>

  <script>
    // Script tambahan untuk memastikan foto profil dapat diganti dinamis
    function changeProfilePicture() {
      const imageUrl = prompt("Masukkan URL foto profil baru:");
      if (imageUrl) {
        document.querySelector('.profile-picture').src = imageUrl;
      }
    }

    // Tambahkan event listener untuk demonstrasi
    const profilePicture = document.querySelector('.profile-picture');
    profilePicture.addEventListener('click', changeProfilePicture);
  </script>
</body>
</html>
