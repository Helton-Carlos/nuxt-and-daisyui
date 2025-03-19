<template>
    <div class="mockup-phone">
      <canvas class="camera" />
      <div class="display">
        <header class="w-full flex justify-between items-center px-4 pt-4 mx-auto bg-green-700 text-white h-[70px]">
          <div class="text-base font-semibold border-t-2">
            Agro-Técnico 
          </div>

          <div tabindex="0" role="button" class="btn btn-ghost btn-circle">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor"> <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h7" /> </svg>
          </div>
        </header>

        <section class="artboard phone-1 m-4">  
          <fieldset class="fieldset mb-4">
            <legend class="fieldset-legend">Pesquisar</legend>
            <input class="input w-full" type="text" placeholder="Digite produtos" />
          </fieldset>

          <div class="card bg-base-100 card-xs shadow-sm">
            <div class="card-body">
              <h2 class="card-title">Noticias da semana</h2>
              <p>Biosseguridade na bovinocultura leiteira: qual a sua importância?</p>
              <div class="justify-end card-actions">
                <button class="btn bg-green-700 text-white">Veja mais</button>
              </div>
            </div>
          </div>

          <div class="stat">
            <div class="stat-title">Produção Mensal</div>
            <div class="stat-value">89,400</div>
            <div class="stat-desc">21% a mais que mês passado</div>
          </div>

          <div class="stat">
            <div class="stat-title">Meta Mensal</div>
            <div class="stat-value text-red-700">4,200</div>
            <div class="stat-desc text-red-700">↗︎ 40 (2%)</div>
          </div>

          <fieldset class="fieldset p-2 mt-2 bg-base-100 border border-base-300 rounded-box w-64">
            <label class="fieldset-label flex items-center gap-2">
              <input type="checkbox" class="toggle" />
              Ativar Status
            </label>
          </fieldset>
        </section>   
            
        <footer class="w-full bg-green-700 py-4">
          <div class="dock flex justify-between w-[80%] mx-auto text-white">
            <button class="flex items-center gap-2">
              <svg class="size-[1.1em]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><g fill="currentColor" stroke-linejoin="miter" stroke-linecap="butt"><polyline points="1 11 12 2 23 11" fill="none" stroke="currentColor" stroke-miterlimit="10" stroke-width="2"></polyline><path d="m5,13v7c0,1.105.895,2,2,2h10c1.105,0,2-.895,2-2v-7" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></path><line x1="12" y1="22" x2="12" y2="18" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></line></g></svg>
              <span class="dock-label">Home</span>
            </button>
            
            <button class="flex items-center gap-2">
              <svg class="size-[1.1em]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><g fill="currentColor" stroke-linejoin="miter" stroke-linecap="butt"><polyline points="3 14 9 14 9 17 15 17 15 14 21 14" fill="none" stroke="currentColor" stroke-miterlimit="10" stroke-width="2"></polyline><rect x="3" y="3" width="18" height="18" rx="2" ry="2" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></rect></g></svg>
              <span class="dock-label">Notificação</span>
            </button>
            
            <button class="flex items-center gap-2">
              <svg class="size-[1.1em]" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><g fill="currentColor" stroke-linejoin="miter" stroke-linecap="butt"><circle cx="12" cy="12" r="3" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></circle><path d="m22,13.25v-2.5l-2.318-.966c-.167-.581-.395-1.135-.682-1.654l.954-2.318-1.768-1.768-2.318.954c-.518-.287-1.073-.515-1.654-.682l-.966-2.318h-2.5l-.966,2.318c-.581.167-1.135.395-1.654.682l-2.318-.954-1.768,1.768.954,2.318c-.287.518-.515,1.073-.682,1.654l-2.318.966v2.5l2.318.966c.167.581.395,1.135.682,1.654l-.954,2.318,1.768,1.768,2.318-.954c.518.287,1.073.515,1.654.682l.966,2.318h2.5l.966-2.318c.581-.167,1.135-.395,1.654-.682l2.318.954,1.768-1.768-.954-2.318c.287-.518.515-1.073.682-1.654l2.318-.966Z" fill="none" stroke="currentColor" stroke-linecap="square" stroke-miterlimit="10" stroke-width="2"></path></g></svg>
              <span class="dock-label">Config</span>
            </button>
          </div>
        </footer>
      </div>
    </div>
</template>