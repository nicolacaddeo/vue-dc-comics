<template>
  <div id="card">
    <img :src="imgUrl" >
    <h1>{{ title }}</h1>
    <span>{{ subTitle }}</span>
    <span>{{ price }}</span>
  </div>
</template>

<script>
export default {
    name: 'CardComponent',
    props: {
        imgUrl: String,
        price: String,
        title: String,
        subTitle: String
    }
    
}
</script>

<style scoped lang="scss">
#card {
    display: flex;
    img {
        width: 150px;
        height: 150px;
    }
    h1 {
        color: white;
    }
}
    
</style>

