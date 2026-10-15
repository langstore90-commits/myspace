<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MySpace 🚀 | Personal Website</title>

<style>
* {
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #050817;
    color: white;
    overflow-x: hidden;
}

header {
    text-align: center;
    padding: 22px 10px;
    background: #0a1030;
    border-bottom: 1px solid #5542a5;
}

.logo {
    font-size: 30px;
    font-weight: bold;
    color: #d8b4fe;
}

header p {
    color: #a5b4fc;
    margin-bottom: 0;
}

nav {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 7px;
    padding: 12px 5px;
    background: #0b1230;
    position: sticky;
    top: 0;
    z-index: 10;
    border-bottom: 1px solid #292d62;
}

nav button {
    background: transparent;
    color: #ddd6fe;
    border: 1px solid transparent;
    padding: 10px 12px;
    border-radius: 20px;
    cursor: pointer;
    font-size: 13px;
    margin: 0;
}

nav button.active,
nav button:hover {
    background: linear-gradient(90deg, #7c3aed, #c026d3);
    color: white;
}

.page {
    display: none;
    animation: masuk .4s ease;
}

.page.active {
    display: block;
}

@keyframes masuk {
    from {
        opacity: 0;
        transform: translateY(12px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.hero {
    text-align: center;
    padding: 55px 18px;
    background: linear-gradient(140deg, #101c51, #492078, #101638);
    position: relative;
    overflow: hidden;
}

.hero h1 {
    font-size: clamp(28px, 6vw, 48px);
}

.gradient {
    background: linear-gradient(90deg, #c4b5fd, #f0abfc, #93c5fd);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.rocket {
    display: inline-block;
    font-size: 70px;
    animation: terbang 3s ease-in-out infinite;
}

@keyframes terbang {
    0%, 100% {
        transform: translateY(0) rotate(-10deg);
    }
    50% {
        transform: translateY(-20px) rotate(8deg);
    }
}

.container {
    width: 92%;
    max-width: 850px;
    margin: 25px auto;
}

.card {
    background: linear-gradient(145deg, #111d40, #101329);
    border: 1px solid #35386e;
    border-radius: 18px;
    padding: 22px;
    margin-bottom: 20px;
    box-shadow: 0 8px 25px #0003;
}

h2 {
    color: #d8b4fe;
}

p {
    line-height: 1.7;
}

.center {
    text-align: center;
}

button,
.btn {
    display: inline-block;
    border: none;
    padding: 12px 17px;
    margin: 5px 3px;
    border-radius: 25px;
    background: linear-gradient(90deg, #7c3aed, #c026d3);
    color: white;
    font-weight: bold;
    cursor: pointer;
    text-decoration: none;
    transition: .25s;
}

button:hover,
.btn:hover {
    transform: translateY(-2px);
    filter: brightness(1.15);
}

.avatar {
    width: 125px;
    height: 125px;
    object-fit: cover;
    border-radius: 50%;
    border: 4px solid #a78bfa;
    background: #29245b;
}

.info {
    padding: 13px;
    margin-top: 10px;
    background: #090f29;
    border: 1px solid #252d56;
    border-radius: 10px;
    overflow-wrap: anywhere;
}

.info strong {
    color: #c4b5fd;
}

input,
textarea {
    width: 100%;
    padding: 12px;
    margin-top: 7px;
    border: 1px solid #424979;
    border-radius: 10px;
    background: #080e25;
    color: white;
    font-size: 15px;
}

input[type="file"] {
    font-size: 13px;
}

label {
    display: block;
    margin-top: 15px;
    color: #c7d2fe;
}

textarea {
    min-height: 90px;
    resize: vertical;
}

.gallery {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 10px;
    margin-top: 18px;
}

.gallery img {
    width: 100%;
    height: 150px;
    object-fit: cover;
    border-radius: 12px;
    border: 1px solid #7662d5;
}

.star {
    position: fixed;
    z-index: 20;
    pointer-events: none;
    animation: kelap 1.5s infinite alternate;
}

@keyframes kelap {
    from { opacity: .3; }
    to { opacity: 1; }
}

footer {
    text-align: center;
    padding: 25px 10px;
    background: #080d20;
    color: #a5b4fc;
    font-size: 13px;
}

.status {
    color: #86efac;
    overflow-wrap: anywhere;
}

.small {
    color: #a5b4fc;
    font-size: 13px;
}

@media (max-width: 500px) {
    nav button {
        padding: 9px;
        font-size: 12px;
    }

    .card {
        padding: 16px;
    }

    .hero {
        padding: 40px 12px;
    }
}
</style>
</head>

<body>

<header>
    <div class="logo">🚀 MySpace</div>
    <p>Dream • Learn • Grow • Shine ✨</p>
</header>

<nav>
    <button class="active" data-page="home">🏠 Home</button>
    <button data-page="profil">👤 Profil</button>
    <button data-page="sekolah">🏫 Sekolah</button>
    <button data-page="galeri">🖼️ Galeri</button>
    <button data-page="edit">✏️ Edit</button>
</nav>

<!-- HOME -->
<section class="page active" id="home">

    <div class="hero">
        <div class="rocket">🚀</div>

        <h1>Welcome to <span class="gradient">MySpace!</span></h1>

        <p>
            🌌 Selamat datang di dunia pribadiku!<br>
            Kenali diriku, sekolahku, dan impianku.
        </p>

        <button onclick="pindah('profil')">Kenali Aku 👤</button>
        <button onclick="pindah('sekolah')">Sekolahku 🏫</button>
        <br>
        <button onclick="buatBintang()">✨ Kejutan Bintang</button>
    </div>

    <main class="container">
        <section class="card center">
            <h2>🌟 Welcome to My Universe</h2>
            <p>
                Ini adalah ruang pribadiku untuk berbagi cerita,
                mengenalkan diriku, dan menyimpan kenangan.
            </p>
            <p>🚀 Explore the universe. Dream without limits. ⭐</p>
        </section>

        <section class="card center">
            <h2>🪐 Explore MySpace</h2>
            <button onclick="pindah('profil')">👤 Profil Pribadi</button>
            <button onclick="pindah('sekolah')">🏫 Profil Sekolah</button>
            <button onclick="pindah('galeri')">🖼️ Galeri Foto</button>
            <button onclick="pindah('edit')">✏️ Isi Dataku</button>
        </section>

        <section class="card center">
            <h2>💫 Daily Motivation</h2>
            <p id="kata">
                Mimpilah setinggi bintang dan teruslah berusaha! 🚀
            </p>
            <button onclick="gantiKata()">Ganti Kata ✨</button>
        </section>
    </main>
</section>

<!-- PROFIL -->
<section class="page" id="profil">
    <main class="container">

        <section class="card center">
            <img id="fotoTampil" class="avatar" alt="Foto profil"
            src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 120 120'%3E%3Crect width='120' height='120' fill='%2329245b'/%3E%3Ctext x='60' y='80' font-size='60' text-anchor='middle'%3E%F0%9F%91%A4%3C/text%3E%3C/svg%3E">

            <h1 id="namaTampil">Nama Kamu ✨</h1>
            <p id="kelasTampil">Kelas belum diisi</p>
            <p id="tentangTampil">Halo! Selamat datang di profilku.</p>

            <button onclick="pindah('edit')">✏️ Edit Profil</button>
        </section>

        <section class="card">
            <h2>✨ Informasi Pribadi</h2>

            <div class="info">Nama panggilan: <strong id="panggilanTampil">Belum diisi</strong></div>
            <div class="info">Umur: <strong id="umurTampil">Belum diisi</strong></div>
            <div class="info">Hobi: <strong id="hobiTampil">Belum diisi</strong></div>
            <div class="info">Cita-cita: <strong id="citaTampil">Belum diisi</strong></div>
        </section>

    </main>
</section>

<!-- SEKOLAH -->
<section class="page" id="sekolah">
    <main class="container">

        <section class="card center">
            <div style="font-size:75px">🏫</div>
            <h1 id="sekolahTampil">Sekolahku</h1>
            <p id="alamatTampil">Alamat sekolah belum diisi.</p>
            <button onclick="pindah('edit')">✏️ Edit Sekolah</button>
        </section>

        <section class="card">
            <h2>📚 Informasi Sekolah</h2>

            <div class="info">Wali kelas: <strong id="waliTampil">Belum diisi</strong></div>
            <div class="info">Jurusan: <strong id="jurusanTampil">Belum diisi</strong></div>
            <div class="info">Pelajaran favorit: <strong id="mapelTampil">Belum diisi</strong></div>
            <div class="info">Motto hidup: <strong id="mottoTampil">Terus belajar dan berkembang!</strong></div>
        </section>

    </main>
</section>

<!-- GALERI -->
<section class="page" id="galeri">
    <main class="container">

        <section class="card">
            <h2>🖼️ Galeri Kenangan</h2>
            <p>Pilih foto dari galeri HP kamu. Maksimal 6 foto.</p>

            <input type="file" id="inputGaleri" accept="image/*" multiple>

            <div class="gallery" id="galeriTampil"></div>

            <button onclick="hapusGaleri()">🗑️ Hapus Semua Foto</button>
            <p class="small">Gunakan foto berukuran kecil agar penyimpanan tidak penuh.</p>
            <p id="statusGaleri" class="status"></p>
        </section>

    </main>
</section>

<!-- EDIT -->
<section class="page" id="edit">
    <main class="container">

        <section class="card">
            <h2>✏️ Edit Profilku</h2>
            <p>Isi informasi berikut, kemudian tekan Simpan Data.</p>

            <form id="formProfil">

                <label>Foto profil</label>
                <input type="file" id="fotoInput" accept="image/*">

                <label>Nama lengkap</label>
                <input id="nama" maxlength="80" placeholder="Nama lengkap">

                <label>Nama panggilan</label>
                <input id="panggilan" maxlength="50" placeholder="Nama panggilan">

                <label>Umur</label>
                <input id="umur" type="number" min="1" max="120" placeholder="Umur">

                <label>Kelas</label>
                <input id="kelas" maxlength="50" placeholder="Contoh: XI A">

                <label>Hobi</label>
                <input id="hobi" maxlength="200" placeholder="Hobi kamu">

                <label>Cita-cita</label>
                <input id="cita" maxlength="100" placeholder="Cita-cita kamu">

                <label>Tentang diriku</label>
                <textarea id="tentang" maxlength="800" placeholder="Ceritakan tentang dirimu"></textarea>

                <h2 style="margin-top:30px">🏫 Informasi Sekolah</h2>

                <label>Nama sekolah</label>
                <input id="sekolah" maxlength="150" placeholder="Nama sekolah">

                <label>Alamat sekolah</label>
                <input id="alamat" maxlength="250" placeholder="Alamat sekolah">

                <label>Wali kelas</label>
                <input id="wali" maxlength="100" placeholder="Nama wali kelas">

                <label>Jurusan</label>
                <input id="jurusan" maxlength="100" placeholder="Jurusan">

                <label>Pelajaran favorit</label>
                <input id="mapel" maxlength="100" placeholder="Pelajaran favorit">

                <label>Motto hidup</label>
                <input id="motto" maxlength="250" placeholder="Motto hidup">

                <button type="submit">💾 Simpan Data</button>
            </form>

            <p id="statusEdit" class="status"></p>
        </section>

    </main>
</section>

<footer>
    <p>© <span id="tahun"></span> MySpace 🚀</p>
    <p>Dibuat dengan ❤️ HTML, CSS & JavaScript</p>
</footer>

<script>
const $ = id => document.getElementById(id);

const fields = [
    "nama", "panggilan", "umur", "kelas", "hobi",
    "cita", "tentang", "sekolah", "alamat",
    "wali", "jurusan", "mapel", "motto"
];

const defaults = {
    nama: "Nama Kamu ✨",
    panggilan: "",
    umur: "",
    kelas: "",
    hobi: "",
    cita: "",
    tentang: "Halo! Selamat datang di profilku. 🚀",
    sekolah: "Nama Sekolahku",
    alamat: "",
    wali: "",
    jurusan: "",
    mapel: "",
    motto: "Terus belajar dan berkembang!",
    foto: "",
    galeri: []
};

let data = {...defaults};

try {
    const saved = localStorage.getItem("mySpaceAllInOne");

    if (saved) {
        const parsed = JSON.parse(saved);

        fields.forEach(key => {
            if (parsed[key] !== undefined &&
                parsed[key] !== null) {
                data[key] = String(parsed[key]);
            }
        });

        if (typeof parsed.foto === "string") {
            data.foto = parsed.foto;
        }

        if (Array.isArray(parsed.galeri)) {
            data.galeri = parsed.galeri
                .filter(item => typeof item === "string")
                .slice(-6);
        }
    }
} catch (error) {
    console.log("Data belum tersedia.");
}

function simpan() {
    try {
        localStorage.setItem("mySpaceAllInOne", JSON.stringify(data));
        return true;
    } catch (error) {
        return false;
    }
}

function pindah(id) {
    document.querySelectorAll(".page").forEach(page => {
        page.classList.toggle("active", page.id === id);
    });

    document.querySelectorAll("nav button").forEach(button => {
        button.classList.toggle("active", button.dataset.page === id);
    });

    history.replaceState(null, "", "#" + id);
    window.scrollTo({top: 0, behavior: "smooth"});

    if (id === "edit") isiForm();
    render();
}

document.querySelectorAll("nav button").forEach(button => {
    button.addEventListener("click", () => {
        pindah(button.dataset.page);
    });
});

function isiForm() {
    fields.forEach(key => {
        const input = $(key);
        if (input) input.value = data[key] || "";
    });
}

function setText(id, value, fallback = "Belum diisi") {
    const el = $(id);
    if (el) el.textContent = value || fallback;
}

function render() {
    setText("namaTampil", data.nama, "Nama Kamu ✨");
    setText("panggilanTampil", data.panggilan);
    setText("umurTampil", data.umur ? data.umur + " tahun" : "");
    setText("kelasTampil", data.kelas, "Kelas belum diisi");
    setText("hobiTampil", data.hobi);
    setText("citaTampil", data.cita);
    setText("tentangTampil", data.tentang);
    setText("sekolahTampil", data.sekolah, "Sekolahku");
    setText("alamatTampil", data.alamat);
    setText("waliTampil", data.wali);
    setText("jurusanTampil", data.jurusan);
    setText("mapelTampil", data.mapel);
    setText("mottoTampil", data.motto, "Terus belajar dan berkembang!");

    if (data.foto) {
        $("fotoTampil").src = data.foto;
    }

    renderGaleri();
}

$("fotoInput").addEventListener("change", async function() {
    const file = this.files[0];

    if (!file) return;

    if (!file.type.startsWith("image/") ||
        file.size > 1024 * 1024) {
        alert("Pilih gambar maksimal 1 MB.");
        this.value = "";
        return;
    }

    try {
        data.foto = await bacaFoto(file);

        if (!simpan()) {
            alert("Penyimpanan penuh. Coba foto yang lebih kecil.");
        } else {
            render();
            $("statusEdit").textContent = "Foto profil dipilih. Tekan Simpan Data untuk menyimpan perubahan.";
        }
    } catch (error) {
        alert("Foto gagal dibaca.");
    }
});

function bacaFoto(file) {
    return new Promise((resolve, reject) => {
        const reader = new FileReader();
        reader.onload = () => resolve(reader.result);
        reader.onerror = reject;
        reader.readAsDataURL(file);
    });
}

$("formProfil").addEventListener("submit", function(event) {
    event.preventDefault();

    const updated = {...data};

    fields.forEach(key => {
        updated[key] = $(key).value.trim();
    });

    if (updated.umur &&
        (!Number.isInteger(Number(updated.umur)) ||
         Number(updated.umur) < 1 ||
         Number(updated.umur) > 120)) {
        $("statusEdit").textContent = "Periksa kembali umur yang kamu masukkan.";
        return;
    }

    data = updated;

    if (simpan()) {
        $("statusEdit").textContent = "✅ Data berhasil disimpan! Profil dan sekolah sudah diperbarui.";
        render();
    } else {
        $("statusEdit").textContent = "Penyimpanan gagal. Kurangi ukuran foto atau galeri.";
    }
});

function renderGaleri() {
    const area = $("galeriTampil");
    area.replaceChildren();

    if (!data.galeri.length) {
        const message = document.createElement("p");
        message.textContent = "Belum ada foto. Tambahkan foto dari galeri HP kamu! 🌌";
        area.appendChild(message);
        return;
    }

    data.galeri.forEach(src => {
        const img = document.createElement("img");
        img.src = src;
        img.alt = "Foto kenangan";
        area.appendChild(img);
    });
}

$("inputGaleri").addEventListener("change", async function() {
    const files = Array.from(this.files || []);

    for (const file of files) {
        if (data.galeri.length >= 6) {
            alert("Maksimal 6 foto. Hapus foto lama untuk menambahkan foto baru.");
            break;
        }

        if (!file.type.startsWith("image/") ||
            file.size > 250 * 1024) {
            alert("Setiap foto maksimal 250 KB.");
            continue;
        }

        try {
            const src = await bacaFoto(file);
            data.galeri.push(src);

            if (!simpan()) {
                data.galeri.pop();
                alert("Penyimpanan penuh. Hapus beberapa foto terlebih dahulu.");
                break;
            }
        } catch (error) {
            alert("Foto gagal dibaca.");
        }
    }

    renderGaleri();
    this.value = "";
});

function hapusGaleri() {
    if (!confirm("Yakin ingin menghapus semua foto galeri?")) return;

    data.galeri = [];

    if (simpan()) {
        renderGaleri();
        $("statusGaleri").textContent = "Galeri berhasil dibersihkan.";
    } else {
        $("statusGaleri").textContent = "Gagal menyimpan perubahan.";
    }
}

function buatBintang() {
    for (let i = 0; i < 22; i++) {
        const star = document.createElement("span");

        star.textContent = ["⭐", "✨", "🌟", "💫"][
            Math.floor(Math.random() * 4)
        ];

        star.style.cssText =
            `position:fixed;z-index:99;pointer-events:none;
            left:${Math.random() * 95}vw;
            top:${Math.random() * 90}vh;
            font-size:${18 + Math.random() * 18}px;
            transition:1.4s`;

        document.body.appendChild(star);

        requestAnimationFrame(() => {
            star.style.transform = "translateY(-120px) rotate(180deg)";
            star.style.opacity = "0";
        });

        setTimeout(() => star.remove(), 1450);
    }
}

const kataKata = [
    "Mimpilah setinggi bintang dan teruslah berusaha! 🚀",
    "Setiap hari adalah kesempatan untuk berkembang! 🌟",
    "Jangan takut mencoba hal baru! ✨",
    "Masa depan dimulai dari usaha hari ini! 🌌",
    "Kamu punya kesempatan untuk bersinar! 💫"
];

function gantiKata() {
    const random = Math.floor(Math.random() * kataKata.length);
    $("kata").textContent = kataKata[random];
}

function latarBintang() {
    for (let i = 0; i < 45; i++) {
        const star = document.createElement("span");

        star.className = "star";
        star.textContent = Math.random() > 0.5 ? "✦" : "·";
        star.style.left = Math.random() * 100 + "vw";
        star.style.top = Math.random() * 100 + "vh";
        star.style.fontSize = 10 + Math.random() * 15 + "px";
        star.style.animationDelay = Math.random() * 3 + "s";

        document.body.appendChild(star);
    }
}

$("tahun").textContent = new Date().getFullYear();

latarBintang();
render();

const halamanAwal = location.hash.replace("#", "");

if (["home", "profil", "sekolah", "galeri", "edit"].includes(halamanAwal)) {
    pindah(halamanAwal);
} else {
    pindah("home");
}
</script>

</body>
</html>