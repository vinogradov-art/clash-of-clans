<template>
  <div class="md-body">
    <div class="card__wrapper" v-for="item in items" :key="item.id">
      <card-component
        :name="`${item.lvl} lvl`"
        :title="item.title"
        :disc="item.descr"
      >
        <h1>Hello</h1>
        <p>Edit me</p>
      </card-component>
    </div>
  </div>
</template>

<script>
import CardComponent from "@/componets/UI/CardComponent"

export default {
  components: { CardComponent },

  data() {
    return {
      items: [
        {
          id: 1,
          title: "Archer",
          descr: "archer archer archer archer",
          lvl: 5
        },
        {
          id: 2,
          title: "Barbarian",
          descr: "barbarian barbarian barbarian",
          lvl: 5
        },
        {
          id: 3,
          title: "Giant",
          descr: "giant giant giant giant",
          lvl: 5
        },
        {
          id: 4,
          title: "Goblin",
          descr: "goblin goblin goblin goblin",
          lvl: 5
        },
        {
          id: 5,
          title: "Wizard",
          descr: "wizard wizard wizard wizard",
          lvl: 5
        }
      ]
    }
  }
}
</script>