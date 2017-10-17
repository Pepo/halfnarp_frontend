<style lang="scss" scoped>
.footer{
    position: fixed;
    bottom: 0;
    width: 100%;
    background-color: #7F7F7F;
    text-align: right;
}
.footer__inner-wrapper {
    width: 1280px;
    margin: 0 auto;
    padding: 0.5rem;
}
.footer__headline {
    display: inline;
    font-size: 1.5rem;
}
.footer__button {
    font-size: 1.5rem;
    padding: 0.25rem 1rem;
}
</style>

<template>
	<footer class="footer">
        <div class="footer__inner-wrapper">
        <h4 class="footer__headline">You have choosen 2 talks</h4>
        <button class="footer__button">Submit and help</button>
        </div>
	</footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>
