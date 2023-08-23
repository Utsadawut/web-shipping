<template>
  <div>
    <nav class="navbar navbar-expand-lg" style="background-color: #ffc107;">
  <div class="container-fluid">
    <a class="navbar-brand" ><i class="fas fa-book-reader me-2"></i>RURUShop</a>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <routerLink to="/" class="nav-link active" aria-current="page" href="#">หน้าแรก</routerLink>
        </li>
        <li class="nav-item">
          <routerLink to="/cart" class="nav-link active" aria-current="page" href="#">ตระกร้าสินค้า</routerLink>
        </li>
      </ul>
      <div class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="ค้นหาเลย.." aria-label="Search" v-model="product_store.input">
      </div>
    </div>
  </div>
</nav>
  </div>
</template>

<script setup>
import { useProductStore } from '../store/product'
const product_store = useProductStore()

</script>

<style lang="scss" scoped>

</style>
