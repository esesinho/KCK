<template>
  <v-container fluid grid-list-md>
    <v-layout>
      
      <v-flex d-flex xs12 md6 sm6>
        <v-card id="app" color="purple" dark>
          <v-card-title primary class="title"></v-card-title>
             <v-card-text>
             {{people[0].name +' '+ people[0].age}}
            </v-card-text>
        </v-card>
      </v-flex>
          <v-flex xs3  d-flex  v-for="k in 2">
            <v-layout row wrap>
              <v-flex
                v-for="n in 6"
                xs12
              >
                <v-card
                  color="red lighten-2"
                  dark
                >
                  <v-card-text>{{people[k*n].name +' '+ people[k*n].age}}</v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-flex>
        </v-layout>
      </v-flex>
  </v-container>
</template>
<script>
  export default {
    data: () => ({
        people: [
      { name: 'John', age: 10 },
{
  name: "Witty",
  age: 90
}, {
  name: "Jen",
  age: 81
}, {
  name: "Welbie",
  age: 29
}, {
  name: "Charo",
  age: 60
}, {
  name: "Trudie",
  age: 100
}, {
  name: "Pren",
  age: 31
}, {
  name: "Iosep",
  age: 38
}, {
  name: "Nichole",
  age: 43
}, {
  name: "Cindi",
  age: 14
}, {
  name: "Lauryn",
  age: 73
}, {
  name: "Alvin",
  age: 15
}, {
  name: "Francklyn",
  age: 61
}]
    })
    
  }
</script>
