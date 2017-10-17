<style lang="scss" scoped>
.talk {
    font-size: 0.9rem;
    background-color: #F2F0F0;
    position: relative;
    margin: 0.75em 0;
    display: block;
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
    transition: background-color 0.5s;
    border-left: 1px solid #FFF;
    &:hover{
        transition: background-color 0.5s;
        background-color: #029319;
    }
}
.talk__plus-one {
    font-size: 1.5rem;
    line-height: 1;
    display: block;
}
.talk__link{
    color: #000;
    display: block;
    padding: 0.5rem;
    transition: background-color 0.5s;
    &:hover {
        transition: background-color color 0.5s;
        background-color: #000;
        color: #FFF;
    }
    text-decoration: none;
}
</style>

<template>
    <div class="talk">
        <button class="talk__button">
            <span class="talk__plus-one">+1</span>
            vote
        </button>
        <a href="#" class="talk__link" v-on:click="hideShowTalk">
            <h4>Talk Title</h4>
            <div class="talk__authors">Author Name, Name of Author</div>
        </a>
        <Modal v-bind:showTalk="showTalk" />
    </div>
</template>

<script>
import Modal from '../components/Modal.vue'

export default {
  name: 'Talk',
  components: {
    'Modal': Modal
  },
  data: function () {
    return {
      showTalk: false
    }
  },
  methods: {
    hideShowTalk: function () {
      this.showTalk = true
    }
  }
}
</script>
