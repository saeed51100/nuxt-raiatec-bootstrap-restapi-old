<script lang="ts" setup></script>
<template>
  <nav class="navbar navbar-expand-lg bg-info">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Navbar</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" aria-current="page" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Features</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pricing</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              Dropdown link
            </a>
            <ul class="dropdown-menu">
              <li><a class="dropdown-item" href="#">Action</a></li>
              <li><a class="dropdown-item" href="#">Another action</a></li>
              <li><a class="dropdown-item" href="#">Something else here</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <nav class="bg-gray-900 text-white py-5 border-b border-gray-700">
    <div
        class="container flex flex-col sm:flex-row justify-center gap-3 sm:gap-0 sm:justify-between items-center"
    >
      <NuxtLink to="/" class="text-2xl font-medium">Elon's Blog</NuxtLink>
      <ul class="nav">
        <li>
          <NuxtLink to="/">Home</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/categories">Categories</NuxtLink>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style>
ul.nav {
  @apply flex gap-5 items-center justify-end;
}
ul.nav > li > a {
  @apply text-gray-300 hover:text-gray-50;
}
/*ul.nav > li > a.router-link-active {*/
/*  @apply text-primary-400;*/
/*}*/
</style>
