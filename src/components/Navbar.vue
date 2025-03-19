<template>

    <!-- big screen navbar -->
    <div>
        <nav class="bg-neutral-50  px-10 py-7 fixed top-o w-screen z-99 ">
            <div class="flex flex-row justify-between" v-motion :initial="{ opacity: 0, y: -100 }"
                :enter="{ opacity: 1, y: 0, transition: { delay: 200, duration: 1000 } }">

                <a href="#"><img src="/images/Mitch-Logo.jpg" alt="Mitch Barcenilla Logo" class="w-52"></a>
                <ul class="flex flex-row gap-10 font-archivo font-medium">

                    <li><a href="#" class="hover-slider">Home</a></li>
                    <li><a href="#about" class="hover-slider">About</a></li>
                    <li><a href="#experience" class="hover-slider">Experience</a></li>
                    <li><a href="#contact" class="hover-slider">Contact</a></li>
                    <li><a href="#" class="hover-slider">Resume <i
                                class="fa-solid fa-arrow-up-right-from-square text-sm ms-1"></i></a></li>
                </ul>
            </div>
        </nav>
    </div>

</template>


<script>


</script>