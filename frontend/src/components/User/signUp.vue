<template>
    123132
    <p>註冊</p>
    <!--  <div class="signUp-in">


        <div class="signUp-name">
            <input type="text" id="signUp-text" name="signUp-text" placeholder="用戶名稱(6-12字元)" minlength="6" maxlength="12"
                v-model="name.nameInput" required>
        </div>

        <div class="show-error" v-show="name.errorMsg">
            <p>已經有人用了</p>
        </div>

        <div class="signUp-mail">
            <input type="email" id="signUp-email" name="signUp-email" placeholder="信箱" required v-model="email.emailInput">
        </div>

        <div class="show-error" v-show="email.errorMsg">
            <p>已經被註冊過</p>
        </div>

        <div class="signUp-password">
            <input type="text" id="signUp-password" name="signUp-password" placeholder="密碼" minlength="4" maxlength="20"
                required v-model="password.passwordInput">
        </div>


        <div class="signUp-password-check">
            <input type="text" id="signUp-password-check" name="signUp-password-check" placeholder="確認密碼" minlength="4"
                maxlength="20" required v-model="password.passwordCheck">
        </div>

        <div class="show-error" v-show="password.errorMsg">
            <p>密碼不一致</p>
        </div>



    </div>

    <div class="signUp-backtop">
        <button type="button" @click="signUp">送出</button>
    </div>

    <div class="goToLogin">

        <button type="button" @click="$router.push({ name: 'logIn' })">
            前往登入
        </button>
    </div> -->
</template>

<style scoped></style>

<script>

// import axios from 'axios'

// export default {
//     data() {
//         return {
//             DesktopKv,
//             name: {
//                 nameInput: '',
//                 errorMsg: '',
//                 nameError: true,
//             },
//             email: {
//                 emailInput: '',
//                 errorMsg: '',
//                 emailError: true,
//             },
//             password: {
//                 passwordInput: '',
//                 passwordCheck: '',
//                 errorMsg: '',
//                 passwordError: true,
//             },
//             avatar: 'https://picsum.photos/640/640?r=6732',
//         }
//     },

//     methods: {
//         async signUp() {
//             if (this.password.passwordInput !== this.password.passwordCheck) {
//                 this.password.errorMsg = '密碼不一致，請重新輸入'
//                 return
//             }
//             const userRegister = {
//                 name: this.name.nameInput,
//                 email: this.email.emailInput,
//                 password: this.password.passwordInput,
//                 avatar: this.avatar,
//             }
//             try { //嘗試做
//                 if (this.name.nameError && this.email.emailError && this.password.passwordError) {
//                     await axios.post('https://api.escuelajs.co/api/v1/users/', userRegister)

//                 } else {
//                     alert('註冊失敗，請檢查是否有相同名稱')

//                 }
//             } catch (err) {
//                 console.dir('註冊失敗', err)
//             }
//         }
//     },

//     watch: {
//         async 'name.nameInput'(nowName) { //找全部的api，比對name
//             const nameAPI = await axios.get('https://api.escuelajs.co/api/v1/users')
//             const nameIf = nameAPI.data.some(user => user.name === nowName)
//             if (nameIf) {
//                 this.name.errorMsg = '已經有人用了'
//                 this.name.nameError = false
//             } else {
//                 this.name.errorMsg = ''
//                 this.name.nameError = true
//             }
//         },
//         async 'email.emailInput'(nowEmail) { //專用api，看返回的布林值
//             this.email.errorMsg = ''
//             const checkMail = await axios.post('https://api.escuelajs.co/api/v1/users/is-available', { email: nowEmail })
//             if (!checkMail.data.isAvailable) {
//                 this.email.errorMsg = '已經被註冊過'
//                 this.email.emailError = false
//                 if (nowEmail != this.email.emailInput) {
//                     this.email.errorMsg = ''
//                     this.email.emailError = true
//                 }
//             }
//         },
//         'password.passwordInput'() { //檢查是否與password一致
//             if (this.password.passwordInput !== this.password.passwordCheck) {
//                 this.password.errorMsg = '密碼不一致，請重新輸入'
//                 this.password.passwordError = false
//                 console.log(this.password.passwordError)
//             } else {
//                 this.password.errorMsg = ''
//                 this.password.passwordError = true
//                 console.log(this.password.passwordError)
//             }
//         },
//         'password.passwordCheck'() { //檢查是否與password一致
//             if (this.password.passwordInput !== this.password.passwordCheck) {
//                 this.password.errorMsg = '密碼不一致，請重新輸入'
//                 this.password.passwordError = false
//                 console.log(this.password.passwordError)
//             } else {
//                 this.password.errorMsg = ''
//                 this.password.passwordError = true
//                 console.log(this.password.passwordError)
//             }
//         }
//     },

// }
</script>
