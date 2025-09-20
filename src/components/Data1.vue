<!-- <template>
    <h1>Name            : {{ name }}</h1>
    <h1>Age             : {{ age }} Years old</h1>
    <h1>Status          : {{ status }}</h1>
    <h1>Position        : {{ position }}</h1>
    <h1>Language        : {{ language }}</h1>
    <h1>salary          : {{ salary }} $</h1>
    <h1>My age is       : {{ age }} .
     After plus 10 Final age is {{ plus }}.</h1>
</template>

<script>
export default{
    data(){
        return {
            name : 'John',
            age  : 80,
            position : 'Manager',
            language: 'Khmer and English',
            salary: 3000000,
            status: ''
        }

    },
    computed : {
        plus (){
            return this.age + 10
        }
    },

    created (){
        if (this.age < 18){
            this.status = 'ក្មេងជាង​ ១៨​ ឆ្នាំ'
        }else if( this.age >= 18 && this.age <60){
            this.status = 'មនុស្ស​ពេញវ័យ'
        }else{
            this.status = 'មនុស្សចាស់'
        }
    },
    name : 'Data1.vue',
}
</script> -->



<!-- <template>
    <h1>Username            : {{ username}}</h1>
    <h1>Email             : {{ email }}</h1>
    <h1>Password          : {{ pass }}</h1>
    <h1>Number            : {{ number }}</h1>
    <button @click="plush" >{{ number }}</button>
</template>

<script>
export default{
    data(){
        return {
            username : 'Los',
            email : 'Ma12@sdk11@gmail.com',
            pass : '2@Gat#22',
            number: 10,
        }
    },
    methods : {
        plush () {
            this.number= this.number+1
        }
    },  
    wacth : {
        number (valuenum){
            if (valuenum >15 ){
                alert ("full")
            }
        }
    },
    name : 'Data1.vue',
}  
</script> -->
<!-- 


<template>
    <button @click="uncount" :disabled="number <= 0">-</button>
    <h1>{{ setNumber }}</h1>
    <button @click="count" :disabled="number >= 5">+</button>

</template>

<script>
export default {
    data (){
        return {
            number : 0,
        }

    },
    methods : {
        count (){
            this.number = this.number + 1
        },
        uncount (){
            this.number = this.number -1

        }
    },
    computed : {
        setNumber () {
            return this.number +10
        }
    }
}
</script> -->


<!-- <template>
    <button @click="uncount" :disabled="number <= 0">-</button>
    <h1>{{ number }}</h1>
    <button @click="count" :disabled="number >= 20">+</button>
    <h2>Text: {{ text }}</h2>

</template>

<script>
export default {
    data (){
        return {
            number : 0,
            text: ''
        };

    },
    methods : {
        count (){
           return this.number = this.number + 1
        },
        uncount (){
           return this.number = this.number -1

        }
    },
    watch : {
        number (newVal){
            if(newVal <= 10){
                this.text = "small"
            }else{
                this.text = "big"
            }
        }
    }
}
</script> -->

<!-- <template>
    <h1>-Number</h1>
    <button @click="number--" :disabled="number<=0"> -1</button>
    <h1> <={{ number }}=></h1>
    <button @click="number++" :disabled="number>=10"> +1</button>
    <h1>+Number</h1>
</template>

<script>
export default {
    data (){
        return {
            number : 0,
        }
    }
}
</script> -->

<!-- <template>
    <h1>UserName : {{ data.name }}</h1>
    <h1>Gender   : {{ data.gender }}</h1>
    <h1>Age      : {{ age }}</h1>
    <h1>My Level : {{ level }}</h1>
    <button @click="level -=10" :disabled="level <=0">-10</button>
    <button @click="level +=10" :disabled="level >=100">+10</button>
    <h1>---------------------[ Major ]---------------------</h1>  
    <h1>
    <ul>
        <li v-for='(item, index) in major'>{{ index+1 }}. {{ item }}</li>
    </ul>
    </h1>
    

</template>

<script setup>
import { reactive, ref } from 'vue';
const age = ref(18)
const level = ref(0)
const data = reactive({
    name : 'Los',
    gender : 'Male' 
})
const major = ref(['IT', 'ITE', 'CS'])
</script> -->

<!-- <template>
    <button @click="plus">{{ number }}</button>
    <button @click="plus2">{{ number2.number }}</button>

</template>

<script setup>
import { reactive, ref } from 'vue';

const number =ref(0)
function plus (){
    number.value++
}
const number2 = reactive({
    number : 0,
})
function plus2 (){
    number2.number+=1
}
</script> -->

<!-- <template>
<h1 v-if="age <18">Young</h1>
<h1 v-else>Old</h1>
<img v-bind:src="image" alt="">
</template>

<script setup>
import { ref } from 'vue';

const age = ref(19)
const image = ref('1.png')
</script> -->





