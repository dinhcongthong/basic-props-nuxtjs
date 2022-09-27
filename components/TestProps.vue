<template>
    <div>
        This is child component. <br />
        My name is {{dataFromParents}} <br />
        <button @click="addToCart()">button</button>
    </div>
</template>

<script>
export default {
    data: function () {
        return {
            dataFromParents: this.user
        }
    },
    props: ['user'],
    created: function () {
    },
    methods: {
        addToCart (event) {
            this.$emit('update-cart', 'some value da click roi nhe')
        }
    },
    name: 'TestProps'
}
</script>