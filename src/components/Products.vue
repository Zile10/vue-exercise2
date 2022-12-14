<template>
  <div id="cards-holder">
    <div class="card" style="width: 18rem" v-for="item in products" :key="item">
      <img :src="item.imageSrc" class="card-img-top" :alt="item.itemName" />
      <div class="card-body">
        <h5 class="card-title">{{item.itemName}}</h5>
        <p class="card-text">
          <span v-text="'Price: R' + item.price"></span><br>
          <span v-text="'Color: ' + item.color"></span>
          <!-- <span v-text="` + ${item.color}`"></span>
          <span v-text="'' + item"></span> -->
        </p>
        <button href="#" class="btn btn-primary">Button</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      products: [
        {
          itemName: "men's cotton tshirt blue",
          price: 199,
          stock: 100,
          color: "blue",
          gender: "male",
          imageSrc: "https://i.postimg.cc/ncCCNvGM/mens-cotton-tshirt-blue.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "men's cotton tshirt white",
          price: 199,
          stock: 100,
          color: "white",
          gender: "male",
          imageSrc:
            "https://i.postimg.cc/rFmrM6MV/mens-cotton-tshirt-white.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "men's leather jacket black",
          price: 2699,
          stock: 100,
          color: "black",
          gender: "male",
          imageSrc:
            "https://i.postimg.cc/pTRmS4st/mens-leather-jacket-black.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "men's leather jacket brown",
          price: 2499,
          stock: 100,
          color: "brown",
          gender: "male",
          imageSrc:
            "https://i.postimg.cc/FRpYXp6k/mens-leather-jacket-brown.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "women's denim top blue",
          price: 129,
          stock: 100,
          color: "blue",
          gender: "female",
          imageSrc: "https://i.postimg.cc/8P0rCyzh/womens-denim-top-blue.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "women's leather jacket black",
          price: 2699,
          stock: 100,
          color: "black",
          gender: "female",
          imageSrc:
            "https://i.postimg.cc/SK026J8R/womens-leather-jacket-black.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "women's leather jacket brown",
          price: 2699,
          stock: 100,
          color: "brown",
          gender: "female",
          imageSrc:
            "https://i.postimg.cc/MGycdqbD/womens-leather-jacket-brown.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "men's cotton trousers cream",
          price: 599,
          stock: 100,
          color: "white",
          gender: "male",
          imageSrc:
            "https://i.postimg.cc/wxW1WWJS/mens-cotton-trousers-cream.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "men's cotton trousers tan",
          price: 599,
          stock: 100,
          color: "brown",
          gender: "male",
          imageSrc:
            "https://i.postimg.cc/RhbqNF4M/mens-cotton-trousers-tan.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "men's track pants grey",
          price: 199,
          stock: 100,
          color: "grey",
          gender: "male",
          imageSrc: "https://i.postimg.cc/RZJJJcW2/mens-track-pants-grey.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "women's palazzo pants azure",
          price: 479,
          stock: 100,
          color: "blue",
          gender: "female",
          imageSrc:
            "https://i.postimg.cc/HnLVY5GZ/womens-palazzo-pants-azure.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
        {
          itemName: "women's track pants black",
          price: 249,
          stock: 100,
          color: "black",
          gender: "female",
          imageSrc:
            "https://i.postimg.cc/vH9mLxgC/womens-track-pants-black.jpg",
          description: `These comfortable socks from 'Happy Socks', are guaranteed to keep your feet satisfied.`,
        },
      ],
    }; // End of 'return' object
  },
};
</script>

<style scoped>
  #cards-holder {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    margin: auto;
    row-gap: 20px;
  }
  .cards-holder .card {
    grid-column: span 1;
    margin: auto;
  }
  .cards-holder .card h5 {
    text-transform: capitalize;
  }
  .card {
    width: 18rem;
    display: flex;
    flex-direction: column;
    background-color: white;
    box-shadow: 0 0 5px black;
    padding: 10px;
  }
  .card img {
    width: inherit;
  }
</style>
