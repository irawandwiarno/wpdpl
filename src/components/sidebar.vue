<template>
  <div class="sidebar">
    <div class="title">
      <img src="aset/vector.png" alt="" />
    </div>
    <div class="item-link">
      <router-link to="/" active-class="active">
        <div class="link-container my-3 px-4">Home</div>
      </router-link>
    </div>
    <div class="link-container my-3">
      <div class="item-link">
        <div class="dropdown">
          <button
            class="btn btn-darkred dropdown-toggle"
            type="button"
            data-bs-toggle="dropdown"
            aria-expanded="false"
          >
            Choose Island
          </button>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Jawa</a></li>
            <li><a class="dropdown-item" href="#">Sumatra</a></li>
            <li><a class="dropdown-item" href="#">Sulawesi</a></li>
            <li><a class="dropdown-item" href="#">Kalimantan</a></li>
            <li><a class="dropdown-item" href="#">Bali</a></li>
            <li><a class="dropdown-item" href="#">Papua</a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Alata&display=swap");

.sidebar {
  padding: 10px;
  align-items: left !important;
  color: white;
}

.title {
  margin-bottom: 50px;
}

.link-container {
  font-family: "Alata", sans-serif;
  background-color: #952114;
  color: white;
  padding: 10px;
  border-radius: 8px;
}
.link-container:link {
  text-decoration: none;
}

.btn-darkred {
  background-color: #952114 !important;
  color: white;
}

.dropdown-menu{
    background-color: #9A2C1F;
}

.dropdown-item{
    color: white !important;
}
</style>