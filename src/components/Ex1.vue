<script>
    export default { 
        data() {
            return {
                msg : "Choose your favorite fruit: ",
                fruit1: "apple",
                fruit2: "orange",
                fruit3: "peach",

                /*using array of fruit*/
                fruits:["apple","orange","peach"]
            }
        }
    }
</script>

<template>
  <div id="app">
    {{ msg }}
    {{ fruit1 }} <input type="radio" name="fruit">
    {{ fruit2 }} <input type="radio" name="fruit">
    {{ fruit3 }} <input type="radio" name="fruit">
    <p>
        <h3>Using an array</h3>
        {{ msg }}
        <span v-for="fruit in fruits">
            {{ fruit }} <input type="radio" name="fruit">
        </span>
    </p>
  </div>
</template>

<style scoped>
.greeting {
    color: red;
}
</style>
