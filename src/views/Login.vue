<template>
    <div style="">
        <div class="input-group">
            <label>Username</label>
            <input type="text" v-model="username">
        </div>       
        
        <div class="input-group">
            <label>Password</label>
            <input type="password" v-model="password">
        </div>
        
        <button type="button" v-on:click="login">Login</button>
      <router-link to="/about">เกี่ยวกับเรา</router-link>

    </div>
</template>

<script>
    import axios from 'axios'
    import { loginUser } from '../utils/auth'

    export default {
        name: 'login',
        data() {
            return {
                username: '',
                password: ''
            }
        },
        methods: {
            async login() {
                try {
                    await loginUser(this.username, this.password)
                    this.$router.push('/')
                } catch (err) {
                    alert(`Error: ${err}`)                    
                }
            }
        }
    }
</script>

<style>
    .input-group {
        margin: 1rem;
    }

    .input-group label {
        margin-right: 0.5rem;
    }
</style>

