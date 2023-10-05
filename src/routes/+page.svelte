<script>
  import Navbar from "$lib/components/Navbar.svelte";
  
</script>


<section class="bg-gray-300 h-screen">
  <Navbar />
  <div>
    <h1 class="text-center text-[65px] max-w-[900px] mx-auto text-white">Impulsando Negocios a través de <span class="text-blue-600">Innovaciones Tecnológicas.</span></h1>
    <p class="max-w-[1000px] mx-auto text-gray-200 text-center mt-6">En TOB Group Solutions, nuestra misión es conectar el mundo real y digital, ofreciendo soluciones innovadoras que impulsan la transformación y crecimiento sostenible de nuestros clientes.</p>
  </div>
  <div class="flex justify-center gap-5 mt-5">
    <a href="/" class="bg-blue-900 py-2 px-3 border transition-colors border-white rounded-lg text-white font-medium hover:bg-blue-800">Nuestros Productos</a>
    <a href="/" class="bg-blue-900 border transition-colors border-white py-2 px-3 rounded-lg text-white font-medium hover:bg-blue-800">Contactate</a>
  </div>
  <hr class="max-w-[1000px] mx-auto mt-28 border-0.1 border-gray-200 opacity-30" />
  <div class="max-w-[1000px] mx-auto mt-4 grid grid-cols-3 gap-5">
    <div class="border-r border-white border-opacity-40">
      <h2 class="uppercase font-medium text-white opacity-80">
        Desarrollo de Software
      </h2>
      <p class="text-white font-light opacity-80">Impulsamos la transformación y crecimiento sostenible de nuestros clientes.</p>
    </div>
    <div class="border-r border-white border-opacity-40">
      <h2 class="uppercase font-medium text-white opacity-80">
        Desarrollo de Blockhain
      </h2>
      <p class="text-white font-light opacity-80">Ayudamos en la integración al ecosistema Blockchain.</p>
    </div>
    <div>
      <h2 class="uppercase font-medium text-white opacity-80">
        Consultoría IT
      </h2>
      <p class="text-white font-light opacity-80">Digitaliza tu empresa con nosotros. Garantizamos seguridad y optimización.</p>
    </div>
  </div>
  <hr class="max-w-[1000px] mx-auto mt-5 border-0.1 border-gray-200 opacity-30" />
</section>

<style>
  section {
    background: rgb(5,2,45);
    background: linear-gradient(175deg, rgba(5,2,45,1) 0%, rgba(20,20,91,1) 47%, rgba(25,123,143,1) 100%);
  }
</style>