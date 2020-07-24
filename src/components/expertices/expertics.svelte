<script>
	let languages = [
       { id : 1, name : 'HTML' , experience : '6 Year' },
       { id : 2, name : 'CSS' , experience : '6 Year' },
       { id : 4, name : 'PHP' , experience :   '5 Year' },
       { id : 5, name : 'Mysql' , experience : '5 Year' },
       { id : 3, name : 'Javascript' , experience : '6 Year' },
       { id : 5, name : 'Node' , experience :   '1 Year' },
	];

	let frameworks = [
       { id : 2, name : 'Laravel' , experience : '4.5 Year' },
       { id : 2, name : 'Bootstrap' , experience : '6 Year' },
       { id : 3, name : 'Jquery' , experience : '6 Year' },
       { id : 4, name : 'Vue.js' , experience :   '2.5 Year' },
       { id : 6, name : 'Reactjs' , experience :   '1 Year' },
       { id : 7, name : 'Svelte' , experience :   '1 Year' },
	];
</script>

<div class="row expertise-area">
    <div class="col-md-12 text-center">
    	<h1 class="service-title mt-5 text-white">My Expertices</h1>
    </div>
	<div class="col-md-5 mx-auto text-center mt-5 mb-5">
	<h3 class="exp-title  mt-2">Language</h3>
	 {#each languages as lang, index}
	    <div class="tech">
	   		<h4 > {lang.name}</h4>
	   		<p>Experience : { lang.experience } +</p>
	   	</div>    	
	   {/each}
	</div>	


	<div class="col-md-5 mx-auto text-center mt-5 mb-5">
	<h3 class="exp-title mt-2">Framework</h3>
	 {#each frameworks as fram, i}
	    <div class="tech">
	   		<h4>{fram.name}</h4>
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
      border-bottom: 1px solid #fff;
      cursor: pointer;
	}

	.tech h4,p{
		color: #fff;
		text-transform: uppercase;
	}
</style>