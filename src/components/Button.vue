<template>
    <!--v-on:click="onClick()" works the same as @click="onClick()"-->
    <button @click="onClick()" :style="{background:color}" class="btn">
        {{text}}
    </button>
</template>

<script>
export default {
    name: "Button",
    props: {
        text: String,
        color: String
    },
    methods:{
        onclick(){
            console.log('Click');
        }
    }
}
</script>