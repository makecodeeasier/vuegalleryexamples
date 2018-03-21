<template>
  <div id="app">
   <ImgGallery/>
   <hr> 
 <Carousel/>
 <hr> 
   <h2 style="margin-bottom:30px">Inne przykłady użycia</h2>
  <Coverflow :coverList="coverList" :coverWidth="260" :index="2"/> 
<hr>
  <coverflow :coverList="coverList" :coverWidth="260" :index="2" :coverShadow="true"></coverflow>
   
<hr>
    <coverflow :coverList="coverList" :coverWidth="260" :coverSpace="100" :index="0" :coverFlat="true"></coverflow>

  </div>
</template>

<script>
import ImgGallery from './components/ImgGallery';
import Carousel from './components/Carousel';
import Coverflow from './components/Coverflow';


export default {
  name: 'App', 
  data(){ 

 return {
   coverList: [
                {
                  cover: 'http://dev.itsense.pl/adgroup/images/p1.jpg',
                  title: 'MAKE CODE EASIER'
                }, {
                  cover: 'http://dev.itsense.pl/adgroup/images/p2.jpg',
                  title: 'MICHAŁ GÓRECKI'
                }, {
                  cover: 'http://dev.itsense.pl/adgroup/images/p3.jpg',
                  title: 'Vue'
                }, {
                  cover: 'http://dev.itsense.pl/adgroup/images/p4.jpg',
                  title: 'Webpack'
                }, {
                  cover: 'http://dev.itsense.pl/adgroup/images/p5.jpg',
                  title: 'Fron End Developer'
                }, {
                  cover: 'http://dev.itsense.pl/adgroup/images/p6.jpg',
                  title: 'Node'
                }
              ]
         }

  },
  components: {
        ImgGallery,
    Carousel, 
    Coverflow
    
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

hr{
  margin-top:50px;
  margin-bottom:50px;
}

 

body,
dl,
dt,
dd,
ul,
ol,
li,
h1,
h2,
h3,
h4,
h5,
h6,
pre,
code,
form,
fieldset,
legend,
input,
textarea,
p,
blockquote,
th,
td,
button,
article,
aside,
details,
figcaption,
figure,
footer,
header,
menu,
nav,
section {
  margin: 0;
  padding: 0;
}

*,
*:before,
*:after {
  box-sizing: border-box;
}

ins,
a {
  text-decoration: none;
}

ul {
  list-style: none;
}

html {
  font-size: 12px;
  line-height: 1.4em;
  font-family: -apple-system, BlinkMacSystemFont, 'PingFang SC', 'Hiragino Sans GB', 'Microsoft YaHei', sans-serif;
}

.head,
.foot {
  height: 84px;
  margin-bottom: 30px;

  background-color: #16c1c8;
  box-shadow: 0 1px 6px rgba(0, 0, 0, .10), 0 1px 4px rgba(0, 0, 0, .10);

  text-align: center;
  line-height: 84px;

  font-size: 24px;
  color: #fff;
}

.foot {
  margin-bottom: 0;
}

h2 {
  text-align: center;

  color: #808080;
}

a {
  color: #fff;
}

a:hover {
  color: #ddd;
}




</style>
