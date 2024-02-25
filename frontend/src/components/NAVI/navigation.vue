<template>
    <div class="flex justify-between  px-52 w-full">

        <div>
            <RouterLink :to="'/'" class="login-btn bg-emerald-200"> 這裡回首頁 </RouterLink>
        </div>

        <div class="flex">
            <RouterLink :to="'/'" class="login-btn  bg-emerald-400 hover:bg-emerald-500 hover:text-white"> 登入
            </RouterLink>
            <RouterLink :to="'/'" class="login-btn bg-slate-400 hover:bg-slate-300"> 註冊 </RouterLink>
        </div>

    </div>
</template>

<script setup>
import { ref } from 'vue';

</script>


<style lang="scss">
.login-btn {
    @apply mx-4 px-6 py-2 rounded-lg
}
</style>

