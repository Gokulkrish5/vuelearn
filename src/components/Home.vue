
<!--About interpolation:
Passing a data from inside script and display it in template
Send data to script to html tag
-->

<template>
<div>
  <h1>Test page home</h1>
  <h1> Email : {{email}} </h1>
  <h2>mobile:{{mobile}}</h2>
  <h2>mobiles:{{mobiles=9999}}</h2>
  <!--We can assign value inside interpolation -->
  <h2>Name: {{getname()}}</h2>
  <h2>Name Pass:{{passName("Gokul pass data")}}</h2>
  </div>

</template>
<script>
export default {
    name:"Home",
    data(){
        return{
            email:"gk@test.com",
            mobile:1023,
            mobiles:8098,
            getname(){
                return "Gokul"
            },
            passName(x){
                return x;
            }
        }
    }
}
</script>

<style scoped>
h1{
    color:orange;
}
h2{
    color:gray
}
</style>