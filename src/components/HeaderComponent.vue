<template>
    <header>
        <div id="logo">
            <img src="../assets/img/dc-logo.png" alt="logo DC">
        </div>
        <div>
            <ul>
                <li v-for="item in headerLinks" :key="item in headerLinks">
                    {{ item.name }}
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
import {headerLinks} from '../data/header_links.js'

export default {
    name: 'HeaderComponent',
    data() {
        return {
            headerLinks
        }
    }
}
</script>

<style scoped lang="scss">
header {
    display: flex;
    height: 15vh;
    justify-content: space-around;
    align-items: center;
    width: 100%;
}

ul {
    list-style-type: none;
    li {
        text-transform: uppercase;
        display: inline-block;
        padding: 0 .7rem;
        font-size: .9rem;
        font-weight: bold;
        color: #474746;
        cursor: pointer;
        &:hover {
            color: #0282f9;
        }
    }
}
</style>
    
    
            