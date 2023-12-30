<template>
    <div class="flex py-12 px-16 justify-center antialiased">
        <!-- 横着两个部分 -->
        <div class="flex max-w-[1140px] min-w-60  md:flex-row sm:flex-col">
            <!-- 左侧 -->
            
            <div class="sm:w-full md:w-1/2 flex flex-col">
                <div class="flex justify-center">
                    <img class="w-72 rounded-md" :src="picture" />
                </div>
                <div class="flex">
                    <img class="w-8" :src="barista_picture" />

                    <div> Barista</div>
                </div>
            </div>
            <!-- 右侧 -->
            <div class="sm:w-full md:w-1/2 pt-10 px-4">
                <span class="font-medium text-[28px] pgray">Hello There !</span>
                <p class="font-normal text-base text-justify mb-4" v-html="info.description"></p>
                <p class="font-normal text-base text-justify" v-html="info.description_further"></p>
                <div class="text-center pb-4">
                    <button
                    class="btn btn-outline-secondary mx-2 "
                    @click="open('linkedin')"
                    v-tooltip.bottom="'LinkedIn'"
                    >
                    <i class="fab fa-linkedin"></i>
                    </button>
                    <button
                    class="btn btn-outline-secondary mx-2"
                    @click="open('github')"
                    v-tooltip.bottom="'GitHub'"
                    >
                    <i class="fab fa-github"></i>
                    </button>
                    <button
                    
                    class="btn btn-outline-secondary mx-2"
                    @click="open('googlescholar')"
                    v-tooltip.bottom="'Google Scholar'"
                    >
                    <i class="fab fa-google"></i>
                    </button>
                    <button
                    class="btn btn-outline-secondary mx-2"
                    @click="open('resume')"
                    v-tooltip.bottom="'Resume'"
                    >
                    <i class="fa fa-file"></i>
                    </button>
                </div>
            
            
            
            
            
            
            </div>
        </div>




    </div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue';
defineProps({
    nightMode: Boolean
})
const getImageUrl = (name:string) => {
        return new URL(`${name}`, import.meta.url).href
    }


// data
import info from "../../info";
// let picture = info.flat_picture
let picture = "../../src/assets/photo.png"
let barista_picture = "../../src/assets/barista.jpg"



</script>



<style scoped>

/* .person{
    width: 100%;
    height: 100%;
    background-color: red;} */

</style>

<style>
a{
    color: #669db3ff;
}

</style>