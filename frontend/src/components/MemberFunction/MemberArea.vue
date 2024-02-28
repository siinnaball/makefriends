<template>
    <div class="flex">
        <RouterLink :to="'/'" class="login-btn  bg-emerald-400 hover:bg-emerald-500 hover:text-white"> 聊天窗
        </RouterLink>
        <RouterLink :to="'/'" class="login-btn bg-slate-400 hover:bg-slate-300"> 會員專區 </RouterLink>
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

