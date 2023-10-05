<script>
  import Navbar from "$lib/components/Navbar.svelte";
  import ProyectsSection from "$lib/components/ProyectsSection.svelte";
  
</script>


<section class="bg-gray-300 min-h-screen">
  <Navbar />
  <div>
    <h1 class="text-center mt-4 text-3xl md:text-5xl lg:text-[65px] max-w-[900px] mx-auto text-white">Impulsando Negocios a través de <span class="text-blue-600">Innovaciones Tecnológicas.</span></h1>
    <p class="max-w-[1000px] mx-auto text-gray-200 text-center mt-6 text-sm p-2 md:p-0">En TOB Group Solutions, nuestra misión es conectar el mundo real y digital, ofreciendo soluciones innovadoras que impulsan la transformación y crecimiento sostenible de nuestros clientes.</p>
  </div>
  <div class="flex justify-center flex-col md:flex-row items-center gap-5 mt-5 md:mt-14">
    <a href="/" class="bg-blue-900 py-2 px-3 border transition-colors border-white rounded-lg text-white font-medium hover:bg-blue-800 w-48 text-center">Nuestros Productos</a>
    <a href="/" class="bg-blue-900 border transition-colors border-white py-2 px-3 rounded-lg text-white font-medium hover:bg-blue-800 w-48 text-center">Contactate</a>
  </div>
  <hr class="max-w-[1000px] mx-2 md:mx-auto mt-5 md:mt-24 border-0.1 border-gray-200 opacity-30" />
  <div class="max-w-[1000px] mx-2 md:mx-auto mt-4 grid grid-cols-1 md:grid-cols-3 gap-5">
    <div class="md:border-r border-white border-opacity-40">
      <h2 class="uppercase font-medium text-white opacity-80">
        Desarrollo de Software
      </h2>
      <p class="text-white font-light opacity-80">Impulsamos la transformación y crecimiento sostenible de nuestros clientes.</p>
    </div>
    <div class="md:border-r border-white border-opacity-40">
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
  <hr class="max-w-[1000px]  md:mx-auto mt-5 border-0.1 border-gray-200 opacity-30" />
</section>

<ProyectsSection />

<style>
  section {
    background: rgb(5,2,45);
    background: linear-gradient(175deg, rgba(5,2,45,1) 0%, rgba(20,20,91,1) 47%, rgba(25,123,143,1) 100%);
  }
</style>