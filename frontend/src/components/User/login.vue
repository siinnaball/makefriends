<template>
    <div>
        <p>用戶登入</p>
    </div>

    <div>
        <div>

            <div>
                <input type="text" id="logIn-text" name="logIn-text" placeholder="用戶名稱(6-20字元)" minlength="6" maxlength="20"
                    required v-model="email">
            </div>

            <div>
                <input :type="showPassword ? 'text' : 'password'" id="logIn-password" name="logIn-password" placeholder="密碼"
                    minlength="4" maxlength="15" required v-model="password">

                <button @click="showPassword = !showPassword">
                    <i v-if="!showPassword" class="fas fa-eye-slash"></i>
                    <i v-else class="fas fa-eye"></i>
                </button>
            </div>
        </div>

        <div>
            <button type="button" @click="loginClick">登入</button>
        </div>

        <div>

            <RouterLink to="/register">還不是會員?</RouterLink>

        </div>
    </div>
</template>


<style lang="scss" scoped></style>



<script>
// import { useUserStore } from '@/stores/user.js'




</script>
