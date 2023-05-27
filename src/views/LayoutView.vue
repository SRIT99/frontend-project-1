<template>
    <div>
        <!-- header -->
        <header>
            <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">SR-IT</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#" @click=" $router.push({name: 'gallery'})">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" @click=" $router.push({name: 'gallery'})">Gallery</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" @click=" $router.push({name: 'contact'})">Contact US</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            others
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#" @click=" $router.push({name: 'about'})">About US</a></li>
            <li><a class="dropdown-item" href="#" @click=" $router.push({name: 'notice'})">Notices</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#" @click=" $router.push({name: 'programs'})">Our Programs</a></li>
          </ul>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
        </header>
        <!-- Main -->
        <main>
            <slot>

            </slot>
        </main>
        <!-- footer -->
        <footer></footer>
    </div>
</template>
<script>
export default{
    name:"LayoutView",
};

</script>