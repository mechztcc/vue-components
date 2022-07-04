<template>
    <div class="citacao">
        {{ texto }}
        <slot name="autor" v-if="true"></slot>
        <slot></slot>
    </div>
</template>

<script>
export default {
    // props: {
    //     texto: [String]
    // }
    props: {
        texto: {
            type: String,
            required: true,
            default: 'Carregando'
        }
    }
}
</script>

<style scoped>
    .citacao {
        border: 1px solid #DDD;
        background-color: rgba(0, 0, 0, .1);
        padding: 25px;
        max-width: 450px;
    }
</style>
