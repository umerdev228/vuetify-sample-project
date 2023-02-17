<template>
  <v-col cols="12">
    <v-card>

      <v-col cols="12">
        <v-row class="d-flex align-items-center justify-space-between">
          <div>
            <v-row>
              <v-select
                class="mr-1"
                variant="solo"
                :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
                v-model="val"
              ></v-select>
              <v-select
                class="mr-1"
                variant="solo"
                v-model="val"
                :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
              ></v-select>
              <v-select
                class="mr-1"
                variant="solo"
                v-model="val"
                :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
              ></v-select>
            </v-row>
          </div>
          <v-col cols="2">
            <v-text-field
              density="compact"
              variant="solo"
              label="Search"
              append-inner-icon="mdi-magnify"
              single-line
              hide-details
            ></v-text-field>
          </v-col>
        </v-row>
      </v-col>
      <v-card-item>
        <v-table theme="dark">
          <thead>
          <tr>
            <th class="text-left">
              Title
            </th>
            <th class="text-left">
              Highest Bidder
            </th>
            <th class="text-left">
              Auction Time
            </th>
            <th class="text-left">
              Highest Bid
            </th>
            <th class="text-left">
              Action
            </th>
            <th class="text-left">
              Calories
            </th>
          </tr>
          </thead>
          <tbody>
          <tr
            v-for="item in desserts"
            :key="item.name"
          >
            <td>{{ item.name }}</td>
            <td>{{ item.calories }}</td>
            <td>{{ item.calories }}</td>
            <td>{{ item.calories }}</td>
            <td>{{ item.calories }}</td>
            <td>{{ item.calories }}</td>
          </tr>
          </tbody>
        </v-table>
      </v-card-item>
    </v-card>
  </v-col>

  <!--  <v-container class="fill-height">-->
  <!--    <v-responsive class="d-flex align-center text-center fill-height">-->
  <!--      <v-img-->
  <!--        contain-->
  <!--        height="300"-->
  <!--        src="@/assets/logo.svg"-->
  <!--      />-->

  <!--      <div class="text-body-2 font-weight-light mb-n1">Welcome to</div>-->

  <!--      <h1 class="text-h2 font-weight-bold">Vuetify</h1>-->

  <!--      <div class="py-14" />-->

  <!--      <v-row class="d-flex align-center justify-center">-->
  <!--        <v-col cols="auto">-->
  <!--          <v-btn-->
  <!--            href="https://next.vuetifyjs.com/components/all/"-->
  <!--            min-width="164"-->
  <!--            rel="noopener noreferrer"-->
  <!--            target="_blank"-->
  <!--            variant="text"-->
  <!--          >-->
  <!--            <v-icon-->
  <!--              icon="mdi-view-dashboard"-->
  <!--              size="large"-->
  <!--              start-->
  <!--            />-->

  <!--            Components-->
  <!--          </v-btn>-->
  <!--        </v-col>-->

  <!--        <v-col cols="auto">-->
  <!--          <v-btn-->
  <!--            color="primary"-->
  <!--            href="https://next.vuetifyjs.com/introduction/why-vuetify/#feature-guides"-->
  <!--            min-width="228"-->
  <!--            rel="noopener noreferrer"-->
  <!--            size="x-large"-->
  <!--            target="_blank"-->
  <!--            variant="flat"-->
  <!--          >-->
  <!--            <v-icon-->
  <!--              icon="mdi-speedometer"-->
  <!--              size="large"-->
  <!--              start-->
  <!--            />-->

  <!--            Get Started-->
  <!--          </v-btn>-->
  <!--        </v-col>-->

  <!--        <v-col cols="auto">-->
  <!--          <v-btn-->
  <!--            href="https://community.vuetifyjs.com/"-->
  <!--            min-width="164"-->
  <!--            rel="noopener noreferrer"-->
  <!--            target="_blank"-->
  <!--            variant="text"-->
  <!--          >-->
  <!--            <v-icon-->
  <!--              icon="mdi-account-group"-->
  <!--              size="large"-->
  <!--              start-->
  <!--            />-->

  <!--            Community-->
  <!--          </v-btn>-->
  <!--        </v-col>-->
  <!--      </v-row>-->
  <!--    </v-responsive>-->
  <!--  </v-container>-->
</template>

<script setup>
//
let val = 'California'
const desserts = [
  {
    name: 'Frozen Yogurt',
    calories: 159,
  },
  {
    name: 'Ice cream sandwich',
    calories: 237,
  },
  {
    name: 'Eclair',
    calories: 262,
  },
  {
    name: 'Cupcake',
    calories: 305,
  },
  {
    name: 'Gingerbread',
    calories: 356,
  },
  {
    name: 'Jelly bean',
    calories: 375,
  },
  {
    name: 'Lollipop',
    calories: 392,
  },
  {
    name: 'Honeycomb',
    calories: 408,
  },
  {
    name: 'Donut',
    calories: 452,
  },
  {
    name: 'KitKat',
    calories: 518,
  },
]

</script>
