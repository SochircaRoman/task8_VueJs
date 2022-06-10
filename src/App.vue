<script>
import ListPersons from './components/ListPersons.vue';

export default {
    components: { ListPersons },
    data() {
        return {
            personInformation: {},
        }
    },
    methods: {
        
    },


}

</script>

<template>

    <div class="app">
        <list-persons @emitPersonInformation="emitPersonInformation"></list-persons>
        <details-persons :personInformation="personInformation"></details-persons>
    </div>


  
</template>

<style scoped>

.app{
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

</style>
