<template>
    <div>
        <h4> je suis :</h4>
            <ul class="liste">
                <li v-for="(fruit, index) in fruits" v-bind:key="index">
            {{ index }}  :  {{ fruit }}
                </li>
            </ul>

            <p>{{ prenom }}</p>
            <!-- <p>{{ reversing() }}</p> -->

    </div>
</template>

<script>
    
    export default {
        name:'liste',
    data () {
    return {
        fruits:[
            'banane','fruit'
        ]
    }
},
    props:{
        prenom:{
            type : String,
        }
    },
    // methods: {
    //     reversing: function (){
    //         return this.prenom.split('').reverse().join('');
    //     }
    // }
    }
</script>
<style scoped src='../css/test.css'>

</style>