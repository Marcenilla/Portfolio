<template>
    <div class="flex justify-center h-screen preloader">


        <div class="loader"></div>

    </div>
</template>

<script>

//  loading process
window.addEventListener("load", () => {
    const loader = document.querySelector(".preloader");

    loader.classList.add("preloader--hidden");


});
</script>

<style>
.preloader {
    background: #1b1b1b center;
    height: 100vh;
    width: 100%;
    position: fixed;
    z-index: 99999;
}

.preloader--hidden {
    transition: ease-out 300ms;
    transition-delay: 600ms;
    opacity: 0.5;
    visibility: hidden;
}

.loader {
    position: relative;
    display: flex;
    align-items: start;
    justify-content: center;
    max-width: 6rem;
    margin-top: 3rem;
    margin-bottom: 3rem;
    width: 48px;
    height: 48px;
    margin: auto;
    background: #ff0202;
    transform: rotateX(65deg) rotate(45deg);
    color: #fff;
    animation: layers1 1s linear infinite alternate;
}

.loader:after {
    content: '';
    position: absolute;
    inset: 0;
    background: rgba(255, 255, 255, 0.7);
    animation: layerTr 1s linear infinite alternate;
}

@keyframes layers1 {
    0% {
        box-shadow: 0px 0px 0 0px
    }

    90%,
    100% {
        box-shadow: 20px 20px 0 -4px
    }
}

@keyframes layerTr {
    0% {
        transform: translate(0, 0) scale(1)
    }

    100% {
        transform: translate(-25px, -25px) scale(1)
    }
}
</style>