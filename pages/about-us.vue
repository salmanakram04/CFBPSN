<template>
  <div class="container mt-5">
    <h2>About Us</h2>
    <br />
    <p>
      Hello Everyone! <br /><br />
      Welcome to Collaborative Filter Based Patient Social Network.
      <br />
      <br />
      This is the Final Year Project Web Application made by FA16-BSE-141 and
      SP17-BCS-093 in the supervision of Dr. Assad Abbas.

      <br />
      <br />
      We hope you enjoy our products as much as we enjoy offering them to you.
      If you have any questions or comments, please don't hesitate to contact
      us.

      <br />
      <br />
      Sincerely,
      <br />
      Salman Akram
    </p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      head: {
        title: "About Us - Dish Satellite Information",
        content: "Dish Satellite Information"
      }
    };
  },
  head() {
    return {
      title: this.head.title,
      meta: [
        { hid: "description", name: "description", content: this.head.content }
      ],
      link: [{ rel: "canonical", href: "https://www.dishsatinfo.com/about-us" }]
    };
  }
};
</script>

<style></style>
