<template>
    <div>
        Home
    </div>
    <p>
        Name in store is: {{ name }}
    </p>
</template>

<script setup>
import { useStore } from 'vuex'
import { computed } from 'vue'

const store = useStore()

const name = computed(() => {
    return store.state.user.name
})
    
</script>