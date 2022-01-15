<nav class="nav">
  <a href="/">
    <h1>Musify</h1>
  </a>
  <div class="menu">
    <span></span>
    <span></span>
    <span></span>
  </div>
</nav>

<style>
    .nav {
        @apply px-4 flex items-center justify-between h-16 bg-black z-10;
    }
    h1 {
        @apply font-bold text-lg text-white;
    }
    .menu {
      @apply flex flex-col items-center justify-between h-5 w-6;
    }
    span:nth-child(1),
    span:nth-child(3) {
      @apply w-6;
    }
    span {
      @apply rounded-md w-full h-1 bg-white;
    }
</style>