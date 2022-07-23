<template>
<div>
    <h1>Home Componant</h1>
    <button v-on:click="test1('button 1 clicked')">1 time click</button>
    <button v-on:dblclick="test1('button 2 clicked')">2 time click</button>
    <button v-on:click="getdata()">for count</button>
    <button v-on:click="getconsole()">clik me</button>
    <h2>{{count}}</h2>
</div>
</template>
<script>


export default {
    name:"Event",
    data(){
        return{
             count:0
        }
    },
    methods:{
        getdata()
        { 
        
          this.count=this.count+1;


        
        },
        test1(data)
        {
            alert(data);
        },
        getconsole()
        {
alert("function called");
        }
    }
}
</script>
