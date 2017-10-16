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
    <div class="talk">
        <button class="talk__button">
            <span class="talk__plus-one">+1</span>
            vote
        </button>
        <h4>Talk Title</h4>
        <div class="talk__authors">Author Name, Name of Author</div>
    </div>
</template>

<script>
export default {
  name: 'Talk'
}
</script>
