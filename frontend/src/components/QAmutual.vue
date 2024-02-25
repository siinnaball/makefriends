<template>
    <input type="number" v-model="total" class="border-solid border-4 border-indigo-500/100">

    <div class="flex flex-wrap place-content-center mx-24">

        <div v-for="num in total" :key="num" class="QAcard-style">

            <div class="bg-red-200 h-7"> </div>

            <div class="p-3 flex flex-col justify-between h-full">

                <div class="leading-tight tracking-wider mb-4">QQ問問問問QQQQ問問QQQQ問問QQQQQQQQ</div>

                <div class="flex flex-col justify-between h-full">

                    <div class="mb-3">
                        <div class="mb-1">AAAA</div>
                    </div>


                    <div v-if="clearance" class="submit-btn">
                        <button class=" bg-blue-100 active:bg-blue-600 ">
                            Submit
                        </button>
                    </div>



                </div>

            </div>

        </div>

    </div>
</template>

<script setup>
import { ref } from 'vue';

const total = ref(0);
const clearance = ref(false);
</script>


<style lang="scss">
.QAcard-style {
    @apply bg-pink-100 basis-72 min-h-24 break-all flex flex-col m-2;
}

.submit-btn {
    @apply flex place-content-center
}
</style>

