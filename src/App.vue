<template>
  <div id="app">
    <InfoComponent :title="info.title" :description="info.description" />
    <ImageComponent :imageUrl="image.url" />
    <TextComponent :text="text.content" />
    <LinkComponent :url="link.url" :label="link.label" />
  </div>
</template>

<script>
import InfoComponent from "@/components/InfoComponent.vue";
import ImageComponent from "@/components/ImageComponent.vue";
import TextComponent from "@/components/TextComponent.vue";
import LinkComponent from "@/components/LinkComponent.vue";
import data from "@/data.json";

export default {
  components: {
    InfoComponent,
    ImageComponent,
    TextComponent,
    LinkComponent
  },
  data() {
    return {
      info: data.info,
      image: data.image,
      text: data.text,
      link: data.link
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
