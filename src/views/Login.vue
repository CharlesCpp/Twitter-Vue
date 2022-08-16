<template>
    <div class="container">
        
    </div>
</template>

<script lang="ts">
    import { ref } from 'vue';
    import { supabase } from '../supabase'
    
    export default {
        setup() {
            const email = ref();

            return {
                email,
            }
        }
        
    }
</script>

<style scoped>

</style>