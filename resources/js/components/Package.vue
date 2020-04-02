<template>
  <div class="text-center mt-5">
    <h3 class="font-weight-bold mb-2">Paket Hosting Singapura yang Tepat</h3>
    <h4>Diskon 40% + Domain SSL Gratis untuk Anda</h4>
    <div class="row mt-4">
      <div class="col-sm-12 col-lg-3 no-padding" v-for="item in packages" :key="item.nama">
        <div v-if="!item.bestSeller" class="custom-card">
          <div class="border pt-2 pb-2">
            <h3 class="font-weight-bold">{{item.nama}}</h3>
          </div>
          <div class="border pt-2 pb-2">
            <p class="harga">Rp. {{item.harga}}</p>
            <div class="row justify-content-center">
              <p class="mr-1">Rp</p>
              <h1
                class="font-weight-bold"
              >{{item.hargaDisc.substring(0, item.hargaDisc.lastIndexOf('.'))}}</h1>
              <p
                class="font-weight-bold"
              >{{item.hargaDisc.substring(item.hargaDisc.lastIndexOf('.'), item.hargaDisc.length)}}</p>
            </div>
          </div>
          <div class="border pt-2 pb-2">
            <span class="font-weight-bold">{{item.user}}</span>
            <span>Pengguna Terdaftar</span>
          </div>
          <div class="border pt-2 pb-2">
            <p class="font-weight-bold">{{item.resource}}X RESOURCE POWER</p>
            <div>
              <span class="font-weight-bold">{{item.space}}</span>
              <span>Disk Space</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.bandwidth}}</span>
              <span>Bandwidth</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.email}}</span>
              <span>POP3 Email</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.database}}</span>
              <span>Databases</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.addons}}</span>
              <span>Addon Domains</span>
            </div>
            <div v-if="item.backup !== 'Instant'">
              <span class="font-weight-bold">{{item.backup}}</span>
              <span>Backup & Restore</span>
            </div>
            <div v-else>
              <span class="font-weight-bold">{{item.backup}}</span>
              <span>Backup</span>
            </div>
            <div v-if="item.freeDomain">
              <span class="font-weight-bold">Domain Gratis</span>
              <span>Selamanya</span>
            </div>
            <div v-if="item.sslUnlimited">
              <span class="font-weight-bold">Unlimited SSl</span>
              <span>Gratis Selamanya</span>
            </div>
            <div v-if="item.server">
              <span class="font-weight-bold">Private</span>
              <span>Name Server</span>
            </div>
            <div v-if="item.prioritas">
              <span class="font-weight-bold">Prioritas</span>
              <span>Layanan Support</span>
            </div>
            <img v-if="item.nama==='Bisnis'" src="../../assets/svg/star.svg" alt />
            <div v-if="item.protection">
              <span class="font-weight-bold">{{item.protection}}</span>
              <span>Mail Protection</span>
            </div>
            <div class="mt-5 mb-3">
              <button
                type="button"
                class="btn btn-outline-dark"
              >{{item.nama==='Bisnis'?'Diskon 40%':'Pilih Sekarang'}}</button>
            </div>
          </div>
        </div>
        <!-- Best Seller -->
        <div v-else class="custom-card-best">
          <div class="best-seller">
            <img src="../../assets/svg/best seller.svg" alt />
          </div>
          <div class="border pt-2 pb-2 blue">
            <h3 class="font-weight-bold white">{{item.nama}}</h3>
          </div>
          <div class="border pt-2 pb-2 blue">
            <p class="harga white">Rp. {{item.harga}}</p>
            <div class="row justify-content-center">
              <p class="mr-1 white">Rp</p>
              <h1
                class="font-weight-bold white"
              >{{item.hargaDisc.substring(0, item.hargaDisc.lastIndexOf('.'))}}</h1>
              <p
                class="font-weight-bold white"
              >{{item.hargaDisc.substring(item.hargaDisc.lastIndexOf('.'), item.hargaDisc.length)}}</p>
            </div>
          </div>
          <div class="border pt-2 pb-2 dark-blue">
            <span class="font-weight-bold white">{{item.user}}</span>
            <span class="white">Pengguna Terdaftar</span>
          </div>
          <div class="border pt-2 pb-2">
            <p class="font-weight-bold">{{item.resource}}X RESOURCE POWER</p>
            <div>
              <span class="font-weight-bold">{{item.space}}</span>
              <span>Disk Space</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.bandwidth}}</span>
              <span>Bandwidth</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.email}}</span>
              <span>POP3 Email</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.database}}</span>
              <span>Databases</span>
            </div>
            <div>
              <span class="font-weight-bold">{{item.addons}}</span>
              <span>Addon Domains</span>
            </div>
            <div v-if="item.backup !== 'Instant'">
              <span class="font-weight-bold">{{item.backup}}</span>
              <span>Backup & Restore</span>
            </div>
            <div v-else>
              <span class="font-weight-bold">{{item.backup}}</span>
              <span>Backup</span>
            </div>
            <div v-if="item.freeDomain">
              <span class="font-weight-bold">Domain Gratis</span>
              <span>Selamanya</span>
            </div>
            <div v-if="item.sslUnlimited">
              <span class="font-weight-bold">Unlimited SSl</span>
              <span>Gratis Selamanya</span>
            </div>
            <div v-if="item.server">
              <span class="font-weight-bold">Private</span>
              <span>Name Server</span>
            </div>
            <div v-if="item.prioritas">
              <span class="font-weight-bold">Prioritas</span>
              <span>Layanan Support</span>
            </div>
            <img v-if="item.nama==='Bisnis'" src="../../assets/svg/star.svg" alt />
            <div v-if="item.protection">
              <span class="font-weight-bold">{{item.protection}}</span>
              <span>Mail Protection</span>
            </div>
            <div class="mt-5 mb-3">
              <button type="button" class="btn btn-primary">Pilih Sekarang</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Package",
  mounted() {
    fetch("http://127.0.0.1:8000/api")
      .then(res => res.json())
      .then(data => {
        this.packages = data;
      })
      .catch(err => console.error(err));
  },
  data: () => {
    return {
      packages: []
    };
  }
};
</script>

<style scoped>
.custom-card {
  border: 0.1px solid rgb(223, 223, 223);
  padding: 0;
}

.custom-card-best {
  border: 1px solid #008fee;
  padding: 0;
}

.harga {
  text-decoration: line-through;
}

.border {
  border-bottom: 0.1px solid rgb(223, 223, 223);
}

.no-padding {
  padding: 0;
}

.blue {
  background-color: #008fee;
  border: none !important;
}

.white {
  color: white !important;
}

.dark-blue {
  background-color: #007fde;
  border: none !important;
}

.best-seller {
  position: absolute;
  left: -5px;
  top: -5px;
}
</style>