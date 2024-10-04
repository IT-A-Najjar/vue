<template>
    <div class="parent">
        my name is {{ name }}
     <form>
        <slot name="slotHeader"></slot>
        <slot name="slotInputs"></slot>
        <slot name="slotActions"></slot>
     </form>
    </div>
</template>

<script>
export default{
    props:{
        name:{
            type: String,
        },
    },
};


</script>