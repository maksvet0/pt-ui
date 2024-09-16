<template>
  <div class="navBar">
    <div class="header">
      <div class="logoHolder">
        <img class="logo" src="../../images/logo/PtLogoLong.svg">
      </div>
      <div class="userAvatarHolder">
        <img class="userAvatar" src="../../images/users/UserAvatar.svg">
      </div>
    </div>
    <div class="menuItems">
      <ButtonLinkWithIcon title="Home" style-class="buttons" >
        <template #icon>
          <img src="@/images/buttons/HomeButton.svg" alt="Home Icon" class="icon" />
        </template>
      </ButtonLinkWithIcon>
      <ButtonLinkWithIcon title="By Themes" style-class="buttons" >
        <template #icon>
          <img src="@/images/buttons/ByThemesButton.svg" alt="ByThemes Icon" class="icon" />
        </template>
      </ButtonLinkWithIcon>
      <img class="spliter" src="@/images/misc/spliterLong.svg"/>
      <ButtonLinkWithIcon title="Blog" style-class="buttons" >
        <template #icon>
          <img src="@/images/buttons/BlogButton.svg" alt="ByThemes Icon" class="icon" />
        </template>
      </ButtonLinkWithIcon>
      <ButtonLinkWithIcon title="Donate" style-class="buttons" >
        <template #icon>
          <img src="@/images/buttons/DonateButton.svg" alt="ByThemes Icon" class="icon" />
        </template>
      </ButtonLinkWithIcon>
      <ButtonLinkWithIcon title="Source" style-class="buttons" >
        <template #icon>
          <img src="@/images/buttons/SourceButton.svg" alt="ByThemes Icon" class="icon" />
        </template>
      </ButtonLinkWithIcon>
      <ButtonLinkWithIcon title="About" style-class="buttons">
        <template #icon>
          <img src="@/images/buttons/AboutButton.svg" alt="ByThemes Icon" class="icon" />
        </template>
      </ButtonLinkWithIcon>
    </div>
  </div>

</template>

<style scoped>

  .spliter{
    margin: 15pt;
    width: 250pt;
  }

  .buttons {
    font-size: 15pt;
    margin-top: 1pt;
  }

  .header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
  }


  .navBar {
    height: 100vh;
    background: #1E1E1E;
    width: fit-content;
    padding-right: 5pt;
    padding-left: 3pt;
  }

  .menuItems {
    display: flex;
    flex-direction: column;
    padding-left: 5pt;
  }

  .userAvatarHolder {
    border-radius: 15pt;
    background: #303030;
  }

  .userAvatar {
    width: 40pt;
    height: 40pt;
    padding: 5pt 5pt 1.5pt 5pt;
  }


  .logoHolder {
    margin: 5pt;
    background-color: #303030;
    padding: 10pt;
    border-radius: 15pt;
    width: 150pt;
    height: 30pt;
    align-items: center;
    display: flex;
  }

</style>
<script setup lang="ts">
import ButtonLinkWithIcon from "@/components/ui/buttons/ButtonLinkWithIcon.vue";
</script>