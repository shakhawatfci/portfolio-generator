<script>
import { fade, fly } from 'svelte/transition';
import { onMount } from 'svelte';
let isVisiable = false;

onMount(() => {
	isVisiable = true;
})

// $: setInterval(function(){  isVisiable = !isVisiable }, 4000);

</script>


	<div class="row hero-area">
		<div class="col-md-8 mx-auto">
        
        <h1 class="hero-title" > 	
	    <span>|</span>	
	    {#if isVisiable}
	    <span in:fly="{{y: -20, duration: 800}}">
	    {#each 'Shakhawat Hossain' as char, i}
			<span
				in:fade="{{delay: 1000 + i * 150, duration: 700}}"
			>{char}</span>
		{/each}
	    </span>
	     {/if}
		 </h1>
       

			<p class="hero-paragraph">
                Computer Science Graduate, Software Engineer , Open Source Contributor , Envato Author
			</p>

            <ul class="social-network social-circle">
                <li><a  target="_blank"   href="https://github.com/shakhawatfci" class="icoRss" title="Rss"><i class="fa fa-github"></i></a></li>
                <li><a  target="_blank"   href="https://facebook.com/snsabbir.fci" class="icoFacebook" title="Facebook"><i class="fa fa-facebook"></i></a></li>
                <li><a  target="_blank"  href="https://twitter.com/shakhawat_fci" class="icoTwitter" title="Twitter"><i class="fa fa-twitter"></i></a></li>
                <li><a    href="mailto:94shakha.18@gmail.com" class="icoGoogle" title="Google +"><i class="fa fa-envelope"></i></a></li>
                <li><a  target="_blank"  href="https://www.linkedin.com/in/shakhawat-hossain-a2206b116/" class="icoLinkedin" title="Linkedin"><i class="fa fa-linkedin"></i></a></li>
            </ul>	
		</div>
	</div>