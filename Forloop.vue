<template>
<div>
    <h1 class="vue-style">for loop in vue</h1>
    <h1 v-bind:style="{color:colorname}">for loop in vue</h1>
    <table border="2px">
        <tr>
            <td>id</td><td>name</td><td>email</td>
        </tr>
        <tr v-for="item in array1" :key="item.id">
            <td>{{item.id}}</td><td>{{item.name}}</td><td>{{item.email}}</td>
        </tr>
    </table>

</div>
</template>
<script>
export default {
    data() {
        return{
            colorname:'skyblue',
array1:[
    {id:1,name:"shiv",email:"shiv@gmail.com"},
    {id:2,name:"shiva",email:"shiva@gmail.com"},
    {id:3,name:"shivu",email:"shivu@gmail.com"},
    {id:4,name:"shivani",email:"shivani@gmail.com"},
]
        }
    },
}
</script>
<style scoped>
.vue-style{
    color: orange;
}
</style>