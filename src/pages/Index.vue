<template data-v-app>
    <!-- hero section  -->

    <section 

                v-motion :initial="{ opacity: 0, x: -100 }" 
    :enter="{ opacity: 1, x: 0, transition: { delay: 1000, duration: 1000 } }"
    class=" mx-auto px-10 md:px-56">

        <div class="flex flex-col justify-center font-playfair-display font-bold uppercase">
            <div 
            class="flex flex-row justify-center me-[10rem] md:me-[50rem]">
                <p class="font-medium font-archivo text-sm md:text-2xl">HEY! I'm <span
                        class="text-neutral-100 bg-[#C50000] px-1 ms-1">MITCH.</span></p>
            </div>
            <div 

            
            class="flex flex-col justify-center items-center">
                <h1 class="text-[2rem] md:text-[6rem] text-[#1b1b1b] ">Full Stack</h1>
                <div class="w-56 md:w-[55rem] h-0.5 bg-neutral-900 mx-auto"></div>
                <h1 class="text-[2rem] md:text-[6rem] text-[#ED1B24] ">Web Developer</h1>
            </div>
        </div>
        <div 
        class="text-center">
            <h2 class="text-md md:text-2xl text-neutral-500 font-karla">From Bacolod City, Philippines</h2>
            <div class="flex flex-col md:flex-row justify-center items-center gap-5 mt-10">
                <p class="font-archivo md:font-bold uppercase text-[12px] md:text-lg ">Learn more about me</p>
                <a href="#about"
                    class=" uppercase border-0 bg-neutral-900 hover:bg-red-600 transition hover:shadow-2xl hover:scale-110
                    duration-300 ease-in-out px-5 py-1 md:px-10 md:py-2 rounded-full font-medium  text-neutral-100 text-[12px] md:text-lg">Let's
                    go!</a>
            </div>
        </div>
    </section>

    <!-- about me -->
    <div v-motion :initial="{ opacity: 0, y: 50 }" 
    :enter="{ opacity: 1, y: 0, transition: { delay: 1500, duration: 500 } }">
        <div class="flex flex-col justify-center text-center mt-20 md:mt-40">
            <i class="fa-solid fa-xmark text-[#ED1B24]"></i>
            <div class="h-10 md:h-20 w-0.5 bg-neutral-900 mx-auto mt-4 rounded"></div>
        </div>
    </div>


    <section id="about" class="flex justify-center pt-20 md:pt-40">

        <div class="flex flex-col md:flex-row"
         v-motion-slide-visible-once-left 
    :variants="customVariants"
        >

            <div class="flex flex-col font-archivo  z-12 md:me-[-150px]">
                <h1 class="text-2xl md:text-[4rem] text-neutral-800 font-medium">ABOUT ME:</h1>
                <h1 class="text-2xl md:text-[4rem] text-[#ED1B24] font-bold">MITCH BARCENILLA.</h1>
                <div class="h-2 w-20 md:h-4 md:w-52 bg-neutral-800"></div>

                <div class="mt-10 font-archivo text-lg w-56 md:w-96 leading-10">
                    <p class=""> I enjoy creating visually appealing web designs and developing user-friendy software
                        solutions.
                        <br><br>
                        Outside of work, I read novels, exercise, brainstorm new ideas for my start up brand, and spend
                        time with my family.
                    </p>
                </div>
            </div>

            <div class="flex flex-row items-center mt-10 md:mt-auto">
                <div class="h-40 w-20 md:h-72 md:w-36 bg-red-600 rounded-tl-full rounded-bl-full ">
                </div>
                <img src="/images/Mitch-B&W.jpg" class="w-40 md:w-92 ms-[-40px] z-10"
                    alt="Mitch dressed in black in black and white filter">

            </div>

        </div>

    </section>


    <!-- experience -->
    <section id="experience" class="pt-40">

        <div class="flex flex-row items-center justify-center  gap-2 md:gap-5 ms-40 md:ms-[50rem] mb-20 md:mb-40">
            <div class="w-1 h-5 md:w-5 md:h-16 bg-[#ED1B24] -skew-x-24"></div>
            <h1 class="text-2xl md:text-[4rem] font-bold font-archivo uppercase">Experience</h1>
        </div>

        <!-- project -->
        <div class="flex flex-col md:flex-row justify-center items-center gap-20 mb-40">
            <!-- images alternate "placement" for column and row layout-->
            <img class="w-40 md:w-96 md:hidden block"
                src="https://scontent.fmnl9-2.fna.fbcdn.net/v/t39.30808-6/441283863_122143332830203750_7425556550832358537_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeHMSMz1-SVudV2wpy0IQ_kK1y_dU9UUqZzXL91T1RSpnLmBg7cVvid7Pv-vd0xG8sPcHc7E__U6eGQCIaKUXOgr&_nc_ohc=9_fLojN8-ZgQ7kNvgGxYAJ_&_nc_oc=AdjZE8BJgrgpKW0_BSwmEojRMU8P464DgFvT9pP5hWJt57qqSAdvW0GlKluXsa-mne8&_nc_zt=23&_nc_ht=scontent.fmnl9-2.fna&_nc_gid=A579mM4OLykO0LYGKHwML9c&oh=00_AYETcFBZP_8xp65qO8y6gZycYnGXkz0n7D0SmppDzmlW5A&oe=67D58261"
                alt="">

            <div>
                <h2 class="text-xl md:text-[3rem] font-medium font-archivo mb-2">MORSEBIT</h2>
                <p class="text-neutral-700 leading-6 text-sm md:text-md"> In VUE is a product showcase website for
                    <br>my techincal accessories startup brand.
                </p>
                <div class="mt-10 flex justify-center md:justify-start ">
                    <a href="https://morsebit.vercel.app/"
                        class=" uppercase border-0 bg-neutral-900 hover:bg-red-600 transition duration-300 hover:shadow-2xl 
                        ease-in-out px-5 py-1 md:px-10 md:py-2 rounded-full font-medium  text-neutral-100 text-[12px] text-[16px]">See for yourself</a>
                </div>

            </div>
            <!-- images alternate "placement" for column and row layout-->
            <img class="w-40 md:w-96 hidden md:block"
                src="https://scontent.fmnl9-2.fna.fbcdn.net/v/t39.30808-6/441283863_122143332830203750_7425556550832358537_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeHMSMz1-SVudV2wpy0IQ_kK1y_dU9UUqZzXL91T1RSpnLmBg7cVvid7Pv-vd0xG8sPcHc7E__U6eGQCIaKUXOgr&_nc_ohc=9_fLojN8-ZgQ7kNvgGxYAJ_&_nc_oc=AdjZE8BJgrgpKW0_BSwmEojRMU8P464DgFvT9pP5hWJt57qqSAdvW0GlKluXsa-mne8&_nc_zt=23&_nc_ht=scontent.fmnl9-2.fna&_nc_gid=A579mM4OLykO0LYGKHwML9c&oh=00_AYETcFBZP_8xp65qO8y6gZycYnGXkz0n7D0SmppDzmlW5A&oe=67D58261"
                alt="">
        </div>
        <!--  -->

        <!-- project -->
        <div class="flex flex-col md:flex-row justify-center items-center gap-20 mb-40">
            <img class="w-40 md:w-96"
                src="https://scontent.fmnl9-2.fna.fbcdn.net/v/t39.30808-6/441283863_122143332830203750_7425556550832358537_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeHMSMz1-SVudV2wpy0IQ_kK1y_dU9UUqZzXL91T1RSpnLmBg7cVvid7Pv-vd0xG8sPcHc7E__U6eGQCIaKUXOgr&_nc_ohc=9_fLojN8-ZgQ7kNvgGxYAJ_&_nc_oc=AdjZE8BJgrgpKW0_BSwmEojRMU8P464DgFvT9pP5hWJt57qqSAdvW0GlKluXsa-mne8&_nc_zt=23&_nc_ht=scontent.fmnl9-2.fna&_nc_gid=A579mM4OLykO0LYGKHwML9c&oh=00_AYETcFBZP_8xp65qO8y6gZycYnGXkz0n7D0SmppDzmlW5A&oe=67D58261"
                alt="">

            <div>
                <h2 class="text-xl md:text-[3rem] font-medium font-archivo mb-2">MABINI FARM SCHOOL</h2>
                <p class="text-neutral-700 leading-6 text-sm md:text-md"> A functional web application built for the
                    Mabinians.</p>
                <div class="mt-10 flex justify-center md:justify-start ">
                    <a href="https://morsebit.vercel.app/"
                        class=" uppercase border-0 bg-neutral-900 hover:bg-red-600 transition duration-300 hover:shadow-2xl 
                        ease-in-out px-5 py-1 md:px-10 md:py-2 rounded-full font-medium  text-neutral-100 text-[12px] text-[16px]">Read more</a>
                </div>

            </div>
        </div>
        <!--  -->

        <!-- project -->
        <div class="flex flex-col md:flex-row justify-center items-center gap-20">
            <!-- images alternate "placement" for column and row layout-->
            <img class="w-40 md:w-96 md:hidden block"
                src="https://scontent.fmnl9-2.fna.fbcdn.net/v/t39.30808-6/441283863_122143332830203750_7425556550832358537_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeHMSMz1-SVudV2wpy0IQ_kK1y_dU9UUqZzXL91T1RSpnLmBg7cVvid7Pv-vd0xG8sPcHc7E__U6eGQCIaKUXOgr&_nc_ohc=9_fLojN8-ZgQ7kNvgGxYAJ_&_nc_oc=AdjZE8BJgrgpKW0_BSwmEojRMU8P464DgFvT9pP5hWJt57qqSAdvW0GlKluXsa-mne8&_nc_zt=23&_nc_ht=scontent.fmnl9-2.fna&_nc_gid=A579mM4OLykO0LYGKHwML9c&oh=00_AYETcFBZP_8xp65qO8y6gZycYnGXkz0n7D0SmppDzmlW5A&oe=67D58261"
                alt="">

            <div>
                <h2 class="text-xl md:text-[3rem] font-medium font-archivo mb-2">ROBOok</h2>
                <p class="text-neutral-700 leading-6 text-sm md:text-md"> Robotics e-book for Junior High School
                    Students.</p>
                <div class="mt-10 flex justify-center md:justify-start ">
                    <a href="https://robook.vercel.app/"
                        class=" uppercase border-0 bg-neutral-900 hover:bg-red-600 transition duration-300 hover:shadow-2xl 
                        ease-in-out px-5 py-1 md:px-10 md:py-2 rounded-full font-medium  text-neutral-100 text-[12px] text-[16px]">See for yourself</a>
                </div>

            </div>
            <!-- images alternate "placement" for column and row layout-->
            <img class="w-40 md:w-96 hidden md:block"
                src="https://scontent.fmnl9-2.fna.fbcdn.net/v/t39.30808-6/441283863_122143332830203750_7425556550832358537_n.jpg?_nc_cat=101&ccb=1-7&_nc_sid=6ee11a&_nc_eui2=AeHMSMz1-SVudV2wpy0IQ_kK1y_dU9UUqZzXL91T1RSpnLmBg7cVvid7Pv-vd0xG8sPcHc7E__U6eGQCIaKUXOgr&_nc_ohc=9_fLojN8-ZgQ7kNvgGxYAJ_&_nc_oc=AdjZE8BJgrgpKW0_BSwmEojRMU8P464DgFvT9pP5hWJt57qqSAdvW0GlKluXsa-mne8&_nc_zt=23&_nc_ht=scontent.fmnl9-2.fna&_nc_gid=A579mM4OLykO0LYGKHwML9c&oh=00_AYETcFBZP_8xp65qO8y6gZycYnGXkz0n7D0SmppDzmlW5A&oe=67D58261"
                alt="">
        </div>
        <!--  -->
    </section>

    <!-- contact me -->
    <section id="contact" class="py-40">
        <div class="flex flex-col items-center justify-center me-40 md:me-[50rem] mb-20 md:mb-40">
            <h1 class=" text-2xl md:text-[4rem] font-bold font-archivo uppercase">contact me</h1>
            <div class="h-0.5 md:h-1 w-32 md:w-96 bg-[#ED1B24]"></div>
            <div class="flex flex-row gap-5">
                <p>+</p>
                <p>+</p>
                <p>+</p>
            </div>
        </div>

        <div class=" flex flex-col md:flex-row gap-10 md:gap-20 mx-10 md:mx-auto items-start md:justify-center
            md:items-center ">
            <div class="flex flex-col">
                <a id="email" href="mailto:mitchbarcenilla4@gmail.com"
                    class="ms-5 hover:text-[#ED1B24] transition duration-150"><i class="fa-regular fa-envelope"></i>
                    mitchbarcenilla4@gmail.com</a>
            </div>
            <div class="flex flex-col">
                <a href="https://www.facebook.com/0100.010O/"
                    class="ms-5 hover:text-[#ED1B24] transition duration-150"><i
                        class="fa-brands fa-square-facebook"></i> Mitch Barcenilla</a>
            </div>
            <div class="flex flex-col">
                <a href="https://www.instagram.com/imytchyou/"
                    class="ms-5 hover:text-[#ED1B24] transition duration-150"><i class="fa-brands fa-instagram"></i>
                    imytchyou</a>
            </div>
            <div class="flex flex-col">
                <a href="https://github.com/Mitchap" class="ms-5 hover:text-[#ED1B24] transition duration-150"><i
                        class="fa-brands fa-square-github"></i> Mitchap</a>
            </div>
        </div>

        <div class="flex flex-col relative border-1 border-neutral-400 w-20 h-20 md:w-52  md:h-52 mx-auto -mt-20 -z-20">
            <div class="absolute border-1 border-neutral-400 w-20 h-20 md:w-52  md:h-52 bottom-[20px] left-[20px]"></div>
        </div>
    </section>

</template>

<script>
import { MotionDirective as motion } from '@vueuse/motion'

export default {
  directives: {
    motion: motion(),
  },
}
const customVariants = {
  visibleOnce: {
    enter: {
      transition: {
        duration: 2000, // 2 seconds
      },
    },
  },
};

</script>

<style></style>