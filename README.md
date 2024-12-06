<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unitrive Smansa</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            color: #333;
            background-color: #f8f9fa;
            line-height: 1.6;
        }

        header {
            background-color: #007bff;
            color: #fff;
            padding: 20px;
            text-align: center;
            font-size: 2em;
            font-weight: bold;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        nav {
            background-color: #0056b3;
            display: flex;
            justify-content: center;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        nav a {
            color: #fff;
            padding: 15px 20px;
            text-decoration: none;
            font-size: 1.1em;
            transition: background-color 0.3s;
        }

        nav a:hover {
            background-color: #004494;
        }

        #home {
            background-color: red;
            color: #fff;
            padding: 100px 20px;
            min-height: 70vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
        }

        #home h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }

        #home p {
            max-width: 800px;
            font-size: 1.2em;
            text-align: center;
            margin: auto;
        }

        .gallery {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 80%;
            max-width: 600px;
            height: auto;
            border: 2px solid #ddd;
            border-radius: 5px;
            transition: transform 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.05);
            border-color: #007bff;
        }

        .works {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 20px;
        }

        .card-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
        }

        .works .card {
            width: 300px;
            padding: 15px;
            border: 1px solid #ddd;
            border-radius: 8px;
            background-color: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            text-align: center;
            cursor: pointer;
        }

        .works .card:hover {
            transform: scale(1.05);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }

        .works .card h3 {
            font-size: 1.5em;
            color: #007bff;
        }

        .works .card p {
            font-size: 1em;
            color: #555;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px;
        }

        footer a {
            color: #00e676;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }

        footer a:hover {
            color: #76ff03;
        }
    </style>
</head>
<body>
    <header>Unitrive Smansa</header>
    <nav>
        <a href="#" onclick="showSection('home')">Beranda</a>
        <a href="#" onclick="showSection('gallery')">Galeri</a>
        <a href="#" onclick="showSection('works')">Karya</a>
        <a href="#" onclick="showSection('about')">Tentang Kami</a>
    </nav>
    <section id="home">
        <h2>Dunia Unitrive</h2>
        <p>Selamat datang di Dunia Unitrive, tempat Anda menemukan informasi terpercaya dan inspirasi seputar kelas kami. Kami berkomitmen memberikan konten berkualitas yang mudah diakses, membantu Anda menjelajahi berbagai topik dengan cepat dan efektif. Selamat menjelajah!</p>
    </section>
    <section id="gallery" class="gallery" style="display: none;">
        <h2>Galeri</h2>
        <img src="Gambar/Foto Unitrive 1.jpg.jpeg" alt="Foto Unitrive 1">
        <img src="Gambar/Foto Unitrive 2.jpg.jpeg" alt="Foto Unitrive 2">
        <img src="Gambar/Foto Unitrive 3.jpg.jpeg" alt="Foto Unitrive 3">
        <img src="Gambar/Foto Unitrive 4.jpg.jpeg" alt="Foto Unitrive 4">
        <img src="Gambar/Foto Unitrive 5.jpg.jpeg" alt="Foto Unitrive 5">
    </section>
    <section id="works" class="works" style="display: none;">
    <h2>Karya</h2>
    <div class="card-container">
        <div class="card" onclick="showWorkDetails('AdityaSandi')"><h3>Aditya Sandi</h3></div>
        <div class="card" onclick="showWorkDetails('AlexaDanielHerlambang')"><h3>Alexa Daniel Herlambang</h3></div>
        <div class="card" onclick="showWorkDetails('ArgaTristanHasiholan')"><h3>Arga Tristan Hasiholan</h3></div>
        <div class="card" onclick="showWorkDetails('CahyaAwaludin')"><h3>Cahya Awaludin</h3></div>
        <div class="card" onclick="showWorkDetails('DivaJuliyantiPutri')"><h3>Diva Juliyanti Putri</h3></div>
        <div class="card" onclick="showWorkDetails('FachriSuryaKemal')"><h3>Fachri Surya Kemal</h3></div>
        <div class="card" onclick="showWorkDetails('FachrizalArshadBagus')"><h3>Fachrizal Arshad Bagus</h3></div>
        <div class="card" onclick="showWorkDetails('FadlanKaysanPermana')"><h3>Fadlan Kaysan Permana</h3></div>
        <div class="card" onclick="showWorkDetails('FajarMaulanaHidayat')"><h3>Fajar Maulana Hidayat</h3></div>
        <div class="card" onclick="showWorkDetails('FarrelArkaYazid')"><h3>Farrel Arka Yazid</h3></div>
        <div class="card" onclick="showWorkDetails('FitoDetimardarez')"><h3>Fito Detimardarez</h3></div>
        <div class="card" onclick="showWorkDetails('FransiscaRoseMayuri')"><h3>Fransisca Rose Mayuri</h3></div>
        <div class="card" onclick="showWorkDetails('ImanuelBenjaminPasaribu')"><h3>Imanuel Benjamin Pasaribu</h3></div>
        <div class="card" onclick="showWorkDetails('IzmiAlifatushifa')"><h3>Izmi Alifatushifa</h3></div>
        <div class="card" onclick="showWorkDetails('JovankaVeshaNdearly')"><h3>Jovanka Vesha Ndearly</h3></div>
        <div class="card" onclick="showWorkDetails('MaritzaAnevayLituhayu')"><h3>Maritza Anevay Lituhayu</h3></div>
        <div class="card" onclick="showWorkDetails('MedinaRahma')"><h3>Medina Rahma</h3></div>
        <div class="card" onclick="showWorkDetails('MifdaKamiel')"><h3>Mifda Kamiel</h3></div>
        <div class="card" onclick="showWorkDetails('MuhammadNurIhsanFaizen')"><h3>Muhammad Nur Ihsan Faizen</h3></div>
        <div class="card" onclick="showWorkDetails('MuhammadFadhilSyahreza')"><h3>Muhammad Fadhil Syahreza</h3></div>
        <div class="card" onclick="showWorkDetails('MuhammadAtharRaidisa')"><h3>Muhammad Athar Raidisa</h3></div>
        <div class="card" onclick="showWorkDetails('MuhammadGunturWibowo')"><h3>Muhammad Guntur Wibowo</h3></div>
        <div class="card" onclick="showWorkDetails('MuhammadMulkiHakim')"><h3>Muhammad Mulki Hakim</h3></div>
        <div class="card" onclick="showWorkDetails('MuhammadNabilHisyam')"><h3>Muhammad Nabil Hisyam</h3></div>
        <div class="card" onclick="showWorkDetails('MuhammadRizkiAnugrah')"><h3>Muhammad Rizki Anugrah</h3></div>
        <div class="card" onclick="showWorkDetails('NadyaUlyaZaenal')"><h3>Nadya Ulya Zaenal</h3></div>
        <div class="card" onclick="showWorkDetails('RadityaPratamaPutra')"><h3>Raditya Pratama Putra</h3></div>
        <div class="card" onclick="showWorkDetails('RaffaMilanoPoetro')"><h3>Raffa Milano Poetro</h3></div>
        <div class="card" onclick="showWorkDetails('ReniMardiyanti')"><h3>Reni Mardiyanti</h3></div>
        <div class="card" onclick="showWorkDetails('RepiAgustin')"><h3>Repi Agustin</h3></div>
        <div class="card" onclick="showWorkDetails('RizalBudiSampurno')"><h3>Rizal Budi Sampurno</h3></div>
        <div class="card" onclick="showWorkDetails('SyahdaNaylaZakiyah')"><h3>Syahda Nayla Zakiyah</h3></div>
        <div class="card" onclick="showWorkDetails('SyifaKurniaMeilani')"><h3>Syifa Kurnia Meilani</h3></div>
        <div class="card" onclick="showWorkDetails('TasyaAzzahra')"><h3>Tasya Azzahra</h3></div>
        <div class="card" onclick="showWorkDetails('ZahrahWahyuLathiifah')"><h3>Zahrah Wahyu Lathiifah</h3></div>
    </div>
</section>
    <footer>
        <p>Contact Service:</p>
        <p><a href="https://wa.me/6281214152634" target="_blank">Hubungi Fadlan Kaysan Permana di WhatsApp (0812-1415-2634)</a></p>
    </footer>
    <script>
        function showSection(sectionId) {
            document.querySelectorAll('section').forEach(section => section.style.display = 'none');
            document.getElementById(sectionId).style.display = 'block';
        }

       function showWorkDetails(group) {
    let message = "";
    switch (group) {
        case 'Arga Tristan Hasiholan':
            message = `
                <h3>Biografi Arga Tristan Hasiholan Tambunan</h3>
                <p><strong>NISN:</strong> 0083428019</p>
                <p><strong>Nama:</strong> Arga Tristan Hasiholan Tambunan</p>
                <p><strong>Tempat Tinggal:</strong> Purwakarta</p>
                <p><strong>Tanggal Lahir:</strong> 23 Februari 2008</p>
            `;
            break;
                <h2>Biografi</h2>
                <p>${message}</p>
                <button onclick="showSection('works')">Kembali</button>
            `;
        }

        showSection('home');
    </script>
</body>
</html>
