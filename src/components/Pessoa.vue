<template>
    <div>
        <h2>Esta e a descrição da pessoa:{{ nome }}</h2>
        <Info />
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
            nome: "Idail Neto"
        }
    }
}
</script>