<template lang="html">
  <Panel title="精选推荐" :class="$style.panel">
    <section :class="$style.content">
      <div :class="$style.item" v-for="item in items" :key="item.title">
        <dt>{{item.title}} <span :class="$style.red">{{item.sub}}</span></dt>
        <dd>{{item.rate}}</dd>
        <dd>{{item.text}}</dd>
      </div>
    </section>
  </Panel>
</template>

<script>
import Panel from "../core/panel.vue";
export default {
  components: {
    Panel,
  },
  data() {
    return {
      items: [
        {
          title:"定期理财",
          rate:"5.50%",
          text:"历史年化结算利率",
          sub:"90天可质押",
        },
        {
          title:"年年盈",
          rate:"5.80%",
          text:"综合年化收益率",
          sub:"理财推荐",
        },
        {
          title:"机智账户",
          rate:"8%-10%",
          text:"止盈年化收益率",
          sub:"组合投资",
        },
        {
          title:"小白基金",
          rate:"5.00%",
          text:"七日年化收益率",
          sub:"超短期",
        }
      ]
    }
  }
}
</script>

<style lang="scss" module>
@import "../../css/element.scss";
.panel {
  @include panel;
  .content {
    @include list(row);
    &:after{
      content:" ";
      display: block;
      width: 100%;
      height: 0;
      box-sizing: border-box;
      border-bottom: 1px solid #ddd;
      position: relative;
      top: -208px;
    }
    .item {
      width: 50%;
      height: 218px;
      box-sizing: border-box;
      padding-left: 32px;
      position: relative;

      &:after {
        content: " ";
        width: 1px;
        height: 136px;
        display: block;
        position: absolute;
        top: 50%;
        right:0;
        margin-top: -68px;
        border: 1px solid #eee;
      }

      &:nth-child(2n){
        &:after {
          display: none;
        }
      }

      dt {
        font-size:30px;
        line-height: 42px;
        color: #333;
        font-weight: 700;
        margin-top: 34px;
        margin-bottom: 16px;
      }
      dd {
        &:nth-child(2) {
          color: red;
          line-height: 58px;
          color:#ff5155;
          font-size:44px;
          font-weight:700;
        }
        &:nth-child(3) {
          font-size: 24px;
          height: 34px;
          line-height: 34px;
          color: #999;
          white-space: nowrap;
          text-overflow: ellipsis;
          overflow: hidden;
        }
      }
    }
    .red {
      font-size: 22px;
      color: #ff5155;
      border: 1px solid red;
    }
  }

}
</style>
