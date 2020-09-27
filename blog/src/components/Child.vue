<template>
    <div>
        <h1>Child Component</h1> 
        <Users />
        <Product/>
        
    </div>
</template>
<script>
import Users from './Users.vue'
import Product from './Product.vue'

export default {
    name: "Child",
    components: {
        Users,
        Product
    }
}
</script>

<style scoped>
div {
    background-color:aqua;
    height: 500px;
}
</style>

