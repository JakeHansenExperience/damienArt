<template>
  <div>
<div v-for="lamp in lamps">
  <v-card>

    <v-card-title>{{lamp}}</v-card-title>
    <v-img :src="lamp"> </v-img>
    <v-card-subtitle> {{artDescription}} </v-card-subtitle>
    <v-card-subtitle> Price: {{artPrice}} </v-card-subtitle>
    <v-card-subtitle> Status: {{artStatus}} </v-card-subtitle>

  </v-card>
</div>
</div>
</template>


<script>
export default {
  data() {
    return {
      artTitle: "Green Lantern",
      artDescription: "This is a dope non-lamp",
      artPrice: "TBD",
      artStatus: "Available",
      lamps: ['Lamp15.jpg','Lamp17.jpg','Lamp18.jpg','Lamp19.jpg','Lamp20.jpg','Lamp21.jpg','Lamp22.jpg','Lamp23.jpg','Lamp25.jpg','Lamp28.jpg',

    ]
}
},
  props: {
    //the parameters the comopnet accepst
    // message: String,
    // product: Object,
    // email: {
      // type: String
      // required: true,
      // default: 'none'
      // validator: function (value) {
      //   return true if valid
      // }
  },
  computed: {
    // fullName: function () {
    //   return this.fistName + ' ' + this.lastName
  },
  watch: {
    //called when firstname changes value
    // firstName: function (value, oldValue) {...}
  },
  methods: {
},
//Lifecycle Hooks: beforeCreate, created, beforeMount, mounted, beforeUPdate, updated, beforeDestroy, destroyed
};
</script>

<style scoped>
/*
vuetify styling
ranges from 0-16
{property} {direction} -{size}
property is type of spacing, m for margin p for padding
direction designates the side the property applies to
t (top)
b (bottom)
l (left)
r (right)
x (left and right )
y (top and bottom)
a (all directions)
size (1-16)
1 is 4px, 2 is 8 px, n1 is -4 px or auto
with breakpoints for screen sizes, xs, sm, md, lg, xl
{property}{direction}-{breakpoint}-{size} */
</style>
