<template>
    <div>
        <h2>Esta e a descrição de pessoa: {{ nome }}</h2>
    </div>
    <Info/>
</template>

<script>
import Info from './Info.vue';
export default{
    name:"Pessoa",
    components:{
        Info
    },
    data(){
        return{
            nome:"Idail"
        }
    }
}
</script>