<!-- <script setup>
import { reactive, ref } from 'vue';
const word = ref('')
const member = reactive([
    {
        name : 'Los',
        gender : 'Male',
        image: 'public/2.png',
        age: 17
    },
    {
        name : 'Los',
        gender : 'Male',
        image: 'public/2.png',
        age: 90
    },
    {
        name : 'Los',
        gender : 'Male',
        image: 'public/2.png',
        age: 120
    }

])
</script>


<template>

<div v-for="data in member">
    <h1>Username: {{ data.name}}</h1>
    <h1>Gender: {{ data.gender}}</h1>
    <h1>Age: {{ data.age}}</h1>
    <h1 v-if="data.age <18">ក្មេង</h1>
    <h1 v-else-if="data.age <100">ចាស</h1>
    <h1 v-else="">ស្លាប់</h1>
    <img v-bind:src="data.image" alt="" width="300px" height="200px">
    <br>
    <hr>
</div>
<input v-model="word" type="text" placeholder="input your word">
<h3>Your word : {{ word }}</h3>
</template> -->



<!-- <script setup>
import { ref, watch} from 'vue';

const mode =ref(true)
function onClick(){
    mode.value= !mode.value
}
watch(mode, (newval)=>{

    if (newval){
        document.body.classList.add('light')
        document.body.classList.remove('dark')
    }else{
        document.body.classList.add('dark')
        document.body.classList.remove('light')
    }
})

</script>



<template>
    <button v-on:click="onClick">{{ mode? "Dark mode" : "Light mode" }}</button>
</template>
<style>
body.dark{
    background-color: black;
    color: white;
}
body.light{
    background-color: white;
    color: black;
}
</style> -->



<!-- <script setup>
function clickme(name){
    alert("Hello my name is" + name)
}
</script>

<template>
    <button @click="clickme (' Los')">Click on me</button>
</template> -->


<!-- <script setup>
import { ref } from 'vue'

const name = ref('')
const gender = ref('male')
const email = ref('')
const user = ref([])

function handleSubmit() {
  user.value.push({
    name: name.value,
    gender: gender.value,
    email: email.value
  })

  // Optional: Clear form fields after submission
  name.value = ''
  gender.value = 'male'
  email.value = ''
}
  // Delete
function handleDelete(index){
    user.value.splice(index, 1)
}
</script>

<template>
  <form
    class="w-25 shadow-sm m-auto mt-5 pt-3 rounded-3"
    @submit.prevent="handleSubmit"
  >
    <input
      type="text"
      v-model="name"
      placeholder="username"
      class="form-control my-1"
      required
    />

    <select class="form-control w-50 my-1" v-model="gender">
      <option value="male">male</option>
      <option value="female">female</option>
    </select>

    <input
      type="email"
      v-model="email"
      placeholder="email"
      class="form-control my-1"
      required
    />

    <div class="d-flex justify-content-center my-4">
      <button type="submit" class="btn btn-outline-success btn-sm">Add</button>
    </div>
  </form>

  <table class="table mt-5 text-center">
    <thead>
      <tr>
        <th>Name</th>
        <th>Gender</th>
        <th>Email</th>
        <th>Delete</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="(item, index) in user" :key="index">
        <td>{{ item.name }}</td>
        <td>{{ item.gender }}</td>
        <td>{{ item.email }}</td>
        <td class="btn btn-sm my-1 btn-danger" @click="handleDelete">delete</td>
      </tr>
    </tbody>
  </table>

</template> -->
<!-- 

<script setup>
import { ref } from 'vue';
const distance = ref('')
const price = ref('')
const total = ref('')
</script>
<style>
form {
    background-color: rgb(194, 37, 209);
}
</style>

<template>
    <form class="w-50 shadow-sm m-auto mt-5 pt-3 rounded-3 p-3" >
        <h3 class="text-center"> PassAp Price <br>Calculator </h3>
    <p class="">Distance (km):</p>
     <input type="text" v-model="name" placeholder="Input" class="form-control " accordion-itemrequired/>
    
     <p class="pt-3">Price per km ($)</p>
     <input type="text" v-model="name" placeholder="Input" class="form-control mt-0" required
    />
        <h3 class="text-center mt-3">Total Price: {{ distannce*price }}</h3>

    </form>
</template> -->

<script setup>
import { ref, computed } from 'vue';

const distance = ref('');
const price = ref('');

// Computed total price
const total = computed(() => {
  const d = parseFloat(distance.value);
  const p = parseFloat(price.value);
  return isNaN(d) || isNaN(p) ? 0 : d * p;
});
</script>

<template>
  <form class="w-50 shadow-sm m-auto mt-5 pt-3 rounded-3 p-3">
    <h3 class="text-center p-3"> PassApp Price <br />Calculator </h3>

    <p>Distance (km):</p>
    <input type="text" v-model="distance" placeholder="Enter distance" class="form-control" />

    <p class="pt-3">Price per km ($):</p>
    <input
      type="text" v-model="price" placeholder="Enter price" class="form-control"/>

    <h3 class="text-center mt-3">Total Price: ${{ total.toFixed(2) }}</h3>
  </form>
</template>

<style>
form {  
  background-color: rgb(87, 186, 239);
}
</style>


