<template>
  <nav class="navbar navbar-expand-md bg-dark navbar-dark">
    <!-- Brand -->
    <NuxtLink class="navbar-brand" to="/">
      Books Trader
    </NuxtLink>

    <!-- Toggler/collapsibe Button -->
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
      <span class="navbar-toggler-icon" />
    </button>

    <!-- Navbar links -->
    <div id="collapsibleNavbar" class="collapse navbar-collapse">
      <ul class="navbar-nav">
        <li class="nav-item">
          <NuxtLink to="/products" class="nav-link">
            Products <span class="sr-only">(current)</span>
          </NuxtLink>
        </li>
        <li class="nav-item">
          <NuxtLink to="/my-items" class="nav-link">
            My Items <span class="sr-only">(current)</span>
          </NuxtLink>
        </li>
      </ul>
    </div>
  </nav>
</template>
