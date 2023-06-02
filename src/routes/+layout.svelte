<script>
  import '../app.css';
  import Navigation from '../components/Navigation.svelte'
</script>

<div class="p-5">
  <div class="relative">
    <Navigation />
    <div class="py-10">
      <div class="block max-w-[38rem] mx-auto">
        <slot />
      </div>
    </div>
  </div>
</div>
