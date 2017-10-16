<style lang="scss" scoped>
.talk {
    font-size: 0.9rem;
    background-color: #F2F0F0;
    padding: 0.5rem;
    position: relative;
}
.talk__button{
    position: absolute;
    top: 0;
    bottom: 0;
    right: 0;
    background-color: #000;
    border: none;
    color: #FFF;
    padding: 0.5rem;
    cursor: pointer;
    transition: background-color 1s;
    &:hover{
        transition: background-color 1s;
        background-color: #029319;
    }
}
.talk__plus-one {
    font-size: 1.5rem;
    line-height: 1;
    display: block;
}
</style>

<template>
    <section class="category">
        <h3>Kategoriename</h3>
        <Talk />
    </section>
</template>

<script>
import Talk from '../components/Talk.vue'
export default {
  name: 'Category',
  components: {
    'Talk': Talk
  }
}
</script>
