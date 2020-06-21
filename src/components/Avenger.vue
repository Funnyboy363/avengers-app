<template>
    <div>
    <div class="container" v-for="avenger in avengers" v-bind:key="avenger">
     <h4> {{ avenger.name }}</h4>
      <p class="avenger"> Avenger Name: {{ avenger.aname }}</p>
      <p class="avenger">{{ avenger.info }} </p>
    </div>
    </div>
</template>

<script>
export default {
      data() {
          return {
    avengers: [
      { name: 'Tony Stark',
        aname: 'Iron Man',
        info: 'A wealthy American business magnate, playboy, and ingenious scientist, Anthony Edward "Tony" Stark suffers a severe chest injury during a kidnapping. When his captors attempt to force him to build a weapon of mass destruction, he instead creates a mechanized suit of armor to save his life and escape captivity. Later, Stark develops his suit, adding weapons and other technological devices he designed through his company, Stark Industries. He uses the suit and successive versions to protect the world as Iron Man. Although at first concealing his true identity, Stark eventually declared that he was, in fact, Iron Man in a public announcement (wiki)'
      },
      { name: 'Steve Rogers', 
        aname: 'Captain America',
        info: 'The character wears a costume bearing an American flag motif, and he utilizes a nearly indestructible shield that he throws as a projectile. Captain America is the alter ego of Steve Rogers, a frail young man enhanced to the peak of human perfection by an experimental serum to aid the United States governments efforts in World War II. Near the end of the war, he was trapped in ice and survived in suspended animation until he was revived in modern times. Although Captain America often struggles to maintain his ideals as a man out of his time, he remains a highly respected figure in his community, which includes becoming the long-time leader of the Avengers (wiki)'
      },
      { name: 'Thor Odinson',
        aname: 'Thor the mighty',
        info: 'In Germanic mythology, Thor (/θɔːr/; from Old Norse: Þórr, runic ᚦᚢᚱ þur) is a hammer-wielding god associated with thunder, lightning, storms, sacred groves and trees, strength, the protection of mankind and also hallowing and fertility. Besides Old Norse Þórr, extensions of the god occur in Old English as Þunor and in Old High German as Donar (runic ᚦᛟᚾᚨᚱ þonar). All forms of the deity stem from a Common Germanic *Þunraz (wiki)'
      }
    ]
  }
},
}
</script>


<style scoped>
li {
    list-style-type: none;
}

h4 {
    text-align: left;
    margin-top: 30px;
    margin-bottom: 0;
}

.avenger {
    text-align: left;
    margin: 0;
}

</style>