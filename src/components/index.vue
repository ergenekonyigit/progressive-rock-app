<template>
  <div>
    <h1>PRA</h1>
    <div class="Cards">
      <Card v-for="(Card, Index) in Cards"
            :Card="Card"
            :key="Index"></Card>
    </div>
    <p class="footer">Made by <a target="_blank" href="https://github.com/ergenekonyigit">ergenekonyigit</a>, <a target="_blank" href="https://github.com/ergenekonyigit/progressive-rock-app">Github</a></p>
  </div>
</template>

<script>
  import Card from './card'

  export default {
    name: 'Index',
    components: {
      Card
    },
    data () {
      return {
        Cards: [
          {
            theme: 'dark',
            cover_photo: 'alternative.png',
            title: 'Alternative Rock',
            date: 'Late 1970s to early 1980s',
            origin: 'United Kingdom and United States',
            body: 'Alternative rock (also called alternative music, alt-rock or simply alternative) is a style of rock music that emerged from the independent music underground of the 1980s and became widely popular in the 1990s. In this instance, the word "alternative" refers to the genre\'s distinction from mainstream rock music. The term\'s original meaning was broader, referring to a generation of musicians unified by their collective debt to either the musical style or simply the independent, DIY ethos of punk rock, which in the late 1970s laid the groundwork for alternative music. At times, "alternative" has been used as a catch-all description for music from underground rock artists that receives mainstream recognition, or for any music, whether rock or not, that is seen to be descended from punk rock (including some examples of punk itself, as well as new wave, and post-punk).'
          },
          {
            theme: 'dark',
            cover_photo: 'anatolian.png',
            title: 'Anatolian Rock',
            date: 'Late 1950s/early 1980s',
            origin: 'Turkey',
            body: 'Anatolian rock (Turkish: Anadolu rock), also known as Turkish rock, is a fusion of Turkish folk and rock music. It emerged during the mid-1960s, soon after rock groups such as The Beatles, The Rolling Stones, Led Zeppelin, Yes, Status Quo and Omega became popular in Turkey. Examples of this style include Turkish musicians such as Cem Karaca, Barış Manço, Erkin Koray, Fikret Kızılok, Cahit Oben, Selçuk Alagöz, Edip Akbayram alongside bands such as Moğollar, Silüetler, Kurtalan Ekspres, Grup Çığrışım, Grup Çağrışım, Mavi Işıklar, Apaşlar, Kaygısızlar, Haramiler, Modern Folk Üçlüsü and Kardaşlar. Today, Anatolian rock includes music derived from both traditional Turkish folk music and rock.'
          },
          {
            theme: 'dark',
            cover_photo: 'celtic.png',
            title: 'Celtic Rock',
            date: '1970s',
            origin: 'Celtic',
            body: 'Celtic rock is a genre of folk rock, as well as a form of Celtic fusion which incorporates Celtic music, instrumentation and themes into a rock music context. It has been extremely prolific since the early 1970s and can be seen as a key foundation of the development of highly successful mainstream Celtic bands and popular musical performers, as well as creating important derivatives through further fusions. It has played a major role in the maintenance and definition of regional and national identities and in fostering a pan-Celtic culture. It has also helped to communicate those cultures to external audiences.'
          },
          {
            theme: 'dark',
            cover_photo: 'death.png',
            title: 'Death Rock',
            date: 'Late 1970s',
            origin: 'Los Angeles',
            body: 'Deathrock is a subgenre of punk rock, incorporating horror elements and gloomy, gothic theatrics. It emerged in the West Coast of the United States in the early 1980s, and is related to the style of music known as gothic rock. Notable acts include Christian Death and 45 Grave.'
          },
          {
            theme: 'light',
            cover_photo: 'funk.png',
            title: 'Funk Rock',
            date: 'Early 1970s',
            origin: 'United States',
            body: 'Funk rock is a fusion genre that mixes elements of funk and rock.[1] James Brown and others declared that Little Richard and his mid-1950s road band, The Upsetters, were the first to put the funk in the rock and roll beat, with a biographer stating that their music "spark[ed] the musical transition from fifties rock and roll to sixties funk".'
          },
          {
            theme: 'light',
            cover_photo: 'gothic.png',
            title: 'Gothic Rock',
            date: 'Late 1970s',
            origin: 'United Kingdom',
            body: 'Gothic rock (also referred to as goth rock or simply goth) is a style of rock music that emerged from post-punk in the late 1970s. Proto-gothic rock bands grew from the strong ties they had to the English punk rock and emerging post-punk scenes. Such bands include Siouxsie and the Banshees, Joy Division, Bauhaus and the Cure.'
          },
          {
            theme: 'dark',
            cover_photo: 'hard.png',
            title: 'Hard Rock',
            date: 'Mid-1960s',
            origin: 'United States and United Kingdom',
            body: 'Hard rock is a loosely defined subgenre of rock music that began in the mid-1960s, with the garage, psychedelic and blues rock movements. It is typified by a heavy use of aggressive vocals, distorted electric guitars, bass guitar, drums, and often accompanied with keyboards. \n Hard rock developed into a major form of popular music in the 1970s, with bands such as The Who, Led Zeppelin, Queen, Black Sabbath, Deep Purple, Aerosmith, KISS, AC/DC and Van Halen. During the 1980s, some hard rock bands moved away from their hard rock roots and more towards pop rock, while others began to return to a hard rock sound. Established bands made a comeback in the mid-1980s and it reached a commercial peak in the 1980s, with glam metal bands like Bon Jovi and Def Leppard and the rawer sounds of Guns N\' Roses, which followed up with great success in the later part of that decade. Hard rock began losing popularity with the commercial success of R&B, hip-hop, urban pop, grunge and later Britpop in the 1990s. \n Despite this, many post-grunge bands adopted a hard rock sound and in the 2000s there came a renewed interest in established bands, attempts at a revival, and new hard rock bands that emerged from the garage rock and post-punk revival scenes. Out of this movement came garage rock bands like The White Stripes, The Strokes, Interpol and, later on, The Black Keys. In the 2000s, only a few hard rock bands from the 1970s and 1980s managed to sustain highly successful recording careers.'
          },
          {
            theme: 'dark',
            cover_photo: 'progressive.png',
            title: 'Progressive Rock',
            date: 'Mid to late 1960s',
            origin: 'United Kingdom and United States',
            body: 'Progressive rock (shortened as prog; sometimes called art rock, classical rock or symphonic rock) is a broad subgenre of rock music that developed in the United Kingdom and United States throughout the mid to late 1960s. Initially termed "progressive pop", the style was an outgrowth of psychedelic bands who abandoned standard pop traditions in favour of instrumentation and compositional techniques more frequently associated with jazz, folk or classical music. Additional elements contributed to its "progressive" label: lyrics were more poetic, technology was harnessed for new sounds, music approached the condition of "art", and the studio, rather than the stage, became the focus of musical activity, which often involved creating music for listening, not dancing. \n Prog is based on fusions of styles, approaches and genres, involving a continuous move between formalism and eclecticism. Due to its historical reception, prog\'s scope is sometimes limited to a stereotype of long solos, overlong albums, fantasy lyrics, grandiose stage sets and costumes, and an obsessive dedication to technical skill. While the genre is often cited for its merging of high culture and low culture, few artists incorporated literal classical themes in their work to any great degree, and only a handful of groups purposely emulated or referenced classical music. \n The genre coincided with the mid 1960s economic boom that allowed record labels to allocate more creative control to their artists, as well as the new journalistic division between "pop" and "rock" that lent generic significance to both terms. Prog saw a high level of popularity in the early-to-mid 1970s, but faded soon after. Conventional wisdom holds that the rise of punk rock caused this, but several more factors contributed to the decline. Music critics, who often labelled the concepts as "pretentious" and the sounds as "pompous" and "overblown", tended to be hostile towards the genre or to completely ignore it. After the late 1970s, progressive rock fragmented in numerous forms; some bands achieved commercial success well into the 1980s, albeit with changed lineups and more compact song structures, and some crossed into symphonic pop, arena rock, or new wave. \n Early groups who exhibited progressive features are retroactively described as "proto-prog". In 1967, "progressive rock" constituted a diversity of loosely associated style codes. The Canterbury scene, originating in the late 1960s, denoted a subset of prog bands who emphasised the use of wind instruments, complex chord changes and long improvisations. Rock in Opposition, from the late 1970s, was more avant-garde, and when combined with the Canterbury style, created avant-prog. In the 1980s, a new subgenre, neo-progressive rock, enjoyed some commercial success, although it was also accused of being derivative and lacking in innovation. Post-progressive draws upon newer developments in popular music and the avant-garde since the mid 1970s.'
          }
        ]
      }
    }
  }
</script>

<style lang="scss">

  button, a {
    color: inherit;
    cursor: pointer;
  }

  html {
    line-height: 1.2;
  }

  h1 {
    margin: 20px 20px 0px;
  }

  .footer {
    text-align: center;
    margin: 20px;
  }

  .Cards {
    padding: 20px;
    margin: 0 auto;
  }

  .shadow-Card,
  .Card {
    height: 400px;
    margin-bottom: 30px;
  }

</style>
