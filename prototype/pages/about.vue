<template>
  <div class="about">
    <section>
      <v-layout
      column
      wrap
      class="my-5"
      align-center
      text-xs-center
      >
      <div class=" my-5">
        <v-flex xs12 class="my-5 mx-3">
          <h1 class="headline text-xs-center">会社概要</h1>
          <v-jumbotron xs8 offset-xs2 height="auto">
            <v-flex class="mb-5 text-xs-left">
              <h1>MISSION</h1>
              <br />
              <span>物語との出会いを通して、人類に感動する機会を提供する</span>
            </v-flex>
            <v-flex class="mb-4 text-xs-left">
              <h1>会社概要</h1>
            </v-flex>
            <v-data-table
            :items="items"
            hide-actions
            hide-headers
            >
            <template slot="items" slot-scope="props">
              <td class="text-xs-center">{{ props.item.calories }}</td>
              <td class="text-xs-left">{{ props.item.name }}</td>
            </template>
          </v-data-table>
        </v-jumbotron>
      </v-flex>
    </div>
  </v-layout>
</section>
</div>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          value: false,
          calories: '社名',
          name: '株式会社viviane'
        },
        {
          value: false,
          calories: '設立',
          name: '2012年3月14日'
        },
        {
          value: false,
          calories: '事業内容',
          name: 'Webサービスの企画・開発・運営'
        },
        {
          value: false,
          calories: '所在地',
          name: '〒150-0032 東京都渋谷区鶯谷町3-1 SUビル203'
        }
      ]
    }
  }
}
</script>
