<script>
// import { fade, fly } from 'svelte/transition';
import HeroArea from './components/hero/HeroArea.svelte';
import Services from './components/services/Service.svelte';
import Expertics from './components/expertices/expertics.svelte';
import WorkFor from './components/work/WorkFor.svelte';

</script>


<div class="container-fluid hero-area">
	<!-- hero area  -->
	 <HeroArea/>
	<!-- hero area  -->
</div>

<div class="container">
   <!-- services  -->
   <Services/>
   <!-- services  -->
</div>

<div class="container-fluid mt-5">
	    <!-- expertise  -->
     <Expertics	/>
	<!-- expertise  -->
</div>

<div class="container">
   <!-- worked with  -->
   <WorkFor/>
   <!-- worked with  -->
</div>	



