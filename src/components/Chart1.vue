<template>
  <div class="p-grid p-fluid">
    <div class="p-col-12 p-lg-6">
      <div class="card">
        <h5 class="centerText">Linear Chart</h5>
        <Chart type="line" :data="lineData" />
      </div>
    </div>
  </div>
  <div class="p-grid p-fluid">
    <div class="p-col-12 p-lg-6">
      <div class="card">
        <h5 class="centerText">Linear Chart2</h5>
        <Chart type="line" :data="lineData2" />
      </div>
    </div>
  </div>

    <div class="card">
      <h5>Default</h5>
      <Button label="Submit" class="p-mr-2 p-mb-2"></Button>
    </div>

</template>

<script>
//name: "Chart1"
export default {

    data() {
      return {
        lineData: {
          labels: ['Январь', 'February', 'March', 'April', 'May', 'June', 'July', 'Декабрь'],
          datasets: [
            {
              label: 'Телефония',
              data: [65, 59, 80, 81, 56, 55, 40, 1000],
              fill: false,
              backgroundColor: '#2f4860',
              borderColor: '#2f4860'
            },
            {
              label: 'Аналоговая телефония',
              data: [28, 48, 40, 19, 86, 27, 90],
              fill: false,
              backgroundColor: '#00bb7e',
              borderColor: '#00bb7e'
            }
          ]
        },

        lineData2: {
          labels: ['Январь', 'February', 'March', 'April', 'May', 'June', 'July', 'Декабрь'],
          datasets: [
            {
              label: 'Телефония',
              data: [65, 59, 80, 81, 56, 55, 40, 1000],
              fill: false,
              backgroundColor: '#2f4860',
              borderColor: '#2f4860'
            },
            {
              label: 'Аналоговая телефония',
              data: [28, 48, 40, 19, 86, 27, 90],
              fill: false,
              backgroundColor: '#00bb7e',
              borderColor: '#00bb7e'
            }
          ]
        }




      }
    }
}
</script>

<style scoped>

</style>