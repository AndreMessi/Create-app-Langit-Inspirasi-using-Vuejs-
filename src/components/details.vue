<template>
	<div class="details">
		<div class="container">
			<div class="row">
				<div class="col-md-12" v-for="(product,index) in products" :key="index"> 
					<div v-if="proId == product.productId">
						<h1>{{product.productTitle}}</h1>
						<img :src="product.image" class="img-fluid">
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
<script>
	export default{
		name:'details',
		data(){
			return{
				proId:this.$route.params.Pid,
				title:"details",
				products:[
							{
								productTitle:"buku pintar lagu wajib nasional",
								image       : require('../assets/images/product1.jpg'),
								productId:1
							},
							{
								productTitle:"tuntunan pemerograman java",
								image       : require('../assets/images/product2.jpg'),
								productId:2
							},
							{
								productTitle:"buku pintar C++",
								image       : require('../assets/images/product3.jpg'),
								productId:3
							},
							{
								productTitle:"belajar pemerograman android",
								image       : require('../assets/images/product4.jpg'),
								productId:4
							},
							{
								productTitle:"mudah belajar matematika",
								image       : require('../assets/images/product5.jpg'),
								productId:5
							},
							{
								productTitle:"kumpulan cerita kancil dan buaya",
								image       : require('../assets/images/product6.jpg'),
								productId:6
							}
							]
			}
		}
		
	}
</script>