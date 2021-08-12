<template>
<div>
    <Header />
    <h2>Our Shop Page</h2>
    <div>
        <button @click="addItem">Add item</button>
    </div>
</div>
</template>


<script>
import Header from 'Company/Header';
export default {
 components: {
     Header,
 }, 
 methods: {
         addItem() {
             this.$store.state.cartItems += 1
         }
     },  
}
</script>