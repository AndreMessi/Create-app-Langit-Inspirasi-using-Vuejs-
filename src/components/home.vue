<template>
  <div class="home">
    <h1>{{title}}</h1>
    <div class="row">
      <div class="col-md-4 col-lg4" v-for="(data,index) in products" :key="index">
        <img :src="data.image" class="img-fluid">
         <h3 @click="goTodetail(data.productId)" >{{data.productTitle}}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      title: 'kumpulan buku Langit Inspirasi',
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
  },
  methods:{
  goTodetail(prodId) {
    let proId=prodId
    this.$router.push({name:'details',params:{Pid:proId}})
  }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.row img{
  max-height: 15em;
  width: 100%;

}
.row h3{
  cursor:pointer;
}
</style>
