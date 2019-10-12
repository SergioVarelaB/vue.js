<template>
    <div>
        <!--<div v-text ="title"></div>
        <div v-if="showName">
            <p>{{user.firstName}}</p>
        </div>
            <div v-else>
                <p>no se puede mostrar nombre</p>
            </div>
        <hr>
        <ul>
            <li v-for-key="task in tasks">
                {{task.title}}
            </li>
        </ul>-->
        <input type="text" v-model="user.firstName">
        <button type = "button" v-on:click="saludar(user.firstName)">
            picale pero con cuidado
        </button>
        <hr>
        <input type="text" v-on:keyp = "typeando">

    </div>
    
</template>


<script>
    export default {
        data(){
            return{
             title: 'que pex vue.js',
             user: {
                 firstName: 'joe',
                 lastName: 'battle'
             },
            myhtml: '<h3>que pex</h3>', 
            showName : false,
            tasks: [
                {title: 'eat'},
                {title: 'dinner'},
                {title: 'eat'}
            ]
           }
        },
        methods: {
            saludar(name){
                alert('ya te gusto '+name )
            },
            typeando(){
                
            }
        }
    }
</script>

<style media = "screen">

</style>