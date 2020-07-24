<script type="text/javascript">
	let services = [
     { id: 1, serviceName : 'Software Development' , icon : 'fas fa-project-diagram' },
     { id: 2, serviceName : 'Apps Development' , icon : 'fab fa-app-store' },
     { id: 3, serviceName : 'Web Development' , icon : 'fas fa-laptop-code' },
     { id: 4, serviceName : 'Web Design' , icon : 'fa fa-globe' },
     { id: 5, serviceName : 'SASS PROVIDER' , icon : 'fa fa-cubes' },
     { id: 6, serviceName : 'Custom Software' , icon : 'fa fa-cogs' }
	];
</script>

		<!-- what i do  -->

     <div class="row">
		<div class="col-md-12 text-center">
			<h1 class="service-title mt-5">What I Do ?</h1>
		</div>
	</div>		
     <div class="row">
       {#each services as value}
       	  <div class="col-md-4">
     		<div class="work-section">
     			<h3 class="work-icon">
     				<i class={value.icon} aria-hidden="true"></i>
     			</h3>
     			<h3 class="work-title">{value.serviceName}</h3>
     		</div>
     	</div>
       {/each}
     	
     </div>
	<!-- what i do  -->