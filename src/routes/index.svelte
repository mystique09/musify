<div class="hero">
    <div class="circle circle-1"></div>
    <div class="header">
      <h2>Listening is everything</h2>
    </div>
    <div class="para">
      Millions of songs and podcasts. No credit card needed.
    </div>
    <div class="btn-container">
      <a href="/signup">Get Musify free</a>
    </div>
    <div class="circle circle-2"></div>
</div>

<style>
  .hero {
    @apply flex items-center justify-center flex-col h-screen relative p-8 text-center bg-blue-800 overflow-hidden;
  }
  
  .header {
    @apply mb-4;
  }
  
  h2 {
    @apply font-bold text-5xl;
  }
  
  h2, .para {
    @apply text-green-400;
  }
  
  .btn-container {
    @apply mt-6 p-6;
  }
  
  a {
    @apply rounded-full bg-green-400 px-8 py-4 uppercase text-sm font-bold text-blue-800;
  }
  
  .circle {
    @apply absolute h-64 w-64 rounded-full bg-green-400;
  }
  
  .circle-1 {
    @apply -top-24 -right-32;
  }
  
  .circle-2 {
    @apply -bottom-24 -left-24 h-72 w-72;
  }
</style>