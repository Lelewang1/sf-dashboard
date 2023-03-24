<template>
  <CRow>
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4 month"
        style="min-height: 400px; min-width: 400px; color: white"
      >
        <template #value
          ><h1 style="font-size: 100px; font-weight: bold">
            {{ stats[0]?.value }}
          </h1>
          <!-- <span class="fs-6 fw-normal">
            (+12.4% <CIcon icon="cil-arrow-bottom" />)
          </span> -->
        </template>

        <template #title
          ><h1 style="font-size: 50px; font-weight: bold">
            {{ stats[0]?.title }}
          </h1></template
        >
        <!-- <template #action>
          <CDropdown placement="bottom-end">
            <CDropdownToggle
              color="transparent"
              class="p-0 text-white"
              :caret="false"
            >
              <CIcon icon="cil-options" class="text-high-emphasis-inverse" />
            </CDropdownToggle>
            <CDropdownMenu>
              <CDropdownItem href="#">Action</CDropdownItem>
              <CDropdownItem href="#">Another action</CDropdownItem>
              <CDropdownItem href="#">Something else here</CDropdownItem>
            </CDropdownMenu>
          </CDropdown>
        </template> -->
        <!-- <template #chart>
          <CChart
            type="line"
            class="mt-3 mx-3"
            style="height: 70px"
            :data="{
              labels: [
                'January',
                'February',
                'March',
                'April',
                'May',
                'June',
                'July',
              ],
              datasets: [
                {
                  label: 'My First dataset',
                  backgroundColor: 'transparent',
                  borderColor: 'rgba(255,255,255,.55)',
                  pointBackgroundColor: '#321fdb',
                  data: [68, 59, 84, 84, 51, 55, 40],
                },
              ],
            }"
            :options="{
              plugins: {
                legend: {
                  display: false,
                },
              },
              maintainAspectRatio: false,
              scales: {
                x: {
                  grid: {
                    display: false,
                    drawBorder: false,
                  },
                  ticks: {
                    display: false,
                  },
                },
                y: {
                  min: 30,
                  max: 89,
                  display: false,
                  grid: {
                    display: false,
                  },
                  ticks: {
                    display: false,
                  },
                },
              },
              elements: {
                line: {
                  borderWidth: 1,
                  tension: 0.4,
                },
                point: {
                  radius: 4,
                  hitRadius: 10,
                  hoverRadius: 4,
                },
              },
            }"
          />
        </template> -->
      </CWidgetStatsA>
    </CCol>
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4 month"
        style="min-height: 400px; min-width: 400px; color: white"
      >
        <template #value
          ><h1 style="font-size: 100px; font-weight: bold">
            {{ stats[1]?.value }}
          </h1>
          <span class="fs-6 fw-normal">
            <!-- (-12.4% <CIcon icon="cil-arrow-bottom" />) -->
          </span>
        </template>
        <template #title>
          <h1 style="font-size: 50px; font-weight: bold">
            {{ stats[1]?.title }}
          </h1></template
        >
      </CWidgetStatsA>
    </CCol>
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4 month"
        style="min-height: 400px; min-width: 400px; color: white"
      >
        <template #value
          ><h1 style="font-size: 100px; font-weight: bold">
            {{ stats[2]?.value }}
          </h1>
          <span class="fs-6 fw-normal">
            <!-- (-12.4% <CIcon icon="cil-arrow-bottom" />) -->
          </span>
        </template>
        <template #title>
          <h1 style="font-size: 50px; font-weight: bold">
            {{ stats[2]?.title }}
          </h1></template
        >
      </CWidgetStatsA>
    </CCol>
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4 month"
        style="min-height: 400px; min-width: 400px; color: white"
      >
        <template #value
          ><h1 style="font-size: 100px; font-weight: bold">
            {{ stats[3]?.value }}
          </h1>
          <span class="fs-6 fw-normal">
            <!-- (-12.4% <CIcon icon="cil-arrow-bottom" />) -->
          </span>
        </template>
        <template #title
          ><h1 style="font-size: 50px; font-weight: bold">
            {{ stats[3]?.title }}
          </h1></template
        >
      </CWidgetStatsA>
    </CCol>
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4 year"
        style="min-height: 400px; min-width: 400px; color: white"
      >
        <template #value
          ><h1 style="font-size: 100px; font-weight: bold">
            {{ stats[4]?.value }}
          </h1>
          <span class="fs-6 fw-normal">
            <!-- (-12.4% <CIcon icon="cil-arrow-bottom" />) -->
          </span>
        </template>
        <template #title
          ><h1 style="font-size: 50px; font-weight: bold">
            {{ stats[4]?.title }}
          </h1></template
        >
      </CWidgetStatsA>
    </CCol>

    <!-- income -->
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4 year"
        style="min-height: 400px; min-width: 400px; color: white"
      >
        <template #value
          ><h1 style="font-size: 100px; font-weight: bold">
            {{ stats[5]?.value }}
          </h1>
          <span class="fs-6 fw-normal">
            <!-- (40.9% <CIcon icon="cil-arrow-top" />) -->
          </span>
        </template>
        <template #title
          ><h1 style="font-size: 50px; font-weight: bold">
            {{ stats[5]?.title }}
          </h1></template
        >
        <template #action>
          <!-- <CDropdown placement="bottom-end">
            <CDropdownToggle
              color="transparent"
              class="p-0 text-white"
              :caret="false"
            >
              <CIcon icon="cil-options" class="text-high-emphasis-inverse" />
            </CDropdownToggle>
            <CDropdownMenu>
              <CDropdownItem href="#">Action</CDropdownItem>
              <CDropdownItem href="#">Another action</CDropdownItem>
              <CDropdownItem href="#">Something else here</CDropdownItem>
            </CDropdownMenu>
          </CDropdown> -->
        </template>
        <!-- <template #chart>
          <CChart
            type="line"
            class="mt-3 mx-3"
            style="height: 70px"
            :data="{
              labels: [
                'January',
                'February',
                'March',
                'April',
                'May',
                'June',
                'July',
              ],
              datasets: [
                {
                  label: 'My First dataset',
                  backgroundColor: 'transparent',
                  borderColor: 'rgba(255,255,255,.55)',
                  pointBackgroundColor: '#39f',
                  data: [1, 18, 9, 17, 34, 22, 11],
                },
              ],
            }"
            :options="{
              plugins: {
                legend: {
                  display: false,
                },
              },
              maintainAspectRatio: false,
              scales: {
                x: {
                  grid: {
                    display: false,
                    drawBorder: false,
                  },
                  ticks: {
                    display: false,
                  },
                },
                y: {
                  min: -9,
                  max: 39,
                  display: false,
                  grid: {
                    display: false,
                  },
                  ticks: {
                    display: false,
                  },
                },
              },
              elements: {
                line: {
                  borderWidth: 1,
                },
                point: {
                  radius: 4,
                  hitRadius: 10,
                  hoverRadius: 4,
                },
              },
            }"
          />
        </template> -->
      </CWidgetStatsA>
    </CCol>
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4 year"
        style="min-height: 400px; min-width: 400px; color: white"
      >
        <template #value
          ><h1 style="font-size: 100px; font-weight: bold">
            {{ stats[6]?.value }}
          </h1>
          <span class="fs-6 fw-normal">
            <!-- (84.7% <CIcon icon="cil-arrow-top" />) -->
          </span>
        </template>
        <template #title
          ><h1 style="font-size: 50px; font-weight: bold">
            {{ stats[6]?.title }}
          </h1></template
        >
        <!-- <template #action>
          <CDropdown placement="bottom-end">
            <CDropdownToggle
              color="transparent"
              class="p-0 text-white"
              :caret="false"
            >
              <CIcon icon="cil-options" class="text-high-emphasis-inverse" />
            </CDropdownToggle>
            <CDropdownMenu>
              <CDropdownItem href="#">Action</CDropdownItem>
              <CDropdownItem href="#">Another action</CDropdownItem>
              <CDropdownItem href="#">Something else here</CDropdownItem>
            </CDropdownMenu>
          </CDropdown>
        </template>
        <template #chart>
          <CChart
            type="line"
            class="mt-3"
            style="height: 70px"
            :data="{
              labels: [
                'January',
                'February',
                'March',
                'April',
                'May',
                'June',
                'July',
              ],
              datasets: [
                {
                  label: 'My First dataset',
                  backgroundColor: 'rgba(255,255,255,.2)',
                  borderColor: 'rgba(255,255,255,.55)',
                  data: [78, 81, 80, 45, 34, 12, 40],
                  fill: true,
                },
              ],
            }"
            :options="{
              plugins: {
                legend: {
                  display: false,
                },
              },
              maintainAspectRatio: false,
              scales: {
                x: {
                  display: false,
                },
                y: {
                  display: false,
                },
              },
              elements: {
                line: {
                  borderWidth: 2,
                  tension: 0.4,
                },
                point: {
                  radius: 0,
                  hitRadius: 10,
                  hoverRadius: 4,
                },
              },
            }"
          />
        </template> -->
      </CWidgetStatsA>
    </CCol>
    <CCol :xs="6">
      <CWidgetStatsA
        class="mb-4"
        style="
          min-height: 400px;
          min-width: 400px;
          background-color: #ffa200;
          color: white;
        "
      >
        <template #value>
          <h1 style="font-size: 100px; font-weight: bold">
            {{ stats[7]?.value }}
          </h1>
          <span class="fs-6 fw-normal">
            <!-- (-23.6% <CIcon icon="cil-arrow-bottom" />) -->
          </span>
        </template>
        <template #title
          ><h1 style="font-size: 50px; font-weight: bold">
            {{ stats[7]?.title }}
          </h1></template
        >
        <!-- <template #action>
          <CDropdown placement="bottom-end">
            <CDropdownToggle
              color="transparent"
              class="p-0 text-white"
              :caret="false"
            >
              <CIcon icon="cil-options" class="text-high-emphasis-inverse" />
            </CDropdownToggle>
            <CDropdownMenu>
              <CDropdownItem href="#">Action</CDropdownItem>
              <CDropdownItem href="#">Another action</CDropdownItem>
              <CDropdownItem href="#">Something else here</CDropdownItem>
            </CDropdownMenu>
          </CDropdown>
        </template>
        <template #chart>
          <CChart
            type="bar"
            class="mt-3 mx-3"
            style="height: 70px"
            :data="{
              labels: [
                'January',
                'February',
                'March',
                'April',
                'May',
                'June',
                'July',
                'August',
                'September',
                'October',
                'November',
                'December',
                'January',
                'February',
                'March',
                'April',
              ],
              datasets: [
                {
                  label: 'My First dataset',
                  backgroundColor: 'rgba(255,255,255,.2)',
                  borderColor: 'rgba(255,255,255,.55)',
                  data: [
                    78, 81, 80, 45, 34, 12, 40, 85, 65, 23, 12, 98, 34, 84, 67,
                    82,
                  ],
                  barPercentage: 0.6,
                },
              ],
            }"
            :options="{
              maintainAspectRatio: false,
              plugins: {
                legend: {
                  display: false,
                },
              },
              scales: {
                x: {
                  grid: {
                    display: false,
                    drawTicks: false,
                  },
                  ticks: {
                    display: false,
                  },
                },
                y: {
                  grid: {
                    display: false,
                    drawBorder: false,
                    drawTicks: false,
                  },
                  ticks: {
                    display: false,
                  },
                },
              },
            }"
          />
        </template> -->
      </CWidgetStatsA>
    </CCol>
  </CRow>
</template>

<script>
// import { CChart } from '@coreui/vue-chartjs'
export default {
  name: 'WidgetsStatsA',
  components: {
    // CChart,
  },
  data() {
    return {
      stats: [],
    }
  },
  methods: {
    async refresh() {
      const res = await fetch('api/data')
      const data = await res.json()
      return data
    },
  },
  async created() {
    this.stats = await this.refresh()
    setInterval(async () => {
      this.stats = await this.refresh()
    }, 1800000)
  },
}
</script>

<style scoped>
/* .month {
  background-color: #005FE5;
}

.year {
  background-color: #00B9A3;
} */

.month {
  background-color: #00b9a3;
}

.year {
  background-color: #363636;
}
</style>
