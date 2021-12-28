<template>
    <div class="box">
        <div class="clomuns">
            <div class="column is-8" role="form" aria-label="Formulário para uma nova tarefa">
                <input type="text" class="input" placeholder="Qual tarefa deseja inserir?"/>
            </div>
            <div class="column">
                <temporizador/>
            </div>
        </div>
    </div>
</template> 

<script lang="ts">
import { defineComponent } from 'vue'
import Temporizador from './Temporizador.vue'

export default defineComponent({
    name: 'Formulário',
    components: {
        Temporizador
    }
})
</script>

<style>

</style>