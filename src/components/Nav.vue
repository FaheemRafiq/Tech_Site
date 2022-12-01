<script>
import ButtonVue from './Button.vue';
export default {
    components:{
        ButtonVue,
    },
    props:{
        display:Boolean,
    }
}
</script>

<!-- Content Section -->

<template>
    <div v-if="display" class="fixed top-0 right-0 bg-blue-600 h-full w-full text-white z-50">
        <div  class="flex px-10 h-2/3 flex-col">
            <div class="self-end pt-4 relative left-5" >
                <button @click="$emit('close')">
                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-7 h-7">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                    </svg>
                </button>
            </div>
            <div class="flex flex-col items-center h-1/2 w-full">
                <nav class="flex flex-col justify-evenly h-full text-lg uppercase font-light">
                    <a href="#features" class="border-b-2 border-pink-500 hover:text-green-500 hover:font-bold">Features</a>
                    <a href="#pricing"  class="border-b-2 border-pink-500 hover:text-green-500 hover:font-bold">Pricing</a>
                    <a href="#contact"  class="border-b-2 border-pink-500 hover:text-green-500 hover:font-bold">Contact</a>
                </nav>
                <Button-vue name="login" blue="false" />
                <img class="pt-4" src="../assets/images/podcast.png" width="60" alt="Site Logo">
            </div>
        </div>
   </div>
</template>
