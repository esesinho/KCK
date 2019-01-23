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
  name: "Nanette",
  age: 25
}, {
  name: "Alexia",
  age: 15
}, {
  name: "Claire",
  age: 51
}, {
  name: "Waite",
  age: 77
}, {
  name: "Margalo",
  age: 39
}, {
  name: "Jermaine",
  age: 84
}, {
  name: "Guglielmo",
  age: 87
}, {
  name: "Rossy",
  age: 21
}, {
  name: "Joelynn",
  age: 13
}, {
  name: "Vevay",
  age: 95
}, {
  name: "Jacenta",
  age: 5
}, {
  name: "Kelcy",
  age: 75
}]
    })
    
  }
</script>
