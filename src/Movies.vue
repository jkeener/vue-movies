<template>
<div class="container">
  <div v-for="movie in movies" class="images">
    <a v-bind:href="movie.url">
              <img v-bind:src="movie.img">
          </a>
    <div class="title">{{movie.title}}</div>
  </div>
</div>
</template>

<script>
export default {
  data() {
    return {
      movies: [
        //Add your images, captions, and urls here.
        {
          img: 'assets/pics/my-neighbor-totoro.jpg',
          url: "http://www.imdb.com/title/tt0096283/",
          title: "My Neighbour Totoro"
        },
        {
          img: 'assets/pics/pans-labyrinth.jpg',
          url: "http://www.imdb.com/title/tt0457430/",
          title: "Pan’s Labyrinth"
        },
        {
          img: 'assets/pics/close-encounters.jpg',
          url: "http://www.imdb.com/title/tt0075860/",
          title: "Close Encounters of the..."
        },
        {
          img: 'https://goo.gl/RbOhf5',
          url: "http://www.imdb.com/title/tt0088847/",
          title: "The Breakfast Club"
        },
        {
          img: 'https://goo.gl/WY4BpP',
          url: "http://www.imdb.com/title/tt0046438/",
          title: "Tokyo Story"
        },
        {
          img: 'https://goo.gl/cXtjiH',
          url: "http://www.imdb.com/title/tt0045152/",
          title: "Singin’ in the Rain"
        },
        {
          img: 'https://goo.gl/unT8xp',
          url: "http://www.imdb.com/title/tt0097202/",
          title: "The Killer"
        },
        {
          img: 'https://goo.gl/BJ16O6',
          url: "http://www.imdb.com/title/tt0053779/",
          title: "La Dolce Vita"
        },
        {
          img: 'https://goo.gl/AUAuh3',
          url: "http://www.imdb.com/title/tt0304141/",
          title: "Harry Potter and the..."
        },
        {
          img: 'https://goo.gl/QcbjWV',
          url: "http://www.imdb.com/title/tt0169547/",
          title: "American Beauty"
        },
        {
          img: 'https://goo.gl/nMuYVz',
          url: "http://www.imdb.com/title/tt0206634/",
          title: "Children of Men"
        },
        {
          img: 'https://goo.gl/HtT9zC',
          url: "http://www.imdb.com/title/tt0054047/",
          title: "The Magnificent Seven"
        },
        {
          img: 'https://goo.gl/ucQR2L',
          url: "http://www.imdb.com/title/tt0120815/",
          title: "Saving Private Ryan"
        },
        {
          img: 'https://goo.gl/db8DPi',
          url: "http://www.imdb.com/title/tt0047478/",
          title: "Seven Samurai"
        },
        {
          img: 'https://goo.gl/Y4be5n',
          url: "http://www.imdb.com/title/tt0266308/",
          title: "Battle Royale"
        },
        {
          img: 'https://goo.gl/Xya3we',
          url: "http://www.imdb.com/title/tt0058946/",
          title: "The Battle of Algiers"
        },
        {
          img: 'https://goo.gl/IOqjqw',
          url: "http://www.imdb.com/title/tt0096438/",
          title: "Who Framed Roger Rabbit"
        },
        {
          img: 'https://goo.gl/H42Oxm',
          url: "http://www.imdb.com/title/tt0038348/",
          title: "Beauty and the Beast"
        },
        {
          img: 'https://goo.gl/pmJ8yk',
          url: "http://www.imdb.com/title/tt0317248/",
          title: "City of God"
        },
        {
          img: 'https://goo.gl/hWkewV',
          url: "http://www.imdb.com/title/tt0031885/",
          title: "The Rules of the Game"
        },
        {
          img: 'https://goo.gl/6WSNbG',
          url: "http://www.imdb.com/title/tt0060138/",
          title: "Au hasard Balthazar"
        },
        {
          img: 'https://goo.gl/7c2d1R',
          url: "http://www.imdb.com/title/tt0033870/",
          title: "The Maltese Falcon"
        },
        {
          img: 'https://goo.gl/uxsYkf',
          url: "http://www.imdb.com/title/tt0042546/",
          title: "Harvey"
        },
        {
          img: 'https://goo.gl/r798lo',
          url: "http://www.imdb.com/title/tt0015864/",
          title: "The Gold Rush"
        },
        {
          img: 'https://goo.gl/4kQQYT',
          url: "http://www.imdb.com/title/tt0050976/",
          title: "The Seventh Seal"
        },
        {
          img: 'https://goo.gl/RwxzGu',
          url: "http://www.imdb.com/title/tt0097216/",
          title: "Do the Right Thing"
        },
        {
          img: 'https://goo.gl/nZWZmi',
          url: "http://www.imdb.com/title/tt0031381/",
          title: "Gone with the Wind"
        },
        {
          img: 'https://goo.gl/NaI02s',
          url: "http://www.imdb.com/title/tt0049730/",
          title: "The Searchers"
        },
        {
          img: 'https://goo.gl/2LJaDS',
          url: "http://www.imdb.com/title/tt0119396/",
          title: "Jackie Brown"
        },
        {
          img: 'https://goo.gl/lRPHOO',
          url: "http://www.imdb.com/title/tt0034583/",
          title: "Casablanca"
        },
        {
          img: 'https://goo.gl/EuKXBe',
          url: "http://www.imdb.com/title/tt0041959/",
          title: "The Third Man"
        },
        {
          img: 'https://goo.gl/RIzgkg',
          url: "http://www.imdb.com/title/tt0062229/",
          title: "Le Samouraï"
        },
        {
          img: 'https://goo.gl/ZCG6IF',
          url: "http://www.imdb.com/title/tt0056172/",
          title: "Lawrence of Arabia"
        },
        {
          img: 'https://goo.gl/E6QEoe',
          url: "http://www.imdb.com/title/tt0054997/",
          title: "The Hustler"
        },
        {
          img: 'https://goo.gl/fEcSBn',
          url: "http://www.imdb.com/title/tt0407887/",
          title: "The Departed"
        },
        {
          img: 'https://goo.gl/4KAsVr',
          url: "http://www.imdb.com/title/tt0055630/",
          title: "Yojimbo"
        },
        {
          img: 'https://goo.gl/h9smFF',
          url: "http://www.imdb.com/title/tt0047296/",
          title: "On the Waterfront"
        },
        {
          img: 'https://goo.gl/2XXDvk',
          url: "http://www.imdb.com/title/tt0049902/",
          title: "A Man Escaped"
        },
        {
          img: 'https://goo.gl/b8002D',
          url: "http://www.imdb.com/title/tt0053472/",
          title: "Breathless"
        },
        {
          img: 'https://goo.gl/577tHH',
          url: "http://www.imdb.com/title/tt0172495/",
          title: "Gladiator"
        },
        {
          img: 'https://goo.gl/2QmDvK',
          url: "http://www.imdb.com/title/tt0057565/",
          title: "High and Low"
        },
        {
          img: 'https://goo.gl/hFHu24',
          url: "http://www.imdb.com/title/tt0144084/",
          title: "American Psycho"
        },
        {
          img: 'https://goo.gl/1RJ7kq',
          url: "http://www.imdb.com/title/tt0070040/",
          title: "The Spirit of the Beehive"
        },
        {
          img: 'https://goo.gl/cVx8sR',
          url: "http://www.imdb.com/title/tt0099685/",
          title: "GoodFellas"
        },
        {
          img: 'https://goo.gl/oCrsXy',
          url: "http://www.imdb.com/title/tt0416449/",
          title: "300"
        },
        {
          img: 'https://goo.gl/PGq6QB',
          url: "http://www.imdb.com/title/tt0376968/",
          title: "The Return"
        },
        {
          img: 'https://goo.gl/NNt3s1',
          url: "http://www.imdb.com/title/tt0083944/",
          title: "First Blood"
        },
        {
          img: 'https://goo.gl/Y5nb0A',
          url: "http://www.imdb.com/title/tt0063350/",
          title: "Night of the Living Dead"
        },
        {
          img: 'https://goo.gl/EyOYmB',
          url: "http://www.imdb.com/title/tt0084855/",
          title: "The Verdict"
        },
        {
          img: 'https://goo.gl/ORUyGy',
          url: "http://www.imdb.com/title/tt0082010/",
          title: "An American Werewolf..."
        },
        {
          img: 'https://goo.gl/C0XgLM',
          url: "http://www.imdb.com/title/tt0109506/",
          title: "The Crow"
        },
        {
          img: 'https://goo.gl/YYPvvj',
          url: "http://www.imdb.com/title/tt0110148/",
          title: "Interview with the Vampire"
        },
        {
          img: 'https://goo.gl/1ahWa5',
          url: "http://www.imdb.com/title/tt0077975/",
          title: "Animal House"
        },
        {
          img: 'https://goo.gl/BJjAsA',
          url: "http://www.imdb.com/title/tt0028445/",
          title: "A Day in the Country"
        },
        {
          img: 'https://goo.gl/Mo6tvu',
          url: "http://www.imdb.com/title/tt0042876/",
          title: "Rashomon"
        },
        {
          img: 'https://goo.gl/49RNnF',
          url: "http://www.imdb.com/title/tt0469494/",
          title: "There Will Be Blood"
        },
        {
          img: 'https://goo.gl/XXzYeX',
          url: "http://www.imdb.com/title/tt0023969/",
          title: "Duck Soup"
        },
        {
          img: 'https://goo.gl/8t8hko',
          url: "http://www.imdb.com/title/tt0050212/",
          title: "The Bridge on the River Kwai"
        },
        {
          img: 'https://goo.gl/bKqOL5',
          url: "http://www.imdb.com/title/tt0058182/",
          title: "A Hard Day’s Night"
        },
        {
          img: 'https://goo.gl/BRoCD8',
          url: "http://www.imdb.com/title/tt0022100/",
          title: "M"
        },
        {
          img: 'https://goo.gl/ynmoNM',
          url: "http://www.imdb.com/title/tt0040522/",
          title: "Bicycle Thieves"
        },
        {
          img: 'https://goo.gl/2qFokz',
          url: "http://www.imdb.com/title/tt0128445/",
          title: "Rushmore"
        },
        {
          img: 'https://goo.gl/ZPy5Iu',
          url: "http://www.imdb.com/title/tt0090728/",
          title: "Big Trouble in Little China"
        },
        {
          img: 'https://goo.gl/yhGdZw',
          url: "http://www.imdb.com/title/tt0052357/",
          title: "Vertigo"
        },
        {
          img: 'https://goo.gl/dBkU2z',
          url: "http://www.imdb.com/title/tt0245712/",
          title: "Amores Perros"
        },
        {
          img: 'https://goo.gl/ovf8N5',
          url: "http://www.imdb.com/title/tt0056801/",
          title: "8 ½"
        },
        {
          img: 'https://goo.gl/AitYxk',
          url: "http://www.imdb.com/title/tt0099674/",
          title: "The Godfather Part III"
        },
        {
          img: 'https://goo.gl/TgGqx2',
          url: "http://www.imdb.com/title/tt0114746/",
          title: "12 Monkeys"
        },
        {
          img: 'https://goo.gl/bh0p5f',
          url: "http://www.imdb.com/title/tt0020530/",
          title: "Un chien andalou"
        },
        {
          img: 'https://goo.gl/iHDAtU',
          url: "http://www.imdb.com/title/tt0048980/",
          title: "The Red Balloon"
        },
        {
          img: 'https://goo.gl/iuaDc6',
          url: "http://www.imdb.com/title/tt0092099/",
          title: "Top Gun"
        },
        {
          img: 'https://goo.gl/OUdk77',
          url: "http://www.imdb.com/title/tt0364569/",
          title: "Oldboy"
        },
        {
          img: 'https://goo.gl/axjqaS',
          url: "http://www.imdb.com/title/tt0060196/",
          title: "The Good, the Bad and..."
        },
        {
          img: 'https://goo.gl/fZzwdx',
          url: "http://www.imdb.com/title/tt0053291/",
          title: "Some Like It Hot"
        },
        {
          img: 'https://goo.gl/nCoesa',
          url: "http://www.imdb.com/title/tt0203009/",
          title: "Moulin Rouge!"
        },
        {
          img: 'https://goo.gl/CHabzg',
          url: "http://www.imdb.com/title/tt0116282/",
          title: "Fargo"
        },
        {
          img: 'https://goo.gl/LuhMMd',
          url: "http://www.imdb.com/title/tt0030341/",
          title: "The Lady Vanishes"
        },
        {
          img: 'https://goo.gl/42Xq0H',
          url: "http://www.imdb.com/title/tt0081398/",
          title: "Raging Bull"
        },
        {
          img: 'https://goo.gl/y0ibXe',
          url: "http://www.imdb.com/title/tt0043014/",
          title: "Sunset Boulevard"
        },
        {
          img: 'https://goo.gl/AX1Qzg',
          url: "http://www.imdb.com/title/tt0071315/",
          title: "Chinatown"
        },
        {
          img: 'https://goo.gl/yvdgqw',
          url: "http://www.imdb.com/title/tt0069704/",
          title: "American Graffiti"
        },
        {
          img: 'https://goo.gl/sGVVk7',
          url: "http://www.imdb.com/title/tt0110912/",
          title: "Pulp Fiction"
        },
        {
          img: 'https://goo.gl/nv8mhB',
          url: "http://www.imdb.com/title/tt0095016/",
          title: "Die Hard"
        },
        {
          img: 'https://goo.gl/gxIPxs',
          url: "http://www.imdb.com/title/tt0090605/",
          title: "Aliens"
        },
        {
          img: 'https://goo.gl/B5XtWP',
          url: "http://www.imdb.com/title/tt0078748/",
          title: "Alien"
        },
        {
          img: 'https://goo.gl/PktXkr',
          url: "http://www.imdb.com/title/tt0032599/",
          title: "His Girl Friday"
        },
        {
          img: 'https://goo.gl/eyabqO',
          url: "http://www.imdb.com/title/tt0057115/",
          title: "The Great Escape"
        },
        {
          img: 'https://goo.gl/W0n7Vu',
          url: "http://www.imdb.com/title/tt0181875/",
          title: "Almost Famous"
        },
        {
          img: 'https://goo.gl/IFdJZZ',
          url: "http://www.imdb.com/title/tt0265666/",
          title: "The Royal Tenenbaums"
        },
        {
          img: 'https://goo.gl/9HRfaz',
          url: "http://www.imdb.com/title/tt0211915/",
          title: "Amélie"
        },
        {
          img: 'https://goo.gl/XIWkss',
          url: "http://www.imdb.com/title/tt0015648/",
          title: "Battleship Potemkin"
        },
        {
          img: 'https://goo.gl/ld8F4j',
          url: "http://www.imdb.com/title/tt0117951/",
          title: "Trainspotting"
        },

      ],
    };
  },
}
</script>

<style>

.container {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(13em,1fr));
  grid-gap: .5em;
  padding: 1em;
}

.images {
  position: relative;
  margin: 0 0 1.2em 1em;
  justify-self: center;
  align-self: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.images:before {
  position: absolute;
  content: '';
  height: 25px;
  width: 25px;
  background-color: #fda9b8;
  z-index: 1;
  top: -10px;
  left: -10px;
}

img {
  filter: grayscale(100%);
  height: 19em;
  width: 13em;
  transition: filter .5s ease-in-out;
  border: 1px solid darkgray;
}

img:hover {
  filter: grayscale(0);
  transition: filter .5s ease-in-out;
}

.title {
  padding: .3em;
}

@media screen and (min-width: 1100px) {
  .container {
    width: 70%;
  }
}
</style>
