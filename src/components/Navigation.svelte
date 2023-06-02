<script>
  import NavContainer from './navigation-helpers/NavContainer.svelte';
  import NavSection from './navigation-helpers/NavSection.svelte';
  import NavSectionTitle from './navigation-helpers/NavSectionTitle.svelte';
  import NavLink from './navigation-helpers/NavLink.svelte';
</script>

<div>
  <NavContainer>
    <NavSection>
      <NavLink active href="https://brijesh.blog" label="Brijesh's Blog" />
    </NavSection>

    <NavSection>
      <NavSectionTitle label="External links" />
      <NavLink href="#" label="Github" external />
      <NavLink href="#" label="Linkedin" external />
      <NavLink
        href="https://www.goodreads.com/user/show/162236489-brijesh-wawdhane"
        label="Goodreads"
        external
      />
    </NavSection>
  </NavContainer>
</div>
