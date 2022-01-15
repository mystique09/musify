<script>
  import Navigator from "$lib/components/Navigator.svelte";
</script>

<footer>
  <div class="container">
    <div class="branding-logo">
      <a href="/">
        <h3>Musify</h3>
      </a>
    </div>
    <div class="navigators">
      <Navigator url="/" heading="Company" list={['About', 'Jobs', 'For The Record']} />
      <Navigator url="/" heading="Community" list={['For Artist', 'Developers', 'Advertising', 'Inventors', 'Vendors']} />
      <Navigator url="/" heading="Useful Links" list={['Support', 'Web Player', 'Mobile App']} />
    </div>
    <div class="visit-my-github-and-others">
      <div class="link">
        <a href="/">
          <span>Github</span>
        </a>
        </div>
      <div class="link">
        <a href="/">
          <span>LinkedIn</span>
        </a>
      </div>
      <div class="link">
        <a href="/">
          <span>Facebook</span>
        </a>
      </div>
    </div>
  </div>
</footer>

<style>
  footer {
    @apply bg-black;
  }
  .container {
    @apply px-4 py-6 flex flex-col justify-between;
  }
  .branding-logo {
    @apply mt-4 flex items-start text-white;
  }
  .branding-logo h3 {
    @apply text-xl font-bold;
  }
  .navigators {
    @apply mt-8 flex flex-col items-start justify-between;
  }
  .visit-my-github-and-others {
    @apply flex flex-row h-24 items-end;
  }
  .link {
    @apply text-white mr-4;
  }
</style>