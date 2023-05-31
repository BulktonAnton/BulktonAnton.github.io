<script>
  import "prism-themes/themes/prism-one-dark.css";
</script>

<svelte:head>
  <link rel="stylesheet" href="/pico.min.css" />

  <style>
    nav {
      margin-left: 10%;
      margin-right: 10%;
    }
    .container-fluid {
   
    background-image: url(startsida.jpg);
    background-size: cover;
    background-position: center;

}


  </style>
</svelte:head>

<nav>
  <ul>
    <li><a href="/">Hem</a></li>
    <li><a href="/devblog">Blog</a></li>
  </ul>
</nav>

<main class="container-fluid">
  <hr />

    <slot />
</main>
