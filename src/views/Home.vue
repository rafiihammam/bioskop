<template>
<div id="home">
    <div class="container">
            <div class="row row-cols-4">
            <div class="col" v-for="(data, index) in movies" :key="index">
                <div class="image-area">
                    <img :src="data.image" class="image">
                </div>
                <div class="content-area">
                    <h4>{{ data.title}} ({{data.release}})</h4>
                    <span class="badge badge-pill badge-success margin-pill">{{ data.duration }}</span>
                    <p class="font-text">Dircted by : <b>{{ data.director }}</b></p>
                </div>
                <div class="button-area">
                    <button class="btn btn-info" @click="goToDetail(data.id)">Info</button>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
  name: 'Home',
  data () {
    return {
      title: 'Home',
      movies: [
        {
          title: 'Tenggelamnya Kapal Van Der Wijck',
          image: require('../assets/3.jpg'),
          duration: '113 min',
          director: 'Gina S. Noer',
          release: 2019,
          desc: 'Berlatar tahun 1930-an, dari tanah kelahirannya Makassar, Zainuddin (Herjunot Ali) berlayar menuju kampung halaman ayahnya di Batipuh, Padang Panjang. Di sana, ia bertemu dengan Hayati (Pevita Pearce), seorang gadis cantik jelita yang menjadi bunga di persukuannya. Kedua muda-mudi itu jatuh cinta. Namun, adat dan istiadat yang kuat meruntuhkan cinta mereka berdua. Zainuddin hanya seorang melarat yang tak bersuku; karena ibunya berdarah Bugis dan ayah berdarah Minang, statusnya dalam masyarakat Minang yang matrilineal tidak diakui. Oleh sebab itu, ia dianggap tidak memiliki pertalian darah lagi dengan keluarganya di Minangkabau. Sedangkan Hayati adalah perempuan Minang santun keturunan bangsawan.Pada akhirnya, lamaran Zainuddin ditolak keluarga Hayati. Hayati dipaksa menikah dengan Aziz (Reza Rahadian), laki-laki kaya terpandang yang lebih disukai keluarga Hayati daripada Zainuddin. Kecewa, Zainuddin pun memutuskan untuk berjuang, pergi dari ranah Minang dan merantau ke tanah Jawa demi bangkit melawan keterpurukan cintanya. Zainudin bekerja keras membuka lembaran baru hidupnya. Sampai akhirnya ia menjadi penulis terkenal dengan karya-karya masyhur dan diterima masyarakat seluruh Nusantara.Tetapi sebuah peristiwa tak diduga kembali menghampiri Zainuddin. Di tengah gelimang harta dan kemasyhurannya, dalam sebuah pertunjukan opera, Zainuddin kembali bertemu Hayati, kali ini bersama Aziz, suaminya. Pada akhirnya, kisah cinta Zainuddin dan Hayati menemui ujian terberatnya; Hayati pulang ke kampung halamannya dengan menaiki kapal Van der Wijck. Di tengah-tengah perjalanan, kapal yang dinaiki Hayati tenggelam. Sebelum kapal tenggelam, Zainuddin mengetahui bahwa Hayati sebetulnya masih mencintainya.',
          id: 1
        },
        {
          title: 'The Undisputed',
          image: require('../assets/1.jpg'),
          duration: '130 min',
          director: 'Justin Lin',
          release: 2011,
          desc: 'Dalam film pertama Undisputed, Scott Adkins tidak bermain dalam film ini. Barulah dalam Undisputed 2, Scott Adkins berperan sebagai Yuri Boyka dan menjadi ikon film seni bela diri. Film Undisputed 2 menampilkan Scott Adkins sebagai penjahat. Meskipun menjadi penjahat, sulit untuk membencinya karena dia benar-benar menunjukkan aksi bela diri yang sangat mengagumkan.Dia adalah seorang badass yang penggemar ingin ceritanya terus berlanjut dan hebatnya hal itu benar-benar terjadi karena Undisputed 3 dan 4 adalah film yang fantastis. Baik Undisputed 3 dan Undisputed 4 menampilkan beberapa adegan pertarungan terbaik dalam sejarah film seni bela diri',
          id: 2
        },
        {
          title: 'Crows Zero X Genjiaahhh',
          image: require('../assets/2.jpg'),
          duration: '142 min',
          director: 'Alfonso Cuaron',
          release: 2004,
          desc: 'Cerita dimulai dengan Takiya Genji (Oguri Shun), anak seorang bos Yakuza, memasuki Suzuran All-Boys High School sebagai senior ditransfer dengan tujuan menaklukkan itu. ... Mereka setuju bahwa jika Genji mengalahkan Suzuran, ia dapat mewarisi ayahnya keluarga Yakuza.',
          id: 3
        },
        {
          title: 'Serigala Terakhir',
          image: require('../assets/4.jpg'),
          duration: '102 min',
          director: 'Brian Fee',
          release: 2017,
          desc: 'Disebuah pinggiran Jakarta dengan sekelompok remaja laki-laki tumbuh dan menjalin persahabatan yang sangat kuat. Mereka adalah Ale (Fathir Muchtar), Jarot (Vino G. Bastian), Lukman (Dion Wiyoko), Sadat (Ali Syakieb), dan Jago (Dallas Pratama). Ale adalah sosok yang paling menonjol di antara mereka. Jiwa pemimpinnya sangat kentara sekali. Sementara Jarot adalah sosok yang paling tidak banyak omong dan tertutup.Suatu hari, ada pertandingan sepak bola antara kelompok Ale dan kelompok saingan. Setelah pertandingan, perkelahian pecah. Salah satu anggota saingan berencana untuk menusuk Ale. Namun, Jarot berhasil menggagalkan dengan memukul kepala penyerang dengan batu, akhirnya mati.Jarot ditangkap. Kelompok Ale, orang tua Jarot ini, dan adiknya Yani (Zaneta Georgina) terkejut. Kelompok Ale masih melakukan rutinitas mereka. Fathir ingin menjadi anggota kelompok, tetapi ditolak. Pulang ke rumah, ia melihat neneknya sudah mati; ia kemudian meninggalkan perkampungan kumuh. Sementara itu, di penjara, Jarot disiksa oleh narapidana lain. Selama jam berkunjung, ia cemburu narapidana lain, yang dikunjungi oleh keluarga mereka. Dia merindukan teman-temannya. Setelah itu, ia bertarung kembali melawan narapidana lain yang mengganggunya.Ketika keluar dari penjara, Jarot bertemu Fathir. Fathir membawa dia ke markas besar geng narkoba, Naga Hitam (Black Dragon). Jarot ditawarkan keanggotaan oleh pemimpin mereka (George Rudy), yang ia menerima. Jarot dan Fathir ditugaskan untuk melindungi distribusi obat di daerah kumuh rumahnya. Mereka harus berurusan dengan kelompok Ale. Jarot kemudian datang kembali ke rumah untuk melihat keluarga dan Aisyah. Dia mengungkapkan cintanya. Kemudian, adiknya Lukman meninggal karena overdosis. Untuk membalas dendam, Lukman berencana untuk membunuh Jarot, tetapi dia ditembak oleh Fathir. Sadat dan Jago sangat marah, dan berencana untuk memperkosa Yani. Jarot, marah, dan balas dendam dengan menyiksa mereka sampai mati.Ale belajar bahwa Aisyah jatuh cinta dengan Jarot. Dia mengunci dirinya di kamarnya. Namun, Aisyah berhasil melarikan diri dan memenuhi Jarot di atap untuk meminta dia untuk tinggal bersamanya; Jarot menolak. Setelah pertemuan tersebut, Aisyah didorong dari atap oleh Fathir dan mati segera. Jarot menganggap dia bunuh diri, sementara Ale mencurigai Jarot. Jarot panggilan Ale untuk menemuinya. Mereka melawan, dan Ale mengeluarkan pistolnya. Ketika mereka terus berjuang, tembakan terdengar; Ale tertembak dan mati. Saat ia berjalan pergi, Jarot ditembak dua kali oleh Fathir. Film ini ditutup dengan adegan yang menunjukkan Fathir sebagai sang serigala terakhir karena Fathir adalah pembunuh yang terakhir dan meninggalkan daerah kumuh dengan tujuan untuk membalas dendam kepada Kelompok Ale yang telah mencampakkannya. Adegan ditutup dengan Bara yang mengambil Pistol milik Ale yang menandakan bahwa dia telah mengambil kekuasaan Ale.',
          id: 4
        }
      ]
    }
  },
  methods: {
    goToDetail (proId) {
      this.$router.push({ name: 'detail', params: { Pid: proId } })
    }
  }
}

</script>

<style>
.container
{
    margin-top: 2%;
}
.font-text
{
    font-size: 9pt;
    margin: 10px 0;
}
.image-area
{
    width: 200px;
    height: 300px;
    text-align: center;
}
.image{
    width: 200px;
    height: 300px;
}
.content-area
{
    margin: 10px 0;
    height: 30%;
}
</style>
