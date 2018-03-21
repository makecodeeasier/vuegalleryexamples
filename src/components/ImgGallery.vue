<template>
<section>
    <div style="row">
    <gallery :images="images" :index="index" @close="index = null"></gallery>



<h2>Klasyczna galeria wywoływana przy naciśnięciu przycisku</h2>

<button class="btn btn-primary btn-lg" style="margin:10px" @click="index = imageIndex" >POKAŻ GALERIĘ</button>

  </div>

  </section>
</template>
  
<script>
  import VueGallery from 'vue-gallery';
  
  export default {
    name: 'ImgGallery',
    data: function () {
      return {
        images: [
          'http://dev.itsense.pl/adgroup/images/p1.jpg',
          'http://dev.itsense.pl/adgroup/images/p2.jpg',
          'http://dev.itsense.pl/adgroup/images/p3.jpg',
          'http://dev.itsense.pl/adgroup/images/p4.jpg',
          'http://dev.itsense.pl/adgroup/images/p5.jpg',
          'http://dev.itsense.pl/adgroup/images/p6.jpg',
          
        ],
        index: null
      };
    },
 
    components: {
      'gallery': VueGallery
    },
  }
</script> 