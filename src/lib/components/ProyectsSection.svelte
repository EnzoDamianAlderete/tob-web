<script>
    

  let productos = [
      {
          id:1,
          title:"BeChain Core®",
          text:"Consiste en una API rest a través de la cual cualquier empresa u organización puede subir documentos o datos y certificarlos a través de nuestra plataforma en forma rápida y sencilla.",
          url:"https://bechain.io/",
          img:"https://www.tob-group-solutions.com/assets/bechain-core-c7709ac3.png"
      },
      {
          id:2,
          title:"BeChain Tracking®",
          text:"Permite comprobar la trazabilidad de la información en forma inviolable. En el hash es donde encontramos la verdadera clave del proceso de trazabilidad. Ese hash se cuelga a la Blockchain a través de una transacción que quedará registrada eternamente en todos los nodos de la red.",
          url:"https://bechain.io/",
          img:"https://www.tob-group-solutions.com/assets/bechain%20tracking-efe2b38d.png"
      },
      {
          id:3,
          title:"Génesis®",
          text:"Nuestro sistema web de gestión B2B GENESIS es una solución integral para simplificar la administración financiera y operativa de empresas en el mundo de las criptomonedas. Con herramientas para un registro de transacciones, automatización contable y control de operaciones, brinda flexibilidad y control.",
          url:"https://bechain.io/",
          img:"https://www.tob-group-solutions.com/assets/genesis-b6a985eb.png"
      },
      {
          id:4,
          title:"Token Estate®",
          text:"Una solución innovadora de tokenización de activos que permite digitalizar activos inmuebles (Real World Asset Tokenization). Proporciona una infraestructura digital segura para representar activos con tokens digitales, lo que facilita su posesión, transferencia y verificación. Al unir el mundo real con el digital, crea un ecosistema transparente y abre nuevas oportunidades de inversión.",
          url:"https://bechain.io/",
          img:"https://www.tob-group-solutions.com/assets/token%20esatate-dddd26c3.png"
      },
      {
          id:5,
          title:"LÍA, tu asistente virtual",
          text:"LIA, nuestro chatbot basado en inteligencia artificial, ofrece asistencia y orientación en tareas cotidianas a través de la plataforma de mensajería de WhatsApp. Desde la gestión de citas y reuniones hasta la transcripción de audios y resolución de imprevistos, está diseñado para ser tu asistente personal.",
          url:"https://bechain.io/",
          img:"/lia.webp"
      },
  ]

</script>

<section class="my-8 mx-auto max-w-[1100px] grid-cols-1 md:grid-cols-3">
  <h2 class="text-3xl text-blue-500 text-center font-bold p-4">Nuestros Productos</h2>
  <div class="flex justify-center align-middle items-center gap-4 text-center flex-wrap">
      {#each productos as producto(producto.id)}
      <div class="card-container">
          <a href={producto.url} target="_blank">
              <div class="card">
                  <div class="front-content flex flex-col">
                  <p>{producto.title}</p>
                  <img src={producto.img} alt="">
                  </div>
                  <div class="content">
                  <p class="heading">{producto.title}</p>
                  <p>
                  {producto.text}
                  </p>
                  </div>
              </div>
          </a>
        </div>
       {/each} 
  </div>
</section>

<style>
  
.card-container {
width: 350px;
height: 400px;
position: relative;
border-radius: 10px;
box-shadow: 0 10px 20px rgba(0, 0, 0, 0.2);
overflow: hidden;
}

.card {
width: 100%;
height: 100%;
border-radius: inherit;
}

.card .front-content {
width: 100%;
height: 100%;
display: flex;
align-items: center;
justify-content: center;
transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1)
}

.card .front-content p {
font-size: 32px;
font-weight: 700;
opacity: 1;
background: linear-gradient(-45deg, #11b1da 0%, #072f6b 100% );
background-clip: text;
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1)
}

.card .content {
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
display: flex;
flex-direction: column;
align-items: center;
justify-content: center;
text-align: center;
gap: 10px;
background: linear-gradient(-45deg, #1b94b3 0%, #072f6b 100% );
color: #e8e8e8;
padding: 20px;
line-height: 1.5;
border-radius: 5px;
pointer-events: none;
transform: translateY(96%);
transition: all 0.6s cubic-bezier(0.23, 1, 0.320, 1);
}

.card .content .heading {
font-size: 32px;
font-weight: 700;
}

.card:hover .content {
transform: translateY(0);
}

.card:hover .front-content {
transform: translateY(-30%);
}

.card:hover .front-content p {
opacity: 0;
}


</style>