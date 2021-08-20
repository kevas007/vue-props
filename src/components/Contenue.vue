    <template>
        <div>
            <h1>{{ text }}</h1>
            <h1>{{para}}</h1>
            <liste :prenom="prenom"></liste>
        </div>
    </template>



    <script>
        import Liste from './Liste.vue';
    export default {
        name:'contenue',
    data() {
        return {
            para: 'je suis un bg',
            text: "je suis dev",
        
            prenom:10000,

        };
    },
    components: {
        'liste': Liste
    }
    };
    </script>

    <style>
    </style>