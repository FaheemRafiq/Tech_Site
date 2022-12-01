<script>
export default {
props:{
    name:String,
    blue:Boolean
}
}
</script>

<template>
   <button class="uppercase py-2 px-5 rounded-md text-white bg-[#DB2877] hover:bg-white hover:text-black hover:transition-all hover:duration-500" :class="{'bg-[#5267DF]': blue == true}">
          {{name}}
    </button>
</template>