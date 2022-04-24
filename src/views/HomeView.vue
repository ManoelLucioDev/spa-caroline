<template>
<div>
  <v-carousel :show-arrows= "false" cycle hide-delimiters >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src "
      
      
    ></v-carousel-item>
  </v-carousel>

  <section>
      <div>
        <h2>{{title}}</h2>
      </div>

  </section>

</div>


</template>

<script>


export default {
  name: 'HomePage',
data () {
      return {
        items: [
          {
            src: require('../assets/slide1.png')
          },
            {
            src: require('../assets/slide2.png')
          },
            {
            src: require('../assets/slide3.png')
          },
            {
            src: require('../assets/slide4.png')
          },
        ],
        title: 'Titulo sobre os projetos, ou serviços'
      }
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.example-slide {
  align-items: center;
  
  background-color: #999;
  color: #999;
  display: flex;
  font-size: 1.5rem;
  justify-content: center;
  min-height: 10rem;
}
</style>

