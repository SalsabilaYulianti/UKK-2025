<template>
  <div class="container">
    <nav class="navbar">
      <h3>
        JUMLAH SELURUH
      </h3>
    </nav>
    <div class="jurusan m-5  "> 
      <div class="row jumlah">
        <div class="card m-5 guru" style="width: 30rem;">
        <div class="card-body text1">
          <h4 class="card-title">GURU LAKI-LAKI</h4>
          <h5 class="mb-4">82 orang</h5>
        </div>
      </div>
      <div class="card m-5 guru" style="width: 30rem;">
          <div class="card-body text1">
            <h4 class="card-title">GURU PEREMPUAN</h4>
            <h5 class="mb-4">25 orang</h5>
          </div>
      </div>
    </div>
      <div class="row jumlah1 ">
        <div class="card m-5 siswa" style="width: 30rem;">
            <div class="card-body text1">
              <h4 class="card-title">SELURUH JUMLAH SISWA</h4>
              <h5 class="mb-4">1500 orang</h5>
            </div>
        </div>
      </div>
    </div>

  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Inria+Serif:ital,wght@0,300;0,400;0,700;1,300;1,400;1,700&display=swap');

.container {
  height: 100vh;
  width: 100%;
}

.navbar {
font-family: "Inria Serif", serif;
font-weight: 500;
font-style: normal;
margin: 0px;
background-color:#211C63;
color: floralwhite;
padding: 1em;
justify-content: center ;
font-size: 20px;
}

h4, h5{
  font-family: "Inria Serif", serif;
  font-weight: 500;
  font-style: normal;
  margin: 0px;
  color:black
}
.jumlah, .jumlah1{
  justify-content: center;
}

.siswa, .guru{
  border: 2px solid #211C63;
}

.text1{
  text-align: center;
}

</style>