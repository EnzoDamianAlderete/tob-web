<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  import { Button, Dropdown, DropdownItem } from 'flowbite-svelte';
  import { ChevronDownSolid } from 'flowbite-svelte-icons';
</script>

<Navbar let:hidden let:toggle class=" py-6 bg-transparent h-1/5">
  <NavBrand href="/">
    <h1 class="text-white text-2xl font-bold">TOB Group Solutions</h1>
    <!-- <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">Flowbite</span> -->
  </NavBrand>
  <NavHamburger on:click={toggle} menuClass="text-white" />
  <NavUl {hidden}>
    <NavLi on:click={toggle} class="lg:text-white text-md uppercase font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/">Inicio</NavLi>
    <NavLi on:click={toggle} class="lg:text-white text-md uppercase font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/products">Productos</NavLi>
    <NavLi on:click={toggle} class="lg:text-white text-md uppercase font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/cotizador">TOB Labs</NavLi>
    <NavLi on:click={toggle} class="lg:text-white text-md uppercase font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/clientes">Clientes</NavLi>
    <NavLi on:click={toggle} class="lg:text-white text-md uppercase font-medium" nonActiveClass="hover:text-basa-gold transition-colors" href="/comisiones">Contacto</NavLi>
    <button class="text-white flex items-center uppercase">Idioma<ChevronDownSolid class="w-3 h-3 ml-2 text-white dark:text-white"/></button>
    <Dropdown>
      <DropdownItem class="flex gap-2 items-center hover:bg-gray-200 transition-colors">
        <img src="/es.png" alt="Bandera de Español" class="w-5"/>
        Español
      </DropdownItem>
      <DropdownItem class="flex gap-2 items-center hover:bg-gray-200 transition-colors">
        <img src="/en.png" alt="Bandera de Español" class="w-5"/>
        Inglés
        </DropdownItem>
      <DropdownItem class="flex gap-2 items-center hover:bg-gray-200 transition-colors">
        <img src="/fr.png" alt="Bandera de Español" class="w-5"/>
        Frances
      </DropdownItem>
    </Dropdown>
    <!-- <NavLi class="text-basa-blue text-md uppercase" nonActiveClass="hover:text-basa-gold transition-colors" href="/products">Otros</NavLi> -->
  </NavUl>
</Navbar>