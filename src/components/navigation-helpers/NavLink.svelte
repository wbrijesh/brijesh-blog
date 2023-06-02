<script>
  export let active = false;
  export let external = false;
  export let href = '';
  export let label = '';

  // let linkClass =
  //   'text-[16px] ' + active
  //     ? 'text-orange-600 font-medium '
  //     : 'text-gray-500 hover:text-orange-600 transition ' + external
  //     ? 'flex items-center gap-2 mr-4 '
  //     : 'block ';
</script>

<a
  class="text-[16px] {active
    ? 'text-orange-600 font-medium'
    : 'text-gray-500 hover:text-orange-600 transition'} {external
    ? 'flex items-center gap-2 mr-4'
    : 'block'}"
  {href}
  target="_blank"
>
  {#if external}
    <svg
      xmlns="http://www.w3.org/2000/svg"
      width="16"
      height="16"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      strokeWidth="2"
      strokeLinecap="round"
      strokeLinejoin="round"
      class="feather feather-external-link"
    >
      <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6" />
      <polyline points="15 3 21 3 21 9" />
      <line x1="10" y1="14" x2="21" y2="3" />
    </svg>
  {/if}
  <p>{label}</p>
</a>
