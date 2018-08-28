<template>
        <form id="login-comp">
        <h1>{{ CompanyName }}</h1>
        <input type="text" placeholder="username">
        <input type="text" placeholder="password">
        <button @click="login()"> Login</button>
        <router-link to='/register'>Dont have an Account?</router-link>
        </form>
</template>

<script>
export default {
    name: 'login',
    data () {
        return {
            CompanyName: 'Truck Stop'

        }
    },
    mounted () {

    },
    methods: {
        login () {
            this.$router.push('/home')
        }
    },
    computed: {

    }
}
</script>

<style scoped lang="scss">
    @import url('https://fonts.googleapis.com/css?family=Do+Hyeon');
    @import url('https://fonts.googleapis.com/css?family=Montserrat');
        #login-comp {
        align-self: center;
        font-family: 'Do Hyeon', sans-serif;
        width: 425px;
        height: 400px;
        background: #ecf0f1;  /* fallback for old browsers */
        border-radius: 5px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin: 10px;
        h1 {
            align-self: center;
            font-size: 62px;
            font-weight: 800;
            color: white;
        }
        input {
            background-color: white;
            color: rgb(121, 121, 121);
            // border-bottom:1px solid #00BFA5;
            // border: 0;
            font-family: 'Montserrat', sans-serif;
            font-size: 24px;
            font-weight: 200;
            align-self: center;
            text-align: center;
            width: 90%;
            height:30px;
            border-radius: 4px;
            padding: 20px 5px;
            margin: 15px 0px;
            }
            input:focus {
            border-color:  rgb(75, 74, 74);
            box-shadow: 2px 4px rgb(199, 199, 199);
            }
        button {
            border: none;
            font-family: 'Montserrat', sans-serif;
            font-size: 24px;
            font-weight: 200;
            color: white;
            background-color: #00BFA5;
            align-self: center;
            width: 50%;
            border-radius: 4px;
            margin: 25px 10px;
        }
        button:hover {
            transform: translate(0, -2px);
        }
        a {
            font-family: inherit;
            align-self: center;
        }
    }
</style>