<template>
  <v-container class="yourView">
    <v-row class="ma-0">
      <v-col class="pa-0">
        <v-row class="ma-0">
          <v-col class="d-flex justify-center pa-0">
            <img
              src="../assets/images/1_T.png"
              alt="Golden Knight"
              class="goldenCar"
            />
          </v-col>
        </v-row>
        <v-row class="ma-0">
          <v-col class="d-flex justify-center pa-0">
            <p class="joinText mb-n5">Join Now!</p>
          </v-col>
        </v-row>
        <v-row class="ma-0">
          <v-col class="d-flex justify-center pa-0">
            <p class="dontMissText ma-0">
              Don't miss your chance to win one of our NFTs
            </p>
          </v-col>
        </v-row>
        <v-row class="ma-0">
          <v-col class="pa-0 d-flex justify-center align-center">
            <v-icon :color="'#D0AD46'" class="downIcon"
              >mdi-archive-arrow-down-outline</v-icon
            >
          </v-col>
        </v-row>
        <v-row class="ma-0 mb-10">
          <v-col class="pa-0">
            <p class="completeText">Complete the following steps to enter</p>
          </v-col>
        </v-row>
        <v-row class="ma-0 d-flex align-center justify-space-between">
          <v-col class="pa-0" cols="7">
            <v-card class="fakeAccordion pa-4" color="#3a3636">
              <sweep-widget></sweep-widget>
            </v-card>
          </v-col>
          <v-col class="pa-0 goldenHelmetBox">
            <img
              src="../assets/images/Gold_Logo_no_text.png"
              class="goldenHelmet"
              alt="Golden Helmet"
            />
          </v-col>
        </v-row>
        <v-row class="ma-0">
          <v-col class="pa-0">
            <p class="nftText">NFTs you may win</p>
          </v-col>
        </v-row>
        <v-row class="mx-0 mt-0 allBannersBox">
          <v-col class="pa-0 bannerBox">
            <div class="rectangle px-7 py-11">
              <p class="nftName">Helmet</p>
              <img
                src="../assets/images/HeadGearTransparent_1.png"
                alt="Helmet NFT"
                class="helmetNFT"
              />
            </div>
            <div class="triangle"></div>
          </v-col>
          <v-col class="pa-0 bannerBox">
            <div class="rectangle px-7 py-11">
              <p class="nftName">Shield</p>
              <img
                src="../assets/images/CornucopiasShield.png"
                alt="Shield NFT"
                class="shieldNFT"
              />
            </div>
            <div class="triangle"></div>
          </v-col>
          <v-col class="pa-0 bannerBox">
            <div class="rectangle px-7 py-11">
              <p class="nftName">Sword</p>
              <img
                src="../assets/images/SwordRenderStatic2.png"
                alt="Sword NFT"
                class="swordNFT"
              />
            </div>
            <div class="triangle"></div>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import SweepWidget from "@/components/SweepWidget.vue";

export default {
  name: "AboutView",
  components: {
    SweepWidget,
  },
};
</script>

<style>
* {
  font-family: "Domine";
  font-style: normal;
  color: #ffffff;
}

/* .row{                                 Necesito hacer commit para probar si esto sirve o no
  margin: 0 !important;
}

.col{
  padding: 0 !important;
} */

.yourView {
  background-color: #2f2d2e;
  height: fit-content;
  min-width: 100%;
  min-height: 100vh;
  padding: 0 7.5vw;
}

.goldenCar {
  width: 50%;
  min-width: 400px;
  top: -15vw;
  position: absolute;
}

.joinText {
  font-weight: 700;
  font-size: 105px;
  color: #d81159;

  margin-top: 16vw;
}

.dontMissText {
  font-weight: 400;
  font-size: 40px;
  line-height: 34px;
}

.downIcon {
  margin: 120px 0;
}

.v-icon.v-icon {
  font-size: 80px;
}

.completeText {
  font-weight: 700;
  font-size: 65px;
  line-height: 57px;
}

.fakeAccordion {
  border-radius: 12px !important;
  height: 500px;
}

.goldenHelmetBox {
  flex-grow: 0;
}

.goldenHelmet {
  width: 25vw;
}

.nftText {
  font-weight: 700;
  font-size: 65px;
  line-height: 57px;

  margin: 180px 0 40px !important;
}

.allBannersBox {
  display: flex;
  justify-content: space-between;
  margin-bottom: 200px;
}

.bannerBox {
  width: 24vw;
  flex-grow: 0;
}

.rectangle {
  border-top: solid 28px #d0ad46;
  height: 700px;
  background-color: #3a3636;
  position: relative;
}

.triangle {
  width: 0;
  height: 0;
  border-left: 12vw solid transparent;
  border-right: 12vw solid transparent;

  border-top: 160px solid #3a3636;
}

.nftName {
  font-weight: 400;
  font-size: 40px;
  line-height: 34px;
}

.helmetNFT {
  height: 450px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
}

.shieldNFT {
  height: 300px;
  position: absolute;
  top: 50%;
  left: 55.5%;
  transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
}

.swordNFT {
  height: 450px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
}

.outer {
  position: relative;
  width: 100px;
  border: 1px solid black;
  height: 150px;
  margin-left: 100px;
}

img.image {
  width: 200px;
  opacity: 0.7;
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  -webkit-transform: translateX(-50%);
}
@media only screen and (max-width: 450px) {
  .goldenCar {
    top: -25vw;
  }

  .joinText {
    font-weight: 700;
    font-size: 60px;
    color: #d81159;

    margin: 40vw 0 -30px;
  }

  .dontMissText {
    font-weight: 400;
    font-size: 18px;
    line-height: 34px;
  }

  .downIcon {
    margin: 60px 0;
  }

  .v-icon.v-icon {
    font-size: 60px;
  }
}
</style>
