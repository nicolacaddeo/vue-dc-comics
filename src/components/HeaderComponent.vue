<template>
  <header>
    <div>
        <img src="../assets/img/dc-logo.png" alt="logo DC">
    </div>
    <div>
        <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Collectibles</li>
            <li>Videos</li>
            <li>Fans</li>
            <li>News</li>
            <li>Shop</li>
        </ul>
    </div>
  </header>
</template>

<script>
export default {
    name: 'HeaderComponent'
}
</script>

<style scoped lang="scss">
header {
    display: flex;
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