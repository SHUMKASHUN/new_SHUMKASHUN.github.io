<template>
    <div>
        <nav class="">
            <div>
                <a
                class="navbar-brand"
                href="/"
                @click.prevent="$emit('scroll', 'home')"
                >
                <Logo :nightMode=false />
                </a> 
            </div>
        </nav>
    </div>
</template>


<script setup lang="ts">
import Logo from './Navbar_comp/Logo.vue'

</script>