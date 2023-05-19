<script>
//Definiamo il nome del componente ed eventualmente i componenti che usa (nessuno)
export default {
  name: "AppHeader",
};
</script>

<template>
  <header class="w-100">
    <div class="container">
      <div class="d-flex justify-content-between p-2 align-items-center">
        <div>
          <img src="/public/dc-logo.png" alt="">
        </div>
        <div>
          <ul class="nav justify-content-end">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#">Active</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Link</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </header>
</template>
