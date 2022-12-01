<script>
import ButtonVue from './Button.vue';
export default {
    components:{ButtonVue},
    props:{
        heading:String,
    },
    computed:{
        getSrc(){
            console.log(this.src);
        }
    },
};
</script>

<!-- * Content -->

<template>
  <div>
    <div class="text-white flex justify-center items-center mt-20">
      <div
        class="
          flex flex-col
          items-center
          lg:flex-row
          md:py-20
          lg:py-30 lg:px-20
        "
      >
        <div
          class="
            text-center
            lg:text-left
            py-10
            order-2
            lg:order-2
            w-9/12
            md:w-1/3
          "
        >
          <h1 class="text-3xl font-bold text-gray-200 pb-4">
            {{heading}}
          </h1>
          <!-- ? Defalut Slot -->
          <span>
              <slot name="content"></slot>
          </span>
        </div>
        <div class="w-1/2 flex justify-center lg:order-1">
            <!-- ? Image Slot -->
          <slot name="image"></slot>
        </div>
        <!-- todo Bg black Color Mic -->
        <div
          class="
            absolute
            lg:w-[40%]
            h-80
            -translate-x-20
            translate-y-32
            bg-black
            rounded-tr-full rounded-br-full
          "
        ></div>
      </div>
    </div>
  </div>
</template>
