<!--Methods property
Same like interpolation paasing data but don't overwrite the values
Here we can able to use the data function output to inside method

-->

<template>
<dev>
    <h1>This is method property example</h1>
    <h2>First name: {{getName("Gokul")}}</h2>
    <h2>Last Name: {{getName("Krish")}}</h2>
    <h2>DataName: {{getData().name}}</h2>
    <h2>DataName: {{getData().email}}</h2>
    <h2>topName: {{getData().nameTop}}</h2>
    </dev>
</template>
<script>
export default{
    name:"Methods",
    data(){
        return{
            name:"Top Gokul"
        }
    },

    methods:{
    getName(name){
        return name;  
    },
    getData(){
        return{
            name:"Gk",
            email:"Gk@test.com",
            nameTop:this.name
        }
    }
    }
    
}

</script>