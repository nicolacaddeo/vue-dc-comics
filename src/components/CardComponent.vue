<template>
  <div id="card">
    <img :src="imgUrl" >
    <div class="card-info">
        <h4>{{ title }}</h4>
        <span class="subtitle">{{ subTitle }}</span>
        <span>{{ price }}</span>
    </div>
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
    flex-direction: column;
    width: calc(100% / 6 - 2rem);
    margin: 1rem;
    img {
       width: 200px;
       height: 200px;
    }
    h1 {
        color: white;
    }
    .card-info {
        padding-top: .7rem;
        h4 {
            margin-bottom: .3rem;
        }
        .subtitle {
            text-transform: capitalize;
            margin-right: 1rem;
        }
        
    }
}
    
</style>

