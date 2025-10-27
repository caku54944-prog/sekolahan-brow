<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>SDN Contoh - Situs Resmi</title>
  <meta name="description" content="Situs resmi SDN Contoh - profil, berita, guru, galeri, dan pendaftaran online.">
  <style>
    :root{--accent:#0366d6;--muted:#6b7280;--bg:#f8fafc;--card:#ffffff}
    *{box-sizing:border-box}
    body{font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; margin:0; background:var(--bg); color:#0f172a; line-height:1.45}
    .container{max-width:1100px;margin:0 auto;padding:28px}
    header{background:linear-gradient(90deg, rgba(3,102,214,0.12), rgba(3,102,214,0.05));padding:22px;border-radius:12px;display:flex;gap:16px;align-items:center}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:56px;height:56px;border-radius:10px;background:var(--accent);display:flex;align-items:center;justify-content:center;color:white;font-weight:700}
    nav{margin-left:auto}
    nav a{margin-left:14px;text-decoration:none;color:var(--muted);font-weight:600}
    .hero{display:grid;grid-template-columns:1fr 380px;gap:20px;margin-top:22px}
    .card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(12,18,30,0.06)}
    h1{margin:0 0 8px 0;font-size:28px}
    p.lead{color:var(--muted);margin:0}
    .quick-links{display:flex;gap:8px;margin-top:12px}
    .btn{padding:10px 12px;border-radius:10px;border:0;background:var(--accent);color:#fff;font-weight:700;cursor:pointer}
    .outline{background:transparent;border:1px solid #e5e7eb;color:var(--muted)}

    section{margin-top:20px}
    .grid-3{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
    .news-item{display:flex;gap:12px}
    .news-item img{width:100px;height:70px;object-fit:cover;border-radius:8px}
    .teacher{display:flex;gap:12px;align-items:center}
    .teacher .avatar{width:64px;height:64px;border-radius:999px;background:#eef2ff;display:flex;align-items:center;justify-content:center;font-weight:700}

    .gallery{display:grid;grid-template-columns:repeat(4,1fr);gap:8px}
    .gallery img{width:100%;height:110px;object-fit:cover;border-radius:8px}

    form .row{display:flex;gap:8px}
    form input, form select, form textarea{width:100%;padding:10px;border-radius:8px;border:1px solid #e6edf3}
    form label{font-weight:600;color:#111827;margin-bottom:6px;display:block}
    .muted{color:var(--muted);font-size:13px}

    footer{margin-top:32px;padding:18px;text-align:center;color:var(--muted)}

    @media (max-width:920px){.hero{grid-template-columns:1fr} .grid-3{grid-template-columns:repeat(2,1fr)} .gallery{grid-template-columns:repeat(2,1fr)} }
    @media (max-width:560px){.grid-3{grid-template-columns:1fr} .gallery{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="logo">SD</div>
        <div>
          <div style="font-weight:800">SDN Contoh</div>
          <div class="muted" style="font-size:13px">Sekolah Dasar Negeri - Profil & Informasi</div>
        </div>
      </div>
      <nav>
        <a href="#about">Tentang</a>
        <a href="#berita">Berita</a>
        <a href="#guru">Guru</a>
        <a href="#ppdb">PPDB</a>
        <a href="#kontak">Kontak</a>
      </nav>
    </header>

    <main>
      <div class="hero">
        <div class="card">
          <h1>Selamat datang di SDN Contoh</h1>
          <p class="lead">Kami berdedikasi membangun karakter, kecerdasan, dan kreativitas siswa melalui lingkungan belajar yang aman dan inspiratif.</p>

          <div class="quick-links">
            <button class="btn" onclick="document.getElementById('ppdb').scrollIntoView({behavior:'smooth'})">Daftar PPDB</button>
            <button class="btn outline" onclick="document.getElementById('berita').scrollIntoView({behavior:'smooth'})">Lihat Berita</button>
          </div>

          <section id="about" style="margin-top:16px">
            <div class="card" style="background:transparent;padding:0;box-shadow:none">
              <h3>Visi</h3>
              <p class="muted">Menjadi sekolah unggul yang berkarakter, kreatif, dan berprestasi.</p>
              <h3> Misi</h3>
              <ul class="muted">
                <li>Meningkatkan kualitas pembelajaran berbasis karakter.</li>
                <li>Mengembangkan kreativitas dan potensi siswa.</li>
                <li>Membangun kerjasama dengan orang tua dan masyarakat.</li>
              </ul>
            </div>
          </section>
        </div>

        <aside>
          <div class="card" style="margin-bottom:12px">
            <strong>Info Sekolah</strong>
            <p class="muted" style="margin:8px 0 0 0">Alamat: Jl. Pendidikan No. 10, Desa Contoh<br>Telepon: (031) 123-4567<br>Email: info@sdncontoh.sch.id</p>
          </div>

          <div class="card">
            <strong>Jam Pelayanan</strong>
            <p class="muted" style="margin:8px 0 0 0">Senin - Jumat: 07.00 - 14.00</p>
          </div>
        </aside>
      </div>

      <section id="berita">
        <h2>Berita & Pengumuman</h2>
        <div class="card grid-3" style="padding:12px">
          <div class="news-item">
            <img src="https://picsum.photos/seed/1/400/300" alt="berita 1">
            <div>
              <div style="font-weight:700">Pembelajaran Luar Ruang</div>
              <div class="muted" style="font-size:13px">15 Okt 2025 — Siswa kelas 4 melakukan kunjungan edukasi ke kebun botani.</div>
            </div>
          </div>
          <div class="news-item">
            <img src="https://picsum.photos/seed/2/400/300" alt="berita 2">
            <div>
              <div style="font-weight:700">Lomba Seni Antar Kelas</div>
              <div class="muted" style="font-size:13px">10 Sep 2025 — Tim seni sekolah meraih juara 2 lomba kecamatan.</div>
            </div>
          </div>
          <div class="news-item">
            <img src="https://picsum.photos/seed/3/400/300" alt="berita 3">
            <div>
              <div style="font-weight:700">Pengumuman Libur</div>
              <div class="muted" style="font-size:13px">01 Nov 2025 — Libur nasional (hari besar keagamaan).</div>
            </div>
          </div>
        </div>
      </section>

      <section id="guru">
        <h2>Tim Pengajar</h2>
        <div class="card" style="padding:12px">
          <div class="teacher" style="margin-bottom:10px">
            <div class="avatar">AR</div>
            <div>
              <div style="font-weight:700">Aulia Rahma</div>
              <div class="muted">Guru Kelas 1</div>
            </div>
          </div>
          <div class="teacher" style="margin-bottom:10px">
            <div class="avatar">BN</div>
            <div>
              <div style="font-weight:700">Budi Nugroho</div>
              <div class="muted">Guru Matematika</div>
            </div>
          </div>
          <div class="teacher">
            <div class="avatar">CS</div>
            <div>
              <div style="font-weight:700">Citra Sari</div>
              <div class="muted">Guru Olahraga</div>
            </div>
          </div>
        </div>
      </section>

      <section id="galeri">
        <h2>Galeri Kegiatan</h2>
        <div class="card" style="padding:8px">
          <div class="gallery">
            <img src="https://picsum.photos/seed/g1/800/600" alt="kegiatan1">
            <img src="https://picsum.photos/seed/g2/800/600" alt="kegiatan2">
            <img src="https://picsum.photos/seed/g3/800/600" alt="kegiatan3">
            <img src="https://picsum.photos/seed/g4/800/600" alt="kegiatan4">
          </div>
        </div>
      </section>

      <section id="ppdb">
        <h2>Pendaftaran PPDB Online</h2>
        <div class="card" style="padding:12px">
          <p class="muted">Isi formulir di bawah ini. Data akan divalidasi secara sederhana pada sisi klien. Untuk produksi, butuh backend dan penyimpanan file yang aman.</p>
          <form id="ppdbForm" onsubmit="handlePPDB(event)">
            <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px">
              <div>
                <label>Nama Lengkap</label>
                <input id="nama" required>
              </div>
              <div>
                <label>Tanggal Lahir</label>
                <input id="ttl" type="date" required>
              </div>
            </div>
            <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:10px">
              <div>
                <label>Asal Sekolah</label>
                <input id="asal" required>
              </div>
              <div>
                <label>Jenis Kelamin</label>
                <select id="jk" required>
                  <option value="">Pilih...</option>
                  <option value="L">Laki-laki</option>
                  <option value="P">Perempuan</option>
                </select>
              </div>
            </div>
            <div style="margin-top:10px">
              <label>Alamat</label>
              <textarea id="alamat" rows="3" required></textarea>
            </div>
            <div style="margin-top:10px;display:flex;gap:8px;align-items:center">
              <div style="flex:1">
                <label>Upload Berkas (KTP/KK/Surat Sekolah)</label>
                <input id="file" type="file" accept="image/*,application/pdf">
                <div class="muted" style="font-size:12px;margin-top:6px">(Untuk demo: file tidak dikirimkan ke server. Hanya contoh front-end.)</div>
              </div>
              <div style="width:160px">
                <label>Kelas yang Dituju</label>
                <select id="kelas">
                  <option value="1">Kelas 1</option>
                  <option value="2">Kelas 2</option>
                  <option value="3">Kelas 3</option>
                </select>
              </div>
            </div>

            <div style="display:flex;gap:10px;margin-top:12px">
              <button class="btn" type="submit">Kirim Pendaftaran</button>
              <button type="button" class="btn outline" onclick="resetForm()">Reset</button>
            </div>
          </form>

          <div id="ppdbResult" style="margin-top:12px;display:none" class="card"></div>
        </div>
      </section>

      <section id="kontak">
        <h2>Kontak & Lokasi</h2>
        <div class="card grid-3" style="padding:12px">
          <div>
            <strong>Alamat</strong>
            <div class="muted">Jl. Pendidikan No.10, Desa Contoh</div>
          </div>
          <div>
            <strong>Email</strong>
            <div class="muted">info@sdncontoh.sch.id</div>
          </div>
          <div>
            <strong>Telepon</strong>
            <div class="muted">(031) 123-4567</div>
          </div>
        </div>
      </section>

    </main>

    <footer>
      © 2025 SDN Contoh — Dibuat dengan template sederhana. Untuk fitur lanjut (login admin, manajemen konten, backend PPDB) saya bisa bantu lanjutkan.
    </footer>
  </div>

  <script>
    function handlePPDB(e){
      e.preventDefault();
      const nama=document.getElementById('nama').value.trim();
      const ttl=document.getElementById('ttl').value;
      const alamat=document.getElementById('alamat').value.trim();
      const asal=document.getElementById('asal').value.trim();
      const jk=document.getElementById('jk').value;
      const kelas=document.getElementById('kelas').value;

      if(!nama || !ttl || !alamat || !asal || !jk){
        alert('Mohon lengkapi semua field yang wajib.');
        return;
      }

      const data={nama,ttl,alamat,asal,jk,kelas,submittedAt:new Date().toISOString()};
      // Untuk demo: tampilkan data sebagai JSON. Di produksi, kirim ke API server.
      const res=document.getElementById('ppdbResult');
      res.style.display='block';
      res.innerHTML=`<strong>Pendaftaran Diterima (Demo)</strong><pre style="white-space:pre-wrap">${JSON.stringify(data,null,2)}</pre>`;

      // reset simple
      document.getElementById('ppdbForm').reset();
    }
    function resetForm(){document.getElementById('ppdbForm').reset();document.getElementById('ppdbResult').style.display='none'}
  </script>
</body>
</html>
