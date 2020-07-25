<script>
	let languages = [
       { id : 1, icon: 'fab fa-html5 fa-2x', name : 'HTML' , experience : '3 Year' },
       { id : 2, icon: 'fab fa-css3  fa-2x', name : 'CSS' , experience : '3 Year' },
       { id : 3, icon: 'fab fa-php fa-2x', name : 'PHP' , experience :   '3 Year' },
       { id : 4, icon: 'fas fa-database fa-2x', name : 'Mysql' , experience : '3 Year' },
       { id : 5, icon: 'fab fa-js-square fa-2x', name : 'Javascript' , experience : '2 Year' },
	];

	let frameworks = [
       { id : 1, icon: 'fab fa-laravel fa-2x', name : 'Laravel' , experience : '2 Year' },
       { id : 2, icon: 'fab fa-bootstrap fa-2x', name : 'Bootstrap' , experience : '3 Year' },
       { id : 3, icon: 'fab fa-jquery fa-2x', name : 'Jquery' , experience : '2 Year' },
       { id : 4, icon: 'fab fa-vuejs fa-2x', name : 'Vue.js' , experience :   '1 Year' },
       { id : 6, icon: 'fab fa-staylinked fa-2x', name : 'Svelte' , experience :   '1/2 Year' },
	];
</script>

<div class="row expertise-area">
    <div class="col-md-12 text-center">
    	<h1 class="service-title mt-5 text-white">Where i skilled at</h1>
    	<!-- <hr style="background-color: #fff"> -->
    </div>
	<div class="col-md-5 mx-auto text-center mt-5 mb-5">
	<h3 class="exp-title  mt-2">Language</h3>
	 {#each languages as lang, index}
	    <div class="tech">
	   		<h4 title="{lang.name}"><i class="{lang.icon}"></i></h4>
	   		<p>Experience : { lang.experience } +</p>
	   	</div>    	
	   {/each}
	</div>	


	<div class="col-md-5 mx-auto text-center mt-5 mb-5">
	<h3 class="exp-title mt-2">Framework</h3>
	 {#each frameworks as fram, i}
	    <div class="tech">
	   		<h4 title="{fram.name}"><i class="{fram.icon}"></i></h4>
	   		<p>Experience : { fram.experience } +</p>
	   	</div>    	
	   {/each}
	</div>

  

</div>

<style type="text/css">
	.exp-title
	{
		color: #fff;
		font-size: 2.5em;
		text-transform: uppercase;
	}
	.tech
	{
      margin-top: 20px;
      padding: 10px  0px ;
      /*border-bottom: 1px solid #fff;*/
      cursor: pointer;
	}

	.fa-jquery:after{
		    content: "Jquery";
		    font-size: 25px;
	}

	.tech h4,p{
		color: #fff;
		text-transform: uppercase;
	}
</style>