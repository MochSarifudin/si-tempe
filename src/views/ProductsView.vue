<template>
  <main class="px-12 flex flex-col gap-x-28">
    <h2 class="mb-4 text-xl font-bold">TEMPE BIASA</h2>
    <div class="flex justify-between">
      <div v-for="(tempe, i) in tempeBiasa" :key="i">
        <router-link :to="`/products/${tempe.slug}.${i}`" >
          <img :src="tempe.gambar" width="360" />
          <span class="text-lg font-bold">{{ tempe.harga }}</span>
        </router-link>    
      </div>
    </div>
    <h2 class="my-4 text-xl font-bold">TEMPE KAPUK</h2>
    <div class="flex justify-between">
      <div v-for="(tempe, i) in tempeKapuk" :key="i">
        <img :src="tempe.gambar" width="360" />
        <span class="text-lg font-bold">{{ tempe.harga }}</span>
      </div>
    </div>
    <h2 class="my-4 text-xl font-bold">TEMPE MENJES</h2>
    <div class="flex justify-between">
      <div v-for="(tempe, i) in tempeMenjes" :key="i">
        <img :src="tempe.gambar" width="360" />
        <span class="text-lg font-bold">{{ tempe.harga }}</span>
      </div>
    </div>
  </main>
</template>

<script setup>
const tempeBiasa = [
  {
    slug: 'tempe-biasa',
    deskripsi: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
    gambar: "/tempe1.jpg",
    harga: 'RP. 3000 (TERSEDIA)'
  },
  {
    slug: 'tempe-biasa',
    deskripsi: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
    gambar: "/tempe1.jpg",
    harga: 'RP. 5000 (TERSEDIA)'
  },
  {
    slug: 'tempe-biasa',
    deskripsi: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
    gambar: "/tempe1.jpg",
    harga: 'RP. 10000 (TERSEDIA)'
  }
]

const tempeKapuk = [
  {
    gambar: "/tempe2.jpg",
    harga: 'RP. 3000 (TERSEDIA)'
  },
  {
    gambar: "/tempe2.jpg",
    harga: 'RP. 5000 (TERSEDIA)'
  },
  {
    gambar: "/tempe2.jpg",
    harga: 'RP. 10000 (TERSEDIA)'
  }
]

const tempeMenjes = [
  {
    gambar: "/tempe3.jpg",
    harga: 'RP. 3000 (HABIS)'
  },
  {
    gambar: "/tempe3.jpg",
    harga: 'RP. 5000 (HABIS)'
  },
  {
    gambar: "/tempe3.jpg",
    harga: 'RP. 10000 (HABIS)'
  }
]
</script>
