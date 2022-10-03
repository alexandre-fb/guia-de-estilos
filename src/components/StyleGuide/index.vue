<template>

    <div class="tab-container">

      <ul class="tab-header">
        <li class="tab-header__item" :class="activeTabName == tabNames.tab1 ? 'tab-header__item--active item--active--analytics' : ''" @click="handleTabClick(tabNames.tab1) ">
          {{tabNames.tab1}}
        </li>
        <li class="tab-header__item" :class="activeTabName == tabNames.tab2 ? 'tab-header__item--active item--active--portal' : ''" @click="handleTabClick(tabNames.tab2)">
          {{tabNames.tab2}}
        </li>
      </ul>

      <div class="tab-content" :class="`tab-content--active--${activeTabName}`">
        <AnalyticsStyleGuide v-if="activeTabName === tabNames.tab1" />
        <PortalStyleGuide v-if="activeTabName === tabNames.tab2" />
      </div>
    </div>


</template>

<script>
import AnalyticsStyleGuide from './tabsComponents/AnalyticsStyleGuide.vue'
import PortalStyleGuide from './tabsComponents/PortalStyleGuide copy.vue'

const tabNames = { 
  tab1: 'Analytics',
  tab2: 'Portal',
}

export default {
  name: 'GuiaDeEstilo',
  components: {
    AnalyticsStyleGuide, 
    PortalStyleGuide
  },
  data() {
    return {
      activeTabName: tabNames.tab1,
      tabNames,
    }
  },
  methods: {
    handleTabClick(tabName) {
      this.activeTabName = tabName
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">


  .tab-container {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;

    .tab-header {
      padding: 0;
      margin: 0;
      display: flex;
      list-style: none;
      font-size: 18px;

      .tab-header__item {
        padding: 10px 15px;
        cursor: pointer;
        transition: 300ms ease;
        border-radius: 0 5px 0 0;
        background-color: rgb(246, 246, 246);
        
        &:hover {
          background-color: #dfdfdfc9;
        }
      }

      .tab-header__item--active {
        color: #fff;
        font-weight: 500;
      }

      .item--active--analytics {
        background-color: #00afef !important;
      }

      .item--active--portal {
        background-color: #252642 !important;
      }
    }

    .tab-content {
      width: 100%;
      max-width: 1200px;
      background-color: rgb(246, 246, 246);
      border-radius: 0 10px 10px 10px;
      display: flex;
      transition: 300ms ease;
      padding: 20px;
    }
  }

</style>