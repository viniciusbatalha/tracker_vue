<template>
    <div class="box has-text-weight-bold">
        <div class="columns">
            <div class="column is-7">Descrição da tarefa</div>
            <div class="column">
                <cronometro tempoEmSegundos="15"/>
            </div>
        </div>
    </div>
</template>

<script>
import { defineComponent } from 'vue'
import Cronometro from "./Cronometro.vue"

export default defineComponent({
    name: "Tarefa",
    components: {
        Cronometro,
    },
});
</script>

<style>
.box {
    background: #FAF0CA;
}
</style>