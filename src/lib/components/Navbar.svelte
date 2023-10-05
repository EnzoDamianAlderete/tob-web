<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
</script>

<Navbar let:hidden let:toggle class=" py-6 bg-transparent">
  <NavBrand href="/">
    <h1>TOB Group Solutions</h1>
    <!-- <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Flowbite</span> -->
  </NavBrand>
  <NavHamburger on:click={toggle} menuClass="text-gray-700" />
  <NavUl {hidden} ulClass="dark:bg-gray-100 dark:border-none" nonActiveClass="text-gray-700 dark:bg-gray-100 hover:bg-gray-100 md:hover:bg-transparent md:border-0 md:hover:text-primary-700">
    <NavLi on:click={toggle} class="text-basa-blue text-md uppercase lg:hidden font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/">Inicio</NavLi>
    <NavLi on:click={toggle} class="text-basa-blue text-md uppercase lg:hidden font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/products">Productos</NavLi>
    <NavLi on:click={toggle} class="text-basa-blue text-md uppercase lg:hidden font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/cotizador">Cotizador</NavLi>
    <NavLi on:click={toggle} class="text-basa-blue text-md uppercase lg:hidden font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/clientes">Clientes</NavLi>
    <NavLi on:click={toggle} class="text-basa-blue text-md uppercase lg:hidden font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/comisiones">Comisiones</NavLi>
    <!-- <NavLi class="text-basa-blue text-md uppercase" nonActiveClass="hover:text-basa-gold transition-colors" href="/products">Otros</NavLi> -->
  </NavUl>
</Navbar>