<template>
  <div class="row">

    <div class="col-md-12">
      <div class="card">
        <history-grid :title="historyTable.title" :sub-title="historyTable.subTitle" :data="historyTable.data">

        </history-grid>
      </div>
    </div>

  </div>
</template>
<script>
  import HistoryGrid from 'components/UIComponents/Grids/HistoryGrid.vue'
  import PaperTable from 'components/UIComponents/PaperTable.vue'
  const tableData = [{
    '#': 1,
    name: 'Dakota Rice',
    summary: '€ 1000',
    'loan %': '5',
    'expected date': '8 December',
    'expected profit': '€ 50'
  }, {
    '#': 2,
    name: 'Dakota Rice',
    summary: '€ 1000',
    'loan %': '5',
    'expected date': '8 December',
    'expected profit': '€ 50'
  }, {
    '#': 3,
    name: 'Dakota Rice',
    summary: '€ 1000',
    'loan %': '5',
    'expected date': '8 December',
    'expected profit': '€ 50'
  }, {
    '#': 4,
    name: 'Dakota Rice',
    summary: '€ 1000',
    'loan %': '5',
    'expected date': '8 December',
    'expected profit': '€ 50'
  }, {
    '#': 5,
    name: 'Dakota Rice',
    summary: '€ 1000',
    'loan %': '5',
    'expected date': '8 December',
    'expected profit': '€ 50'
  }]

  export default {
    components: {
      HistoryGrid,
      PaperTable
    },
    data () {
      return {
        historyTable: {
          title: 'Loan Responses Pack #32',
          subTitle: 'You loaned this companies at 12 November',
          data: [...tableData]
        }
      }
    }
  }

</script>
<style>

</style>
