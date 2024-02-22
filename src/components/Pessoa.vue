<template>
    <div>
        <h2>Esta e a descrição da pessoa:{{ nome }}</h2>
        <Info :email="email" :esta_trabalhando="false"/>
        <Form/>
    </div>
</template>

<script>

import Info from './Info';
import Form from './Form.vue';
export default {
    name: "Pessoa",
    components: {
        Info,
        Form
    },
    data() {
        return {
            nome: "Idail Neto",
            email:"neto_br_8@hotmail.com"
        }
    }
}
</script>