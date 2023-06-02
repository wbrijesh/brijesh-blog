<div class="lg:fixed">
  <div class="hidden lg:block">
    <div class="relative z-0">
      <div class="absolute top-0 left-0 w-[200px]"><slot /></div>
    </div>
  </div>

  <div class="pl-0 pt-0 block lg:hidden">
    <div class="block max-w-[38rem] mx-auto">
      <div class="block lg:hidden"><slot /></div>
    </div>
  </div>
</div>
