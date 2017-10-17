<style lang="scss" scoped>
    .modal {
        background-color: rgba(0,0,0,0.8);
        position: fixed;
        z-index: 2;
        top: 0;
        bottom: 0;
        right: 0;
        left: 0;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .modal__window {
        background-color: #FFF;
        width: 50%;
        height: 50%;
        position: relative;
    }

    .modal__inner-contet{
        padding: 0.5rem;
    }

    .modal__footer{
        position: absolute;
        bottom: 0;
        right: 0;
        left: 0;
        padding: 0.5rem;
        background-color: #7F7F7F;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .modal__back-icon {
        height: 1rem;
        width: 1rem;
    }

</style>

<template>
    <div class="modal" v-show="showTalk">
        <div class="modal__window">
            <div class="modal__inner-contet">
                <h1>Talk Title</h1>

                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
                {{ $data }}
            </div>
            <div class="modal__footer">
                <span class="modal__back-wrapper">
                    <button v-on:click="hideModal">
                    <svg class="modal__back-icon" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 408 408"><path d="M408 178.5h-311.1l142.8-142.8-35.7-35.7-204 204 204 204 35.7-35.7-142.8-142.8h311.1v-51z"/></svg>
                    Back
                    </button>
                </span>

                <span class="modal__button-wrapper">
                    Is it interesting for you? <button>+1</button>
                </span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Modal',
  props: ['showTalk'],
  data: function () {
    return {
      'showTalk': this.showTalk
    }
  },
  methods: {
    hideModal: function () {
      this.showTalk = false
    }
  }
}
</script>
