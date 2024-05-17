<script setup>

import {ref} from 'vue'

const clickear = ref(true)

function clic () {

    clickear.value = !clickear.value
}


</script>

<template> 

    <div class="flex text-center max-w-[750px] py-2 gap-[625px] mx-auto rounded-xl my-5 bg-gray-200 text-black"
    :class="{'bg-slate-400 text-white' : !clickear }" >
        <div class="pl-4 font-semibold">
            Tema 1
        </div>
        <button @click="clic" class="text-2xl font-bold hover:bg-gray-500 bg-slate-300 w-6 rounded-lg" >
            +
        </button>
    </div>
</template>