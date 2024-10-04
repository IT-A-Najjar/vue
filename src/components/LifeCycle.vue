<template>
    <div class="life" style="margin-top: 50px;">
        <h2>Life Cycle Hooks </h2>
        <p>age is:{{ age }}</p>
        <button @click="$event =>age++"> inc age</button>
        </div>
</template>

<script>
export default{
    data(){
        return{
            name:"aamna",
            age:23,
        };
    },
    beforeCreate(){
       alert("Befor Updata");
    },
    created(){
        alert("created");
    },
    beforeMount(){
        alert("Befor Mount");
    },
    mounted(){
        alert("Mounted");
    },
    beforeUpdate(){
        alert("befor Update");
    },
    updated(){
        alert("Update");
    },
    beforeUnmount(){
        alert("beforUnmount");
    },
    unmounted(){
        alert("UnMounted");
    },
};

</script>