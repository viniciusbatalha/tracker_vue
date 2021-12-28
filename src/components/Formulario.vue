<template>
    <div class="box">
        <div class="clomuns">
            <div class="column is-8" role="form" aria-label="Formulário para uma nova tarefa">
                <input type="text" class="input" placeholder="Qual tarefa deseja inserir?" v-model="descricao"/>
            </div>
            <div class="column">
                <temporizador @aoTemporizadorFinalizado="finalizarTarefa"/>
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
    },
    data () {
        return {
            descricao: ''
        }
    },
    methods: {
        finalizarTarefa (tempoDecorrido: number) : void {
            console.log('tempo da tarefa', tempoDecorrido)
            console.log('decrição da tarefa', this.descricao)
            this.descricao = ''
        }
    }
})
</script>

<style>

</style>