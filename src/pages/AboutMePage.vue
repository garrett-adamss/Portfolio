<template>
    <section class="container-fluid about-me">
        <div class="row">
            <h1 class="title">ABOUT ME</h1>
            <p class="body">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Iure deleniti temporibus modi eos
                facere, id qui dolorum, quos, assumenda placeat magni. Tempora, culpa sed. Esse magnam inventore
                explicabo maxime autem.</p>
        </div>
    </section>
</template>


<script>

export default {
    name: 'AboutMe',
    setup() {
        return {

        }
    }
}
</script>


<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Oswald&display=swap');

.title {
    font-family: 'Oswald', sans-serif;
    font-size: 150px;
    opacity: 8%;
}

.about-me {
    min-height: 120vh;
    position: relative;
}

.title {
    position: absolute;
    top: 30vh;
    right: 20px;
}

.body {
    position: absolute;
    top: 39vh;
    left: 900px;
}

//animation
:root * {
    /* Pause the animation */
    animation-play-state: paused;
    /* Bind the animation to scroll */
    animation-delay: calc(var(--scroll) * -1s);
    /* These last 2 properties clean up overshoot weirdness */
    animation-iteration-count: 1;
    animation-fill-mode: both;
}

section {
    padding: 0;
    margin: 0;
    min-height: 190vh;
    position: relative;
    background-color: rgb(139, 201, 228);
    animation: body 1s linear;
}

@keyframes section {
    to {
        background-color: rgb(19, 48, 97);
    }
}

.progress {
    height: 3px;
    width: 0%;
    background-color: #fff;
    position: relative;
    top: 0;
    left: 0;
    animation: progress 1s linear;
}

@keyframes progress {
    to {
        background-color: rgb(20, 255, 226);
        width: 100%;
    }
}
</style>