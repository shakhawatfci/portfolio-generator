<script type="text/javascript">
	let companies = [
     { id: 1, companyName : 'DoofazIT' ,  position: 'Jr Software Engineer', period : 'Jan, 2016 - Nov, 2016' },
     { id: 2, companyName : 'Belogin' ,  position: 'Software Engineer', period : 'Mar, 2017 - Oct, 2019' },
     { id: 3, companyName : 'Limmex Automation' ,  position: 'Sr Software Engineer', period : 'Nov, 2019 - Currrently Working' },
	];
</script>

		<!-- what i do  -->

     <div class="row">
		<div class="col-md-12 text-center">
			<h1 class="service-title mt-5">Companies I worked with !</h1>
		</div>
	</div>		
     <div class="row">
       {#each companies as value}
       	  <div class="col-md-4">
     		<div class="work-section">
     			<h3 class="work-icon">
     				<i class="fa fa-first-order" aria-hidden="true"></i>
     			</h3>
     			<h3 class="work-title">{value.companyName}</h3>
                <p>Position : { value.position }</p>
                <p><i class="fa fa-calendar-check-o" aria-hidden="true"></i>
  {value.period}</p>
     		</div>
     	</div>
       {/each}
     	
     </div>
	<!-- what i do  -->