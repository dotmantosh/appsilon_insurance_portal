<template>
  <div class="sidebar">
    <div class="logo">
      <div class="logo__div">
        <img src="../assets/imgs/logo.png" class="logo__img" alt="logo">
      </div>
      <h2 class="logo__name">Insurance Portal</h2>
    </div>
    
    <div class="profile">
      <div class="profile__img--div">
        <img src="../assets/imgs/profileimg.png" alt="profile-img" class="profile__img--img">
      </div>
      <h2 class="profile__name">Hello ! {{name}}</h2>
      <p class="profile__welcome">Welcome Back To Your Insurance Portal</p>
      <p class="profile__plan">Your Plan : <span class="plan">Free</span></p>
      <button class="profile__create--btn">Create New Plan <span>+</span></button>
    </div>

    <div class="side-tab">
      <div class="side-tab__item">
        <OverviewIcon/>
        <p class="mb-0">Overview</p>
      </div>
      <div class="side-tab__item">
        <PolicyIcon/>
        <p class="mb-0">Policy</p>
      </div>
      <div class="side-tab__item">
        <ReportIcon/>
        <p class="mb-0">Report</p>
      </div>
      <div class="side-tab__item">
        <CompanyIcon/>
        <p class="mb-0">Company</p>
      </div>
      <div class="side-tab__item">
        <UserAccountIcon/>
        <p class="mb-0">User Account</p>
      </div>
      <div class="side-tab__item">
        <HistoryIcon/>
        <p class="mb-0">History</p>
      </div>
    </div>

    <div class="logout">
      <LogoutIcon/>
      <p class="mb-0">Log Out</p>
    </div>
  </div>
</template>

<script>
import CompanyIcon from "./icons/Company.vue"
import PolicyIcon from "./icons/Policy.vue"
import OverviewIcon from "./icons/Overview.vue"
import ReportIcon from "./icons/Report.vue"
import UserAccountIcon from "./icons/UserAccount.vue"
import HistoryIcon from "./icons/History.vue"
import LogoutIcon from "./icons/Logout.vue"
export default {
  components:{
    OverviewIcon,
    PolicyIcon,
    ReportIcon,
    CompanyIcon,
    UserAccountIcon,
    HistoryIcon,
    LogoutIcon
  },
  data(){
    return{
      name: "Rusalba Ruiz"
    }
  }
}
</script>

<style lang="scss" scoped>
  .sidebar{
    position: relative;
    width: 30.6rem;
    background-color: #fff;
    min-height: 90vh;
    border-top-left-radius: 20px;
    border-bottom-left-radius: 20px;
    box-shadow: 10px 3px 15px rgba($color: #000000, $alpha: 0.05);
  }

  .logo{
    width: max-content;
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 3rem;
    &__name{
      margin-left: 11px;
      font-size: 1.6rem;
      color: #000;
      font-weight: 600;
      line-height: 21px;
    }
  }

  .profile{
    width: max-content;
    margin: 0 auto;
    &__img--div{
      width: max-content;
      margin: 0 auto;
      margin-top: 22px;
    }
    &__name{
      font-size: 16px;
      font-weight: 700;
      line-height: 21px;
      color: #888cb7;
      text-align: center;
      
    }
    &__welcome{
      font-weight: 400;
      font-size: 1rem;
      line-height: 13px;
      color: var(--app-purple-2);
      margin-top: 4px;
      text-align: center;
    }
    &__plan{
      font-weight: 400;
      font-size: 14px;
      line-height: 19px;
      text-align: center;
      margin-top: 3px;
      color: var(--app-purple-2);
      .plan{
        color: #33d69f;
      }
    }
    &__create--btn{
      display: block;
      margin: 0 auto;
      width: 168px;
      height: 35px;
      text-align: center;
      color: #fff;
      font-size: 14px;
      background-color: var(--app-purple-1);
      box-shadow: 0px 4px 4px rgba($color: #000000, $alpha: 0.12);
      margin-top: 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;

      span{
        margin-left: 14px;
      }

      &:active{
        transform: translateY(2px);
      }
    }
  }

  .side-tab{
    width: max-content;
    margin: 0 auto;
    margin-top: 57px;

    &__item{
      display: flex;
      align-items: center;
      margin-bottom: 28px;
      cursor: pointer;

      p{
        margin-left: 25px;
        font-weight: 400;
        font-size: 16px;
        line-height: 21px;
      }
    }
  }

  .logout{
    display: flex;
    align-items: center;
    position: absolute;
    bottom: 33px;
    left: 50%;
    transform: translateX(-50%);
    cursor: pointer;
    p{
      font-weight: 400;
      font-size: 18px;
      line-height: 24px;
      margin-left: 15px;
      color: var(--app-purple-2);
    }
  }
</style>
