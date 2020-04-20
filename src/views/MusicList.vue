<template>
  <div>
    <mu-paper :z-depth="1">
      <mu-grid-list class="gridlist-inline-demo" cols="4">
        <mu-sub-header>December</mu-sub-header>
        <mu-grid-tile v-for="(tile, index) in list" :key="index">
          <img :src="tile.image" />
          <span slot="title">{{ tile.title }}</span>
          <span slot="subTitle"
            >by <b>{{ tile.author }}</b></span
          >
          <mu-button slot="action" icon>
            <mu-icon></mu-icon>
          </mu-button>
        </mu-grid-tile>
      </mu-grid-list>
    </mu-paper>
  </div>
</template>

<script>
import breakfast from "../assets/images/1.jpg";
import burger from "../assets/images/2.jpg";
import camera from "../assets/images/3.jpg";
import hats from "../assets/images/4.jpg";
import honey from "../assets/images/4.jpg";
import morning from "../assets/images/1.jpg";
import vegetables from "../assets/images/2.jpg";
import waterPlant from "../assets/images/3.jpg";
export default {
  data() {
    return {
      list: [
        {
          image: breakfast,
          title: "Breakfast",
          author: "Myron"
        },
        {
          image: burger,
          title: "Burger",
          author: "Linyu"
        },
        {
          image: camera,
          title: "Camera",
          author: "ruolin"
        },
        {
          image: hats,
          title: "Hats",
          author: "kakali"
        },
        {
          image: honey,
          title: "Honey",
          author: "yuyang"
        },
        {
          image: morning,
          title: "Morning",
          author: "mokayi"
        },
        {
          image: vegetables,
          title: "Vegetables",
          author: "NUyyyyyyy"
        },
        {
          image: waterPlant,
          title: "water",
          author: "TDDyyyyyyy"
        }
      ]
    };
  }
};
</script>
<style>
.gridlist-demo {
  width: 360px;
  height: 450px;
  overflow-y: auto;
}
</style>
