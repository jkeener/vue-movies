<template>
    <div class="container">
       <div v-for="image in images" class="images">
           <img v-bind:src="image.img">
           <div class="title">{{image.title}}</div>
       </div>
    </div>
</template>

<script>

export default {
  data () {
    return {
        images: [
            //Add your images and captions here.
            {img: 'http://lorempixel.com/200/300',title: "Movie 1"},
            {img: 'http://lorempixel.com/201/300',title: "Movie 2"},
            {img: 'http://lorempixel.com/200/301',title: "Movie 3"},
            {img: 'http://lorempixel.com/201/301',title: "Movie 4"},
            {img: 'http://lorempixel.com/202/300',title: "Movie 5"},
            {img: 'http://lorempixel.com/200/302',title: "Movie 6"},
            {img: 'http://lorempixel.com/202/302',title: "Movie 7"},
            {img: 'http://lorempixel.com/203/300',title: "Movie 8"},
            {img: 'http://lorempixel.com/200/303',title: "Movie 9"},
            {img: 'http://lorempixel.com/203/303',title: "Movie 10"},
        ],
    };
  },
}
</script>

<style>
    .container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 1em;
    }
    
    .images {
        position: relative;
        margin: 0 0 1em 1em;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    .images:hover .title {
        visibility: visible;
    }
    
    .images:before {
        position: absolute;
        content: '';
        height: 25px;
        width: 25px;
        background-color: #fda9b8;
        z-index: 1;
        top:-10px; left: -10px;
    }
    
    img {
        filter: grayscale(100%);
        transition: .6s;
    }
    
    img:hover {
        filter: grayscale(0);
    }
    
    .title {
        margin-left: .3em;
        font-size: 1.2em;
        visibility: hidden;
    }

</style>