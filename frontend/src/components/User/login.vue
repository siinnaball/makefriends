<template>
    <div>
        <p>用戶登入</p>
    </div>

    <div class="logIn-box">

        <div class="logIn-in">

            <div class="logIn-data">
                <input type="text" id="logIn-text" name="logIn-text" placeholder="用戶名稱(6-20字元)" minlength="6" maxlength="20"
                    required v-model="email">
            </div>

            <div class="logIn-data">
                <input :type="showPassword ? 'text' : 'password'" id="logIn-password" name="logIn-password" placeholder="密碼"
                    minlength="4" maxlength="15" required v-model="password">

                <button @click="showPassword = !showPassword">
                    <i v-if="!showPassword" class="fas fa-eye-slash"></i>
                    <i v-else class="fas fa-eye"></i>
                </button>
            </div>
        </div>

        <div class="logIn-backtop">
            <button type="button" @click="loginClick">登入</button>
        </div>

        <div class="goToSingup">
            <button type="button" @click="$router.push({ name: 'signUp' })">
                <!-- <RouterLink to="/signUp">還不是會員?</RouterLink> -->
                還不是會員?
            </button>
        </div>
    </div>
</template>


<style lang="scss" scoped></style>



<script>
// import { useUserStore } from '@/stores/user.js'




</script>
