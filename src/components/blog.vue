<template>
	<div class="blog">
		<h1>{{title}}</h1>
		<div class="row">
			<div class="col-md-4">
				<div class="card">
					<div class="card-header">
						<h3>Vus.js</h3>
					</div>
					<div class="card-body">
						Vue.js adalah framework javascript yang digunakan untuk membangun user interface.Vue.js tidak selengkap framework javascript lainnya. Namun, kesederhanaan tersebut membuat Vue.js mudah untuk digunakan dan diintegrasikan dengan library lain maupun projek yang sudah jadi.
					</div>
				</div>
			</div>
			<div class="col-md-4">
				<div class="card">
					<div class="card-header">
						<h3>Angular</h3>
					</div>
					<div class="card-body">
						 Angular JS merupakan framework javascript open souce yang dirilis oleh google pada tahun 2009. Konsep dari Angular JS adalah meningkatkan fungsi dari HTML untuk membangun web app. Bayangkan awalnya HTML hanya digunakan untuk membuat halaman website statis dan kini bisa berfungsi untuk membuat web app dengan menggunakan Angular JS.
					</div>
				</div>
			</div>
			<div class="col-md-4">
				<div class="card">
					<div class="card-header">
						<h3>React</h3>
					</div>
					<div class="card-body">
						React JS adalah sebuah pustaka/library javascript yang bersifat opensource untuk membangun User Interface yang dibuat oleh Facebook. React JS hanya mengurusi semua hal yang berkaitan dengan tampilan dan logika di sekitarnya.
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
	export default{
		name:'blog',
		data (){
			return{
				title:'blog resmi Langit Inspirasi'
			}
		}
	}
</script>

<style scoped>
	
</style>