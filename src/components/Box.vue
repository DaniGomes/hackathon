<template>
  <q-card align='left'>
    <q-item>
      <q-item-tile sublabel class="text-faded" lines='3'>{object}</q-item-tile>
    </q-item>
    <q-card-actions align='end'>
    </q-card-actions>
  </q-card>
</template>

<script>
import {
  QCard,
  QCardActions,
  QCardTitle,
  QItem,
  QItemTile,
  openURL,
  QContextMenu
} from "quasar";

export default {
  name: "Box",
  components: {
    QCard,
    QCardActions,
    QCardTitle,
    QItem,
    QItemTile,
    getDate,
    openURL,
    QContextMenu
  },
  props: ["object"],
  data: function() {
    return {
      text: ''
    };
  }
}
  </script>

<style lang="stylus" scoped>
.q-card {
  margin-bottom: 10px;
}
</style>
