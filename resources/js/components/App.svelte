  <script>
  import {fly} from 'svelte/transition';
    document.addEventListener('DOMContentLoaded', function() {
		var elems = document.querySelectorAll('.collapsible');
		var instances = M.Collapsible.init(elems, {acordeon : true});
 	});
	 
	let mostrar = true; 
	 
  </script>

<div class="container">

  <form action="#">
    <p>
      <label>
        <input type="checkbox" bind:checked={mostrar}/>
        <span>Mostrar</span>
      </label>
    </p>
  </form></div>
{#if mostrar}
	<div class="container" transition:fly="{{ x: -200, duration: 2000 }}">
	<ul class="collapsible">
		<li>
		<div class="collapsible-header">Primero</div>
		<div class="collapsible-body"><span>Lorem ipsum dolor sit amet.</span></div>
		</li>
		<li>
		<div class="collapsible-header">Segundo</div>
		<div class="collapsible-body"><span>Lorem ipsum dolor sit amet.</span></div>
		</li>
		<li>
		<div class="collapsible-header">Tercero</div>
		<div class="collapsible-body"><span>Lorem ipsum dolor sit amet.</span></div>
		</li>
	</ul>
	</div>
{/if}

