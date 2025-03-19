<template>
    <div class="mockup-phone">
      <canvas class="camera" />
      <div class="display">
        <header class="w-full flex justify-between items-center px-4 pt-4 mx-auto bg-primary text-white h-[70px]">
          <div class="text-sm rounded-lg border p-1">
            Lojão do Sport
          </div>

          <div tabindex="0" role="button" class="btn btn-ghost btn-circle">
            <svg xmlns="http://www.w3.org/2000/svg" 
              class="h-5 w-5" fill="none" viewBox="0 0 24 24" 
              stroke="currentColor"> <path stroke-linecap="round" 
              stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h7" 
            /> 
            </svg>
          </div>
        </header>

        <section class="artboard phone-1 m-4">  
          <div
            style="
              background-position: center;
              background-size: cover;
              background-image: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTgSDSmWz1TIsjRbuzCADL_f9OB17mm5EO5TQ&s);
            "
          >
            <div class="hero-content text-neutral-content text-center">
              <div class="max-w-md text-primary">
                <button class="btn btn-primary my-8">
                  % Descontos
                </button>
              </div>
            </div>
          </div>

          <div class="flex flex-col gap-2">
            <h3 class="text-xl font-semibold my-4">Produtos</h3>
          
            <div class="grid grid-cols-1 gap-2 lg:grid-cols-2">
              <div class="card bg-base-100 w-full shadow-sm">
                <figure>
                  <img
                    src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
                    alt="Shoes" />
                </figure>
                <div class="card-body">
                  <h2 class="card-title">Tênis Nike</h2>
                  <p>R$ 250,99</p>
                  <button class="btn btn-primary">Comprar</button>
                </div>
              </div>

              <div class="card bg-base-100 w-full shadow-sm">
                <figure>
                  <img
                    src="https://img.daisyui.com/images/stock/photo-1606107557195-0e29a4b5b4aa.webp"
                    alt="Shoes" />
                </figure>
                <div class="card-body">
                  <h2 class="card-title">Tênis Nike</h2>
                  <p>R$ 250,99</p>
                  <div class="card-actions justify-end">
                    <button class="btn btn-primary">Comprar</button>
                  </div>
                </div>
              </div>
            </div>

            <h3 class="text-xl font-semibold my-4">Novidades da empresa</h3>
          </div>
        </section>   
            
        <footer class="w-full bg-primary py-4 z-50">
          <div class="dock flex justify-between w-[70%] mx-auto text-white">
            <button class="flex items-center gap-2">
              <svg class="size-[1.1em]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><g fill="currentColor" stroke-linejoin="miter" stroke-linecap="butt"><polyline points="1 11 12 2 23 11" fill="none" stroke="currentColor" stroke-miterlimit="10" stroke-width="2"></polyline><path d="m5,13v7c0,1.105.895,2,2,2h10c1.105,0,2-.895,2-2v-7" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></path><line x1="12" y1="22" x2="12" y2="18" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></line></g></svg>
            </button>
            
            <button class="flex items-center gap-2">
              <svg class="size-[1.1em]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><g fill="currentColor" stroke-linejoin="miter" stroke-linecap="butt"><polyline points="3 14 9 14 9 17 15 17 15 14 21 14" fill="none" stroke="currentColor" stroke-miterlimit="10" stroke-width="2"></polyline><rect x="3" y="3" width="18" height="18" rx="2" ry="2" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></rect></g></svg>
            </button>
            
            <button class="flex items-center gap-2">
              <svg class="size-[1.1em]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><g fill="currentColor" stroke-linejoin="miter" stroke-linecap="butt"><circle cx="12" cy="12" r="3" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></circle><path d="m22,13.25v-2.5l-2.318-.966c-.167-.581-.395-1.135-.682-1.654l.954-2.318-1.768-1.768-2.318.954c-.518-.287-1.073-.515-1.654-.682l-.966-2.318h-2.5l-.966,2.318c-.581.167-1.135.395-1.654.682l-2.318-.954-1.768,1.768.954,2.318c-.287.518-.515,1.073-.682,1.654l-2.318.966v2.5l2.318.966c.167.581.395,1.135.682,1.654l-.954,2.318,1.768,1.768,2.318-.954c.518.287,1.073.515,1.654.682l.966,2.318h2.5l.966-2.318c.581-.167,1.135-.395,1.654-.682l2.318.954,1.768-1.768-.954-2.318c.287-.518.515-1.073.682-1.654l2.318-.966Z" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></path></g></svg>
            </button>
          </div>
        </footer>
      </div>
    </div>
</template>