<template>
  <v-container>
    <h1 class="text-7xl p-10 text-center"> Jokes and Castles </h1>
    <!-- <Header /> -->
    <Header :headerPage="info" />
    <NuxtLink to="/second">Second Page</NuxtLink>
    <nuxt-img src="/castle1.jpg" />
    <Content v-for="joke in jokes" :key="joke.id" :contentPage="joke" />
    <Footer :footerPage="info" />
  </v-container>
</template>

<script>
export default {
  data () {
    return {
      info: {
        title: 'Jokes and Castles',
        description: 'Jokes and Castles',
        author: 'Christopher Barber',
        license: 'MIT License'
      },
      castles: [
        {
          id: 1,
          title: 'Castle Near Body of Water Under Golden Hour',
          description: 'Castle sits on a peninsula during sunset or sunrise. The water is serenely reflective.',
          width: 3000,
          height: 1902,
          pathURL: '../assets/img/castle1.jpg',
          linkURL: 'https://www.pexels.com/@raybilcliff',
          credit: 'Ray Bilcliff',
          creditURL: 'https://www.pexels.com/photo/castle-near-body-of-water-under-golden-hour-1843364/'
        },
        {
          id: 2,
          title: 'Scenic Photo Of Castle During Dawn',
          description: 'Castle sits on a white cliff in the sunset surrounded by trees. The castle has beautiful white spires.',
          width: 3986,
          height: 5979,
          pathURL: '../assets/img/castle2.jpg',
          linkURL: 'https://www.pexels.com/@felixmittermeier',
          credit: 'Felix Mittermeier',
          creditURL: 'https://www.pexels.com/photo/scenic-photo-of-castle-during-dawn-2832044/'
        },
        {
          id: 3,
          title: 'Castle on Hill over Village Near Body of Water',
          description: 'Castle perches on top of a mountain overlooking a quaint, colourful nordic town.',
          width: 5788,
          height: 3867,
          pathURL: '../assets/img/castle3.jpg',
          linkURL: 'https://www.pexels.com/@kaip',
          credit: 'Kai Pilger',
          creditURL: 'https://www.pexels.com/photo/castle-on-hill-over-village-near-body-of-water-547494/'
        },
        {
          id: 4,
          title: 'Green Field and White and Black Concrete Structure during Sunset',
          description: 'Purple sky meets scenic green fields with stalwart castle/cathedral ruins and a medieval town breaking the contrast.',
          width: 4288,
          height: 2848,
          pathURL: '../assets/img/castle4.jpg',
          linkURL: 'https://www.pexels.com/@f4photography',
          credit: 'Peter Spencer',
          creditURL: 'https://www.pexels.com/photo/green-field-and-white-and-black-concrete-structure-during-sunset-663487/'
        },
        {
          id: 5,
          title: 'Gray Castle Under Cloudy Sky',
          description: 'Wide picture of sprawling battlements that meet at a stout fortress on top of a cliff. Green grass and bright daylight lightens the mood.',
          width: 6000,
          height: 4000,
          pathURL: '../assets/img/castle5.jpg',
          linkURL: 'https://www.pexels.com/@rudolf-kirchner-278171',
          credit: 'Rudolf Kirchner',
          creditURL: 'https://www.pexels.com/photo/gray-castle-under-cloudy-sky-831082/'
        },
        {
          id: 6,
          title: 'Body of Water Near Trees during Daytime',
          description: 'Lonely fortess stands on top of a green bluff which is astride a crisp body of water and lovely lush forests.',
          width: 4608,
          height: 3072,
          pathURL: '../assets/img/castle6.jpg',
          linkURL: 'https://www.pexels.com/@pixabay',
          credit: 'Pixabay',
          creditURL: 'https://www.pexels.com/photo/body-of-water-near-trees-during-daytime-161872/'
        },
        {
          id: 7,
          title: 'Architectural Photography of Brown and Gray Castle',
          description: 'Swampy highlands with an old crawling masonry slithering into a low great bridge, stout fortress and cozy wet stone homes',
          width: 3805,
          height: 2547,
          pathURL: '../assets/img/castle7.jpg',
          linkURL: 'https://www.pexels.com/@miquel-rossello-calafell-461325',
          credit: 'Miquel Rosselló Calafell',
          creditURL: 'https://www.pexels.com/photo/architectural-photography-of-brown-and-gray-castle-3061171/'
        },
        {
          id: 8,
          title: 'old medieval ruins of Dunluce Castle on ocean coast in northern Ireland famous place in UK',
          description: 'Beautiful old white-grey ruins that live inside the green mossy mountain cliffs of Northern Ireland.',
          width: 3840,
          height: 5760,
          pathURL: '../assets/img/castle8.jpg',
          linkURL: 'https://www.pexels.com/@iain-1191393',
          credit: 'Iain Irwin',
          creditURL: 'https://www.pexels.com/photo/old-medieval-ruins-of-dunluce-castle-on-ocean-coast-in-northern-ireland-famous-place-in-uk-2350368/'
        },
        {
          id: 9,
          title: 'Medieval stone castle under gloomy sky',
          description: 'Hogwarts style fortress with brown square spire rooves is lighted up and welcomes you with small tunnel against the immense square palisades.',
          width: 4321,
          height: 6482,
          pathURL: '../assets/img/castle9.jpg',
          linkURL: 'https://www.pexels.com/@julia-volk',
          credit: 'Julia Volk',
          creditURL: 'https://www.pexels.com/photo/medieval-stone-castle-under-gloomy-sky-5273514/'
        }
      ],
      jokes: [
        {
          joke: 'Velcro is a total rip off',
          funnyLevel: 300
        },
        {
          joke: 'A man walks into a bar. Ouch.',
          funnyLevel: 100
        },
        {
          joke: 'We don\'t serve your kind in here! A time traveler walks into a bar.',
          funnyLevel: 4000
        },
        {
          joke: 'I thought the chiropractor was going to be bad but I stood corrected',
          funnyLevel: 3000
        },
        {
          joke: 'How much does a pirate sell his ear rings for? Buck an ear',
          funnyLevel: 600
        },
        {
          joke: 'Never trust someone that uses graph paper. They could be plotting something.',
          funnyLevel: 5000
        }
      ]
    }
  },
  head () {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }
      ]
    }
  }
}
</script>
