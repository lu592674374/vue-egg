<template>
  <div>
    <LayoutHeader></LayoutHeader>
    <LayoutContent>
      <div slot="content">
        <slot name="main"></slot>
      </div>
    </LayoutContent>
    <LayoutFooter></LayoutFooter>
  </div>
</template>
<style lang="css">
  body {
    margin: 0 0px;
  }

  a {
    text-decoration: none;
  }

  @import "../../../asset/css/global.css";
</style>
<script type="ts">
  import LayoutHeader from './header/header';
  import LayoutContent from './content/content';
  import LayoutFooter from './footer/footer';
  export default {
    components: {
      LayoutHeader,
      LayoutContent,
      LayoutFooter
    }
  };
</script>
