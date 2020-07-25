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
	    {#each 'ARIFUZZAMAN' as char, i}
			<span
				in:fade="{{delay: 1000 + i * 150, duration: 700}}"
			>{char}</span>
		{/each}
	    </span>
	     {/if}
		 </h1>
       

			<p class="hero-paragraph">
                Computer Science Graduate, Software Engineer , Open Source Contributor
			</p>

            <ul class="social-network social-circle">
                <li><a  target="_blank"   href="https://github.com/arifuzzaman31" class="icoRss" title="Rss"><i class="fab fa-github"></i></a></li>
                <li><a  target="_blank"   href="https://facebook.com/" class="icoFacebook" title="Facebook"><i class="fab fa-facebook"></i></a></li>
                <li><a  target="_blank"  href="https://twitter.com/Arifuzzaman31" class="icoTwitter" title="Twitter"><i class="fab fa-twitter"></i></a></li>
                <li><a    href="mailto:arifuzzaman.rb@gmail.com" class="icoGoogle" title="Google +"><i class="fa fa-envelope"></i></a></li>
                <li><a  target="_blank"  href="https://www.instagram.com/arifuzzaman.rb/" class="icoLinkedin" title="Instagram"><i class="fab fa-instagram"></i></a></li>
            </ul>	
		</div>
	</div>