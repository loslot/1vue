<template>
  <Nav/>
  <Main/>
  <Footer/>
</template>

<script>
import Footer from './components/Footer.vue';
import Main from './components/Main.vue';
import Nav from './components/Nav.vue';


export default {
  name : 'App.vue' ,
  components : {
    Nav,
    Main,
    Footer,
  }  
}
</script>


<!-- <template>
<Data1/>
</template>

<script>
import Data1 from './components/Data1.vue';

export default {

  name :  'App',
  components : {
    Data1,
  }
}
</script> -->

<!-- <template>
<Ui name="Jonh" gender="male" :age="19"/>
<Ui name="Nita" gender="female" :age="8"/>
<Ui name="Devit" gender="male" :age="12"/>
<Ui name="Meta" gender="female" :age="5"/>
<Ui name="Sna" gender="male" :age="9"/>
</template>

<script>
import Ui from './components/Ui.vue';

export default { 
  name : 'App.vue',
  components : {
    Ui,
  }
}
</script>      -->


<!-- 
<template>

</template>

<script>
import Ui from './components/Ui.vue';

export default { 
  name : 'App.vue',
  components : {
    Ui,
  }
}
</script>      -->


<!-- <script setup>
import Ui from './components/Ui.vue';

function handlHello(name){
  alert (`Hello from : ${name}`)
}
</script>

<template>
  <Ui @Say-Hello="handlHello"/>
</template> -->
