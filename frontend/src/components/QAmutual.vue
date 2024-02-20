<template>
    <input type="number" v-model="num" class="border-solid border-4 border-indigo-500/100">
    <div class="flex flex-wrap place-content-center">

        <div class="QAcard-style">

            <div class="bg-red-200 h-7"> </div>

            <div class="p-3 flex flex-col justify-between h-full">

                <div class="leading-tight tracking-wider mb-4">QQ問問問問QQQQ問問QQQQ問問QQQQQQQQ</div>

                <div class="flex flex-col justify-between h-full">

                    <div class="mb-3">
                        <div class="mb-1">AAAA</div>
                    </div>


                    <div class="submit-btn ">
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



</script>


<style lang="scss">
.QAcard-style {
    @apply bg-pink-100 basis-72 min-h-48 break-all flex flex-col m-2;
}

.submit-btn {
    @apply flex place-content-center
}
</style>

