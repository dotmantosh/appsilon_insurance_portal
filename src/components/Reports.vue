<template>
  <div class="reports">
    <div class="reports__top">
      <img src="../assets/imgs/Insurance_-Agent-_Service_VectorForFree- 1.png" alt="imgss"> 
      <Area2 class="area-2"/>
      <Area3 class="area-3"/>
      <div class="reports__top--info">
        <h2>20% Safe On Your First Account</h2>
        <div class="copy-code">
          <div class="code">NEWBIE20</div>
          <p>Copy Code</p>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import Area2 from '../assets/svgs/Area2.vue'
import Area3 from '../assets/svgs/Area3.vue'
export default {
  components:{
    Area2,
    Area3
  }
}
</script>

<style scoped lang="scss">
.reports{
  margin-top: 36px;
  margin-left: 38px;
  margin-right: 38px;
  &__top{
    max-width: 98.1rem;
    position: relative;
    background-color: #f8f9ff;
    box-shadow: 0px 0px 15px rgba($color: #000000, $alpha: 0.15);

    .area-2{
      position: absolute;
      top: 43px;
      left: 0;
      opacity: 0.1;
    }
    .area-3{
      position: absolute;
      top: 80px;
      left: 0;
      opacity: 0.1;
    }

    &--info{
      position: absolute;
      top: 50%;
      right: 90px;
      transform: translateY(-50%);

      h2{
        font-weight: 600;
        font-size: 3.3rem;
        line-height: 44px;
        color: var(--app-grey-1);
        margin-bottom: 3px;
      }

      .copy-code{
        display: flex;
        align-items: center;
        width: max-content;
        margin: 0 auto;

        .code{
          font-size: 22px;
          color: var(--app-grey-1);
          padding: 7px 13px;
          border: 1px dashed var(--app-grey-1);
          border-radius: 5px;
        
        }

        p{
          font-size: 2rem;
          font-weight: 600;
          margin-left: 20px;
          color: var(--app-grey-1);
        }
      }
    }

  }
}



</style>