<template lang="pug">
  div
    f-side-bar
    .main-content
      f-nav-bar
      f-header
      f-body
        router-view
      f-footer
</template>

<script>
import FSideBar from "@/components/decorator/SideBar";
import FNavBar from "@/components/decorator/NavBar";
import FBody from "@/components/decorator/Body";
import FHeader from "@/components/decorator/Header";
import FFooter from "@/components/decorator/Footer";

export default {
  name: "app",

  components: {
    FSideBar,
    FNavBar,
    FBody,
    FHeader,
    FFooter
  }
};
</script>
