<script lang="ts">
    import Moon from './moon.svelte';
</script>

<div id="home" class="home">
    <div class="home--text">
        <p>
            Boston.<br>
            Inside a garden,<br>
            When the moon will shine<br>
            A festival will take place<br>
        </p>
    </div>

    <div class="home--svg">
        <Moon />
    </div>

</div>

<style lang="scss">
    @media only screen and (max-width: 600px) {
        .home--text {
            text-align: center;
        }
    }
    .home {
        position: relative;
        background: #2F2E41;
        width: 100vw;
        height: 100vh;

        &--text {
            color: white;
            position: absolute;
            top: 10%;
            left: 10%;

            font-size: 3rem;
            line-height: 49px;
        }

        &--svg {
            position: absolute;
            bottom: 10%;
            right: 10%;
            width: 40vw;
        }
    }
</style>