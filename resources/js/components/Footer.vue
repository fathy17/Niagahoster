<template>
  <div>
    <div class="footer-1 py-2">
      <div class="container">
        <div class="row d-flex justify-content-center align-items-center">
          <div class="col-sm-6">Bagikan jika Anda menyukai halaman ini.</div>
          <div class="col-sm-6"></div>
        </div>
      </div>
    </div>
    <div class="footer-2 py-3">
      <div class="container d-flex justify-content-between align-items-center white">
        <h3>
          Perlu
          <strong>BANTUAN?</strong> Hubungi Kami :
          <strong>0274-5305505</strong>
        </h3>
        <div>
          <button class="btn btn-outline-light px-4" type="button">
            <span>
              <img class="chat" src="../../assets/svg/chat.svg" alt />
            </span> Live Chat
          </button>
        </div>
      </div>
    </div>
    <div class="footer-3 py-4">
      <div class="container">
        <div class="row">
          <div class="col-sm-6 col-lg-3 white">
            <h5 class="mb-3">HUBUNGI KAMI</h5>
            <p>0274-5305505</p>
            <p>Senin - Minggu</p>
            <p>24 Jam Nonstop</p>
            <p>Jl. Selokan Mataran Monjali</p>
            <p>Karangjati MT</p>
            <p>Sinduadi, Mlati, Sleman</p>
            <p>Yogyakarta 55284</p>
          </div>
          <div class="col-sm-6 col-lg-3 white">
            <h5 class="mb-3">LAYANAN</h5>
            <p>Domain</p>
            <p>Shared Hosting</p>
            <p>Cloud VPS Hosting</p>
            <p>Managed VPS Hosting</p>
            <p>Web Builder</p>
            <p>Keamanan SSL / HTTPS</p>
            <p>Jasa Pembuatan Website</p>
            <p>Program Afiliasi</p>
          </div>
          <div class="col-sm-6 col-lg-3 white">
            <h5 class="mb-3">SERVICE HOSTING</h5>
            <p>Hosting Murah</p>
            <p>Hostung Indonesia</p>
            <p>Hosting Singapura SG</p>
            <p>Hosting PHP</p>
            <p>Hosting Wordpress</p>
            <p>Hosting Laravel</p>
          </div>
          <div class="col-sm-6 col-lg-3 white">
            <h5 class="mb-3">TUTORIAL</h5>
            <p>Knowledgebase</p>
            <p>Blog</p>
            <p>Cara Pembayaran</p>
          </div>
          <div class="col-sm-6 col-lg-3 white">
            <h5 class="mb-3">TENTANG KAMI</h5>
            <p>Tim Niagahoster</p>
            <p>Karir</p>
            <p>Events</p>
            <p>Penawaran dan Promo Spesial</p>
            <p>Kontak Kami</p>
          </div>
          <div class="col-sm-6 col-lg-3 white">
            <h5 class="mb-3">KENAPA PILIH NIAGAHOSTER?</h5>
            <p>Support Terbaik</p>
            <p>Garansi Harga Termurah</p>
            <p>Domain Gratis Selamanya</p>
            <p>Datacenter Hosting Terbaik</p>
            <p>Review Pelanggan</p>
          </div>
          <div class="col-sm-6 col-lg-3 white">
            <h5 class="mb-3">NEWS LETTER</h5>
            <div class="input-group mb-1">
              <input
                type="text"
                class="form-control"
                placeholder="Email"
                aria-label="Recipient's username"
                aria-describedby="button-addon2"
              />
              <div class="input-group-append">
                <button class="btn btn-primary" type="button" id="button-addon2">Berlangganan</button>
              </div>
            </div>
            <div>Dpatkan promo dan konten menarik dari penyedia hosting terbaik Anda</div>
          </div>
          <div class="col-sm-6 col-lg-3 white">
            <div class="d-flex justify-content-between">
              <img src="../../assets/svg/facebook.svg" alt />
              <img src="../../assets/svg/facebook.svg" alt />
              <img src="../../assets/svg/facebook.svg" alt />
            </div>
          </div>
          <div class="col-sm-12 brdr mb-4 pb-4">
            <h5 class="mb-3">PEMBAYARAN</h5>
            <p>-----------------</p>
            <div>Aktifasi instan dengan e-payment. Hosting dan domain langsung aktif!</div>
          </div>
          <div class="col-sm-8 white">
            <p
              class="small"
            >Copyright 2016 Niagahoster | Hosting powerd by PHP7, CloudLinux, CloudFlare, BitNinja and DC Biznet Technovillage Jakarta</p>
            <p
              class="small"
            >Cloud VPS Murah powered by Webuzo Softculous, Intel SSD and cloud computing technology</p>
          </div>
          <div class="col-sm-4 white">
            <p class="small">Syarat dan ketentuan | Kebijakan privasi</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style scoped>
.footer-1 {
  background-color: #dddddd;
  height: 100%;
}

.footer-2 {
  background-color: #00a2f3;
  height: 100%;
}

.footer-3 {
  height: 100%;
  background-color: #303030;
}

.container,
.row {
  height: 100%;
}

.white h3,
.white strong,
.white p {
  color: white;
}

.brdr {
  border-bottom: 1px solid black;
}

.col-sm-6.white {
  margin: 1rem 0;
}

.chat {
  width: 1rem;
  z-index: 2;
}

.chat:hover {
  color: black;
}
</style>