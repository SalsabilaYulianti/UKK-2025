<script setup>

const kata = "SELAMAT DATANG di SMK NEGARI 4 TASIKMALAYA";
const nama = ref('');
const email = ref('');
const pesan = ref('');

function kirim(event) {
  event.preventDefault(); // Mencegah form submit

  // Percabangan untuk memeriksa apakah semua field sudah diisi
  if (nama.value === '' || email.value === '' || pesan.value === '') {
    alert('Harap isi semua field!');
  } else {
    alert(`${kata}\nNama: ${nama.value}\nEmail: ${email.value}\nPesan: ${pesan.value}`);
  }
}
</script>

<template>
  <div class="container">
    <form @submit="kirim">
      <div class="form-group mt-5">
        <label for="exampleInputName"><h5>Nama</h5></label>
        <input v-model="nama" type="text" class="form-control rounded-3 mt-2" placeholder="Masukkan Nama" />
      </div>
      <div class="form-group mt-3">
        <label for="exampleInputEmail"><h5>Email</h5></label>
        <input v-model="email" type="email" class="form-control rounded-3 mt-2" placeholder="Masukkan Email" />
      </div>
      <div class="form-group mt-3">
        <label for="exampleInputMessage" ><h5>Pesan</h5></label>
        <input v-model="pesan" type="text" class="form-control rounded-3 mt-2 pesan" placeholder="Masukkan Pesan" />
      </div>
      <button type="submit" class="btn btn-primary mt-3">Kirim</button>
    </form>
  </div>
</template>


<style scoped>
.container {
  height: 100vh;
  width: 100%;
}

.pesan{
  height: 100px;
}


</style>