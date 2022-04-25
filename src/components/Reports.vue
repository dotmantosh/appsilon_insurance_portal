<template>
  <div class="reports">
    <div class="reports__top">
      <img
        src="../assets/imgs/Insurance_-Agent-_Service_VectorForFree- 1.png"
        alt="imgss"
      />
      <Area2 class="area-2" />
      <Area3 class="area-3" />
      <div class="reports__top--info">
        <h2>20% Safe On Your First Account</h2>
        <div class="copy-code">
          <div class="code">NEWBIE20</div>
          <p>Copy Code</p>
        </div>
      </div>
    </div>
    <div class="reports__items">
      <div class="reports__items--item">
        <h2 class="item-total">1000<span>$</span></h2>
        <p class="item-p mb-0">Total Value of Disbustment</p>

        <div class="policy">
          <div class="policy__top">
            <p class="policy-p">Policy</p>
            <p class="policy-total mb-0">400<span>$</span></p>
          </div>
          <div class="policy__progress">
            <div class="policy__progress--inner"></div>
          </div>
        </div>

        <div class="claim">
          <div class="claim__top">
            <p class="claim-p">claim</p>
            <p class="claim-total mb-0">400<span>$</span></p>
          </div>
          <div class="claim__progress">
            <div class="claim__progress--inner"></div>
          </div>
        </div>
      </div>
      <div class="reports__items--item">
        <h2 class="item-total">2500<span>$</span></h2>
        <p class="item-p mb-0">Total Value of Disbustment</p>

        <div class="policy">
          <div class="policy__top">
            <p class="policy-p">Policy</p>
            <p class="policy-total mb-0">400<span>$</span></p>
          </div>
          <div class="policy__progress">
            <div class="policy__progress--inner"></div>
          </div>
        </div>

        <div class="claim">
          <div class="claim__top">
            <p class="claim-p">claim</p>
            <p class="claim-total mb-0">400<span>$</span></p>
          </div>
          <div class="claim__progress">
            <div class="claim__progress--inner"></div>
          </div>
        </div>
      </div>
      <div class="reports__items--item">
        <h2 class="item-total">2500<span>$</span></h2>
        <p class="item-p mb-0">Total Value of Disbustment</p>

        <div class="policy">
          <div class="policy__top">
            <p class="policy-p">Policy</p>
            <p class="policy-total mb-0">400<span>$</span></p>
          </div>
          <div class="policy__progress">
            <div class="policy__progress--inner"></div>
          </div>
        </div>

        <div class="claim">
          <div class="claim__top">
            <p class="claim-p">claim</p>
            <p class="claim-total mb-0">400<span>$</span></p>
          </div>
          <div class="claim__progress">
            <div class="claim__progress--inner"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Area2 from "../assets/svgs/Area2.vue";
import Area3 from "../assets/svgs/Area3.vue";
export default {
  components: {
    Area2,
    Area3,
  },
};
</script>

<style scoped lang="scss">
.reports {
  margin-top: 36px;
  margin-left: 38px;
  margin-right: 38px;
  &__top {
    max-width: 98.1rem;
    position: relative;
    background-color: #f8f9ff;
    box-shadow: 0px 0px 15px rgba($color: #000000, $alpha: 0.15);

    .area-2 {
      position: absolute;
      top: 43px;
      left: 0;
      opacity: 0.1;
    }
    .area-3 {
      position: absolute;
      top: 80px;
      left: 0;
      opacity: 0.1;
    }

    &--info {
      position: absolute;
      top: 50%;
      right: 90px;
      transform: translateY(-50%);

      h2 {
        font-weight: 600;
        font-size: 3.3rem;
        line-height: 44px;
        color: var(--app-grey-1);
        margin-bottom: 3px;
      }

      .copy-code {
        display: flex;
        align-items: center;
        width: max-content;
        margin: 0 auto;

        .code {
          font-size: 22px;
          color: var(--app-grey-1);
          padding: 7px 13px;
          border: 1px dashed var(--app-grey-1);
          border-radius: 5px;
        }

        p {
          font-size: 2rem;
          font-weight: 600;
          margin-left: 20px;
          color: var(--app-grey-1);
        }
      }
    }
  }

  &__items {
    margin-top: 20px;
    max-width: 98.1rem;
    display: flex;
    justify-content: space-between;

    &--item {
      width: 314px;
      height: 298px;
      background-color: #fff;
      border-radius: 4px;
      box-shadow: 3px 3px 4px rgba($color: #000000, $alpha: 0.06);
      padding: 28px;
      padding-top: 3px;

      .item-total {
        font-weight: 400;
        font-size: 55px;
        line-height: 73px;
        color: var(--app-grey-1);
        position: relative;
        width: max-content;
        span {
          position: absolute;
          top: -15px;
          right: -18px;
          font-size: 35px;
          color: var(--app-purple-1);
        }
      }
      .item-p {
        font-weight: 400;
        font-size: 17px;
        line-height: 23px;
        color: var(--app-grey-1);
        margin-top: 3px;
      }
    }
    .policy {
      margin-top: 45px;
      &__top {
        display: flex;
        justify-content: space-between;
        .policy-p {
          font-size: 17px;
          color: var(--app-grey-1);
          margin-bottom: 8px;
        }

        .policy-total {
          font-size: 22px;
          color: var(--app-grey-1);
          position: relative;
          margin-bottom: 8px;
          span {
            font-size: 13px;
            color: var(--app-purple-1);
            position: absolute;
            top: -0px;
            right: -8px;
          }
        }
      }
      &__progress {
        background-image: linear-gradient(
          to right,
          #ececec,
          #f2f1f1
        ) !important;
        border-radius: 2px;
        height: 5px;
        &--inner {
          background-image: linear-gradient(
            to right,
            #33d69f,
            #50edb8
          ) !important;
          width: 60%;
          border-radius: 2px;
          height: 5px;
        }
      }
    }
    .claim {
      margin-top: 40px;
      &__top {
        display: flex;
        justify-content: space-between;
        .claim-p {
          font-size: 17px;
          color: var(--app-grey-1);
          margin-bottom: 8px;
        }

        .claim-total {
          margin-bottom: 8px;
          font-size: 22px;
          color: var(--app-grey-1);
          position: relative;
          span {
            font-size: 13px;
            color: var(--app-purple-1);
            position: absolute;
            top: -0px;
            right: -8px;
          }
        }
      }
      &__progress {
        background-image: linear-gradient(
          to right,
          #ececec,
          #f2f1f1
        ) !important;
        border-radius: 2px;
        height: 5px;
        &--inner {
          width: 80%;
          background-image: linear-gradient(
            to right,
            #713bdb,
            #a886e9
          ) !important;
          border-radius: 2px;
          height: 5px;
        }
      }
    }
  }
}
</style>
