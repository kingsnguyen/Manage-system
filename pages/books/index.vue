<template>
  <div>
    <h1>test</h1>
  </div>
</template>

<script>
import axios from "axios";
export default {
  created() {
    axios
      .post("/books", {
        bookName: "Fred",
        bookLastName: "Flintstone",
      })
      .then(function (response) {
        console.log(response);
      })
      .catch(function (error) {
        console.log(error);
      });
  },
};
</script>