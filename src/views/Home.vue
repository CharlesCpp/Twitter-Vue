<template>
    <div>
        Hello
    </div>
</template>

<script lang="ts">
    import { onMounted } from "vue";
    import { supabase } from "../supabase"
    export default {
        setup() {
            function getClient() {
                let user = supabase.auth.user()?.id;
                console.log(user);
            }
            
            onMounted(() => {
                getClient();
            })

            return {
                getClient,
            }
        }
    }
</script>

<style scoped>

</style>