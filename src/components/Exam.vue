<template>
  <div class="ui grid sixteen wide" style="margin: 1rem;">
      <div class="ui column one wide green">#</div>
      <div class="ui column seven wide green">Description</div>
      <div class="ui column seven wide green">Price</div>
      <div class="ui column one wide green"></div>

      <!-- items list -->
      <div class="ui column one wide">1</div>
      <div class="ui column seven wide">Item Name</div>
      <div class="ui column six wide">Price</div>
      <div class="ui column two wide">
        <button class="ui red icon button">
          <i class="trash alternate outline icon" v-on:click="deleteItem()"></i>
        </button>
      </div>

      <div class="ui column one wide"></div>
      <div class="ui column seven wide"><input type="text" v-model="item"></div>
      <div class="ui column six wide"><input type="text" v-model="item.price"></div>
      <div class="ui column two wide">
        <button class="ui green icon button" v-on:click="addItem()">
          <i class="plus icon"></i>
        </button>
      </div>

      <div class="ui column eight wide green"><b>TOTAL</b></div>
      <div class="ui column eight wide green">{{ getTotal() }}</div>
  </div>
</template>

<script>
export default {
  name: "Exam",
  methods: {
    getTotal() {
      return 123;
    }
  },
  data() {
    return {
      items: [
        { descripton: "Mug", price: "100.00" },
        { description: "Cat", price: 5000.00 }
      ],
      item: { description: null, price: null }
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
