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
            <p class="joinText">Join Now!</p>
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
        <v-row class="ma-0">
          <v-col class="pa-0">
            <p class="completeText">Complete the following steps to enter</p>
          </v-col>
        </v-row>
        <v-row class="ma-0 d-flex align-center justify-space-between">
          <v-col cols="12" md="6">
            <sweep-widget></sweep-widget>
          </v-col>
          <v-col
            cols="12"
            md="6"
            class="pa-0 goldenHelmetBox d-flex justify-center"
          >
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
            <div class="rectangle">
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
            <div class="rectangle lastTwo">
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
            <div class="rectangle lastTwo">
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

body {
  overflow-x: hidden;
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
  top: -15vw;
  position: absolute;
}

.joinText {
  font-weight: 700;
  font-size: 6.5vw;
  color: #d81159;

  margin: 16vw 0 -20px !important;
}

.dontMissText {
  font-weight: 400;
  font-size: 2.5vw;
  line-height: 34px;
}

.downIcon {
  margin: 7.5vw 0;
}

.v-icon.v-icon {
  font-size: 5vw;
}

.completeText {
  font-weight: 700;
  font-size: 4vw;
  line-height: 57px;

  margin-bottom: 3.5vw !important;
}

.fakeAccordionBox {
  flex-grow: 0;
}

.fakeAccordion {
  border-radius: 12px !important;
  height: 30vw;
  width: 50vw;
  overflow-y: scroll;
}

.goldenHelmetBox {
  flex-grow: 0;
}

.goldenHelmet {
  width: 25vw;
}

.nftText {
  font-weight: 700;
  font-size: 4vw;
  line-height: 57px;

  margin: 11vw 0 2.5vw !important;
}

.allBannersBox {
  display: flex;
  justify-content: space-between;
  margin-bottom: 13vw;
}

.bannerBox {
  width: 24vw;
  flex-grow: 0;
}

.rectangle {
  border-top: solid 1.75vw #d0ad46;
  height: 44vw;
  background-color: #3a3636;
  position: relative;

  padding: 2.5vw 1.75vw;
}

.triangle {
  width: 0;
  height: 0;
  border-left: 12vw solid transparent;
  border-right: 12vw solid transparent;

  border-top: 10vw solid #3a3636;
}

.nftName {
  font-weight: 400;
  font-size: 2.5vw;
  line-height: 34px;
}

.helmetNFT {
  height: 30vw;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
}

.shieldNFT {
  height: 20vw;
  position: absolute;
  top: 50%;
  left: 55.5%;
  transform: translate(-50%, -50%);
  -webkit-transform: translate(-50%, -50%);
}

.swordNFT {
  height: 30vw;
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
@media only screen and (max-width: 500px) {
  .yourView {
    padding: 0 3vw;
  }

  .goldenCar {
    width: 130%;
    min-width: 100px;
    top: -45vw;
    position: absolute;
  }

  .joinText {
    font-weight: 700;
    font-size: 20vw;
    color: #d81159;

    margin: 32.5vw 0 -6vw !important;
  }

  .dontMissText {
    font-weight: 400;
    font-size: 6vw;
    line-height: 8vw;

    padding: 0 3vw;
  }

  .downIcon {
    margin: 17vw 0;
  }

  .v-icon.v-icon {
    font-size: 17vw;
  }

  .completeText {
    font-weight: 700;
    font-size: 9vw;
    line-height: 9vw;

    padding: 0 3vw;
    margin-bottom: 3vw !important;
  }

  .fakeAccordionBox {
    flex-grow: 0;
  }

  .fakeAccordion {
    border-radius: 12px !important;
    height: 500px;
    width: 100vw;
  }

  .goldenHelmetBox {
    flex-grow: 0;
    margin: 10vw auto 0;
  }

  .goldenHelmet {
    width: 45vw;
  }

  .nftText {
    font-weight: 700;
    font-size: 9vw;
    line-height: 9vw;

    padding: 0 3vw;
    margin: 15vw 0 4vw !important;
  }

  .allBannersBox {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 20vw;
  }

  .bannerBox {
    width: 94vw;
    flex-grow: 0;
  }

  .rectangle {
    border-top: solid 6vw #d0ad46;
    height: 175vw;
    background-color: #3a3636;
    position: relative;

    padding: 9vw 6vw;
  }

  .lastTwo {
    border-top: none;
    margin-top: -50vw;
    padding: 12vw 6vw;
    position: relative;
  }

  .lastTwo::after {
    content: "";
    border-top: solid 3vw #d0ad46;
    position: absolute;
    top: 0;
    left: 7vw;
    right: 7vw;
  }

  .triangle {
    width: 0;
    height: 0;
    border-left: 47vw solid transparent;
    border-right: 47vw solid transparent;

    border-top: 40vw solid #3a3636;
  }

  .nftName {
    font-weight: 400;
    font-size: 10vw;
    line-height: 9vw;
  }

  .helmetNFT {
    height: 130vw;
  }

  .shieldNFT {
    height: 120vw;
  }

  .swordNFT {
    height: 130vw;
  }
}
</style>
