<script setup>
import SearchIcon from '../components/icons/IconSearch.vue'
import BookIcon from '../components/icons/IconBook.vue'

</script>

<template>
  <header>
    <img src="../assets/logo.jpeg" class="logo" alt="Logo">
    <h1 class="title">叶语花鸣</h1>
    <p class="title">LeafyLingo</p>
  </header>
  <var-row class="index-entrance">
    <var-col :span="12">
      <RouterLink to="/search" class="nav-link">
        <SearchIcon />
        <span class="label">识别</span>
      </RouterLink>
    </var-col>
    <var-col :span="12">
      <RouterLink to="/database" class="nav-link">
        <BookIcon />
        <span class="label">百科</span>
      </RouterLink>
    </var-col>
  </var-row>
</template>

<style>
header {
  padding-bottom: 20px;
  border-bottom: 1px solid #ddd;
  text-align: center;
}

.logo {
  vertical-align: middle;
  height: 80px;
  width: auto;
}

.title {
  text-align: center;
  margin: 0;
  color: #2E8540;
}

h1 {
  font-size: 40px;
  font-weight: bold;
}

.index-entrance {
  padding-top: 150px;
}

p.title {
  margin-top: -10px;
}

.nav-link {
  display: inline-block;
  vertical-align: top;
  text-decoration: none;
  color: #333;
  font-size: 16px;
  margin: 0 50px;
  text-align: center;
}

.label {
  display: block;
  text-align: center;
  margin-top: 5px;
  font-size: large;
  font-weight: bold;
}

svg {
  width: 50px;
  height: auto;
}
</style>