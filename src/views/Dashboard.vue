<template>
  <div class="dashboard">
    <sidebar />
    <div class="content p-5">
      <div class="search-container">
        <form class="d-flex" role="search">
          <input
            class="form-control me-2"
            type="search"
            placeholder="Search"
            aria-label="Search"
          />
          <button class="btn btn-outline-success" type="submit">Search</button>
        </form>
      </div>

      <div class="rekom fw-bold">Rekomendasi</div>
      <div class="row">
        <div class="col-3">
          <div class="container">
            <div class="card p-1" style="width: 12rem">
              <img src="aset/nasi-goreng.png" class="card-img-top" alt="..." />
              <div class="card-body">
                <h5 class="card-title">Nasi Goreng</h5>
              </div>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="container">
            <div class="card p-1" style="width: 12rem">
              <img src="aset/bakso.png" class="card-img-top" alt="..." />
              <div class="card-body">
                <h5 class="card-title">Bakso</h5>
              </div>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="container">
            <div class="card p-1" style="width: 12rem">
              <img src="aset/sate.png" class="card-img-top" alt="..." />
              <div class="card-body">
                <h5 class="card-title">Sate</h5>
              </div>
            </div>
          </div>
        </div>
        <div class="col-3">
          <div class="container">
            <div class="card p-1" style="width: 12rem">
              <img src="aset/rendang.png" class="card-img-top" alt="..." />
              <div class="card-body">
                <h5 class="card-title">Rendang</h5>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="rekom fw-bold">Popular food</div>
    </div>
  </div>
</template>

<script>
import sidebar from "@/components/sidebar.vue";

export default {
  name: "Dashboard",
  components: {
    sidebar,
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Alata&family=Molengo&display=swap");

.dashboard {
  display: grid;
  grid-template-columns: 1fr 5fr;
  background-color: #aa2b1d;
  height: 100vh;
  width: 100vw;
}

.content {
  background-color: #efeae5;
}

.search-container {
  width: 25rem;
}

.rekom {
  font-family: "Alata", sans-serif;
  color: black;
  font-size: 30px;
}

.card-title {
  font-family: "Molengo", sans-serif;
  font-size: 20px;
}

.card-body {
  padding: 0px !important;
}
</style>
