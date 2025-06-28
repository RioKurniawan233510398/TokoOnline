<template>
  <div class="cards">
    <div class="card" v-for="i in 6" :key="i">
      <img src="https://via.placeholder.com/250x150" alt="Produk" />
      <h3>Produk {{ i }}</h3>
      <p>Rp {{ i * 15000 }}</p>
      <button @click="handleBuy(i)">Beli Sekarang</button>
    </div>
  </div>
</template>

<script setup>
function handleBuy(i) {
  alert(`Produk ${i} ditambahkan ke keranjang!`);
}
</script>
