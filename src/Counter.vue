<template>
    <div>
        {{ count }}
        <div @click="increment">+</div>
    </div>
</template>

<script>
    import store from './store/NotificationStore'
    export default {
        name: "Counter",
        data () {
            return {
                state: store.state
            }
        },
        computed: {
            count () {
                return store.state.count
            }
        },
        methods: {
            increment () {
                store.increment()
            }
        }
    }
</script>

<style scoped>

</style>