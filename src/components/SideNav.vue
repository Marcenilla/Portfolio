<template>
    <div>
        <nav class="bg-neutral-50 flex flex-row justify-between items-center px-10 py-7 fixed top-0 w-screen z-80">
            <a href="#"><img src="/images/Mitch-Logo.jpg" alt="Mitch Barcenilla Logo" class="w-40" /></a>
            <div class="icon z-82">
                <button type="button" @click="toggleSideNav" class="relative w-10 h-10 flex items-center justify-center">
                    <transition name="icon-fade" mode="out-in">
                        <i v-if="mobileNav" key="bars-staggered" class="fa-solid fa-bars-staggered"></i>
                        <i v-else key="bars" class="fa-solid fa-bars"></i>
                    </transition>
                </button>
            </div>

            <div v-show="mobileNav"
                class="fixed flex justify-start h-screen z-81 top-0 transition ease-in-out duration-150 w-64 mt-5 right-0 bg-white/30 backdrop-blur-sm overflow-x-hidden backdrop-blur-sm bg-white/30">
                <ul class="flex flex-col gap-10 font-archivo font-medium mt-20 mx-auto">
                    <li><a href="#" class="hover-slider">Home</a></li>
                    <li><a href="#about" class="hover-slider">About Me</a></li>
                    <li><a href="#experience" class="hover-slider">Experience</a></li>
                    <li><a href="#contact" class="hover-slider">Contact</a></li>
                    <li>
                        <a href="#" class="hover-slider">Resume
                            <i class="fa-solid fa-arrow-up-right-from-square text-sm ms-1"></i></a>
                    </li>
                </ul>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name: "navigation",
    data() {
        return {
            scrollPostion: null,
            windowWidth: null,
            mobileNav: false,
        };
    },
    methods: {
        toggleSideNav() {
            this.mobileNav = !this.mobileNav;
        },
    },
};
</script>

<style>
/* Smooth transition for icon change */
.icon-fade-enter-active, .icon-fade-leave-active {
    transition: opacity 0.3s ease, transform 0.3s ease;
}

.icon-fade-enter-from, .icon-fade-leave-to {
    opacity: 0;
    transform: scale(0.8);
}
</style>
