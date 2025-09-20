<!-- <script setup>
    defineProps({
        name : String
    })
</script>

<template>

    <h1>Hello my name is : {{ name }}</h1>
</template> -->

<!-- <script setup>
    defineProps({
        name : String,
        gender : String,
        age : Number
    })
</script>

<template>
    <div class="container">
        <div class="card p-3 m-3">
            <img src="/public/2.png" alt="" class="img">
            <h4>Name  : {{ name }}</h4>
            <h4>Gender: {{ gender }}</h4>
            <h4>Age   : {{ age + 10}}</h4>
        </div>
    </div>
</template>

<style>
.container{
    display: flex;
    justify-content: center;
    align-items: center;
}
img{
    padding: 5px;
    margin: auto;
    align-items: center;
    border-radius: 50%;
    width: 100px;
    height: 100px;  
}
</style> -->

<!-- <script setup>
const emit = defineEmits(['sayHello']) // use camelCase inside JS

const username = 'John'

function handleEmitHello() {
  emit('sayHello', username)
}
</script>

<template>
  <button @click="handleEmitHello()">Click me</button>
</template> -->
