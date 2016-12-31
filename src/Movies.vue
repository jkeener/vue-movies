<template>
  <div class="container">
    <div class="inner-container">
       <div v-for="movie in movies" class="images">
           <img v-bind:src="movie.img">
           <div class="title">{{movie.title}}</div>
       </div>
    </div>
      <h3 class="count">Number of movies we have seen:<span>&nbsp {{movies.length}}</span></h3>
    </div>
</template>

<script>

export default {
  data () {
    return {
        movies: [
            //Add your images and captions here.
            {img: 'https://goo.gl/unT8xp',title: "The Killer"},
            {img: 'https://goo.gl/BJ16O6',title: "La Dolce Vita"},
            {img: 'https://goo.gl/AUAuh3',title: "Harry Potter and the Prisoner..."},
            {img: 'https://goo.gl/QcbjWV',title: "American Beauty"},
            {img: 'https://goo.gl/nMuYVz',title: "Children of Men"},
            {img: 'https://goo.gl/HtT9zC',title: "The Magnificent Seven"},
            {img: 'https://goo.gl/ucQR2L',title: "Saving Private Ryan"},
            {img: 'https://goo.gl/db8DPi',title: "Seven Samurai"},
            {img: 'https://goo.gl/Y4be5n',title: "Battle Royale"},
            {img: 'https://goo.gl/Xya3we',title: "The Battle of Algiers"},
            {img: 'https://goo.gl/IOqjqw',title: "Who Framed Roger Rabbit"},
            {img: 'https://goo.gl/H42Oxm',title: "Beauty and the Beast"},
            {img: 'https://goo.gl/pmJ8yk',title: "City of God"},
            {img: 'https://goo.gl/hWkewV',title: "The Rules of the Game"},
            {img: 'https://goo.gl/6WSNbG',title: "Au hasard Balthazar"},
            {img: 'https://goo.gl/7c2d1R',title: "The Maltese Falcon"},
            {img: 'https://goo.gl/uxsYkf',title: "Harvey"},
            {img: 'https://goo.gl/r798lo',title: "The Gold Rush"},
            {img: 'https://goo.gl/4kQQYT',title: "The Seventh Seal"},
            {img: 'https://goo.gl/RwxzGu',title: "Do the Right Thing"},
            {img: 'https://goo.gl/nZWZmi',title: "Gone with the Wind"},
            {img: 'https://goo.gl/NaI02s',title: "The Searchers"},
            {img: 'https://goo.gl/2LJaDS',title: "Jackie Brown"},
            {img: 'https://goo.gl/NAae19',title: "Casablanca"},
            {img: 'https://goo.gl/EuKXBe',title: "The Third Man"},
            {img: 'https://goo.gl/RIzgkg',title: "Le Samouraï"},
            {img: 'https://goo.gl/ZCG6IF',title: "Lawrence of Arabia"},
            {img: 'https://goo.gl/2OaDKC',title: "The Hustler"},
            {img: 'https://goo.gl/fEcSBn',title: "The Departed"},
            {img: 'https://goo.gl/4KAsVr',title: "Yojimbo"},
            {img: 'https://goo.gl/h9smFF',title: "On the Waterfront"},
            {img: 'https://goo.gl/2XXDvk',title: "A Man Escaped"},
            {img: 'https://goo.gl/b8002D',title: "Breathless"},
            {img: 'https://goo.gl/577tHH',title: "Gladiator"},
            {img: 'https://goo.gl/2QmDvK',title: "High and Low"},
            {img: 'https://goo.gl/hFHu24',title: "American Psycho"},
            {img: 'https://goo.gl/1RJ7kq',title: "Spirit of the Beehive"},
            {img: 'https://goo.gl/cVx8sR',title: "GoodFellas"},
            {img: 'https://goo.gl/oCrsXy',title: "300"},
            {img: 'https://goo.gl/PGq6QB',title: "The Return"},
            {img: 'https://goo.gl/NNt3s1',title: "First Blood"},
            {img: 'https://goo.gl/Y5nb0A',title: "Night of the Living Dead"},
            {img: 'https://goo.gl/EyOYmB',title: "The Verdict"},
            {img: 'https://goo.gl/ORUyGy',title: "An American Werewolf in London"},
            {img: 'https://goo.gl/C0XgLM',title: "The Crow"},
            {img: 'https://goo.gl/YYPvvj',title: "Interview with the Vampire"},
            {img: 'https://goo.gl/1ahWa5',title: "Animal House"},
            {img: 'https://goo.gl/BJjAsA',title: "A Day in the Country"},
            {img: 'https://goo.gl/Mo6tvu',title: "Rashomon"},
            {img: 'https://goo.gl/49RNnF',title: "There Will Be Blood"},
            {img: 'https://goo.gl/XXzYeX',title: "Duck Soup"},
            {img: 'https://goo.gl/8t8hko',title: "The Bridge on the River Kwai"},
            {img: 'https://goo.gl/bKqOL5',title: "A Hard Day’s Night"},
            {img: 'https://goo.gl/BRoCD8',title: "M"},
            {img: 'https://goo.gl/ynmoNM',title: "Bicycle Thieves"},
            {img: 'https://goo.gl/2qFokz',title: "Rushmore"},
            {img: 'https://goo.gl/ZPy5Iu',title: "Big Trouble in Little China"},
            {img: 'https://goo.gl/yhGdZw',title: "Vertigo"},
            {img: 'https://goo.gl/dBkU2z',title: "Amores Perros"},
            {img: 'https://goo.gl/ovf8N5',title: "8 ½"},
            {img: 'https://goo.gl/AitYxk',title: "The Godfather Part III"},
            {img: 'https://goo.gl/TgGqx2',title: "12 Monkeys"},
            {img: 'https://goo.gl/bh0p5f',title: "Un chien andalou"},
            {img: 'https://goo.gl/iHDAtU',title: "The Red Balloon"},
            {img: 'https://goo.gl/iuaDc6',title: "Top Gun"},
            {img: 'https://goo.gl/OUdk77',title: "Oldboy"},
            {img: 'https://goo.gl/axjqaS',title: "The Good, the Bad and the Ugly"},
            {img: 'https://goo.gl/fZzwdx',title: "Some Like It Hot"},
            {img: 'https://goo.gl/nCoesa',title: "Moulin Rouge!"},
            {img: 'https://goo.gl/CHabzg',title: "Fargo"},
            {img: 'https://goo.gl/LuhMMd',title: "The Lady Vanishes"},
            {img: 'https://goo.gl/42Xq0H',title: "Raging Bull"},
            {img: 'https://goo.gl/y0ibXe',title: "Sunset Boulevard"},
            {img: 'https://goo.gl/AX1Qzg',title: "Chinatown"},
            {img: 'https://goo.gl/yvdgqw',title: "American Graffiti"},
            {img: 'https://goo.gl/sGVVk7',title: "Pulp Fiction"},
            {img: 'https://goo.gl/nv8mhB',title: "Die Hard"},
            {img: 'https://goo.gl/gxIPxs',title: "Aliens"},
            {img: 'https://goo.gl/B5XtWP',title: "Alien"},
            {img: 'https://goo.gl/PktXkr',title: "His Girl Friday"},
            {img: 'https://goo.gl/eyabqO',title: "The Great Escape"},
            {img: 'https://goo.gl/W0n7Vu',title: "Almost Famous"},
            {img: 'https://goo.gl/IFdJZZ',title: "The Royal Tenenbaums"},
            {img: 'https://goo.gl/9HRfaz',title: "Amélie"},
            {img: 'https://goo.gl/XIWkss',title: "Battleship Potemkin"},
            {img: 'https://goo.gl/ld8F4j',title: "Trainspotting"},

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
    }
    
    .inner-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        margin: 1em;
    }
    
    .images {
        position: relative;
        margin: 0 0 1.2em 1em;
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
        height:300px;
        width:200px;
    }
    
    img:hover {
        filter: grayscale(0);
    }
    
    .title {
        margin: .3em;
        font-size: .8em;
        visibility: hidden;
    }

</style>