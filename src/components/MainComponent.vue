<template>
  <div>
    <NavBar :language="language" />
    <div class="max-width">
      <Header
        :imagesSrcArray="headerImagesSrcArray"
        :textArray="headerTextArray"
        :buttonTextArray="buttonTextArray"
      />
      <BaseContentWithImages :imagesSrcArray="topContentImagesSrcArray" />
      <BaseHeader :text="sportsCategoriesText" />
      <SportsCategories
        :iconsSrcArray="sportsCategoriesIconsSrcArray"
        :iconsTextArray="sportsCategoriesIconsTextArray"
      />
      <BaseHeader :text="promotionsText" />
      <BaseContentWithImages :imagesSrcArray="promotionsContentImagesSrcArray" />
      <BaseHeader :text="gameProvidersText" />
      <GameProviders :imageSrcArray="gameProvidersImageSrcArray" />
      <Footer
        :headerTextArray="footerTextArray"
        :text2dArray="footerText2dArray"
        :socialHeaderText="footerSocialHeaderText"
        :socialImagesSrcArray="footerSocialImagesSrcArray"
      />
    </div>
  </div>
</template>

<script>
import NavBar from "./NavBar.vue";
import Header from "./Header.vue";
import BaseContentWithImages from "./BaseContentWithImages.vue";
import BaseHeader from "./BaseHeader.vue";
import SportsCategories from "./SportsCategories.vue";
import GameProviders from "./GameProviders.vue";
import Footer from "./Footer.vue";

export default {
  name: "MainComponent",
  components: {
    NavBar,
    Header,
    BaseContentWithImages,
    BaseHeader,
    SportsCategories,
    GameProviders,
    Footer
  },
  data() {
    return {
      language: "English",
      headerTextArray: ["Main Club Partner", "Official Shirt Sponsor"],
      headerImagesSrcArray: [require("@/assets/images/partner.jpg"), require("@/assets/images/sponsor.jpg")],
      buttonTextArray: ["Sign in", "Register"],
      topContentImagesSrcArray: [require("@/assets/images/main image 1.jpg"), require("@/assets/images/main image 2.jpg")],
      promotionsContentImagesSrcArray: [require("@/assets/images/main image 3.jpg"), require("@/assets/images/main image 4.jpg")],
      sportsCategoriesText: "Sports categories",
      sportsCategoriesIconsSrcArray: [
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
        require("@/assets/images/sport icon.jpg"),
      ],
      sportsCategoriesIconsTextArray: [
        "Soccer",
        "Basketball",
        "Tennis",
        "Ice Hockey",
        "Baseball",
        "Cricket",
        "American Football",
        "Australian Rules",
        "Badmington",
        "Bandy",
        "Beach Volley",
        "Biathlon",
        "Boxing",
        "Call of Duty",
        "CS:GO",
        "Darts",
        "Data 2",
        "Floorball",
      ],
      promotionsText: "Exciting promotions start here",
      gameProvidersText: "Game Providers",
      gameProvidersImageSrcArray: [
        require("@/assets/images/game providers.jpg"),
        require("@/assets/images/game providers.jpg"),
        require("@/assets/images/game providers.jpg"),
        require("@/assets/images/game providers.jpg"),
        require("@/assets/images/game providers.jpg"),
        require("@/assets/images/game providers.jpg")
      ],
      footerTextArray: ["Sports", "Casino", "Support", "About"],
      footerText2dArray: [
        [
          {
            linkText: "Promotions",
            href: "sports1"
          },
          {
            linkText: "In play",
            href: "sports2"
          },
          {
            linkText: "Upcomming",
            href: "sports3"
          }
        ],
        [
          {
            linkText: "Live Casino",
            href: "casino"
          }
        ],
        [
          {
            linkText: "Payment Options",
            href: "support1"
          },
          {
            linkText: "Responsible",
            href: "support2"
          },
          {
            linkText: "Gambling",
            href: "support3"
          },
          {
            linkText: "FAQ",
            href: "support4"
          },
          {
            linkText: "General Betting",
            href: "support5"
          },
          {
            linkText: "Rules",
            href: "support6"
          },
          {
            linkText: "Responsible",
            href: "support7"
          },
          {
            linkText: "Gambling Terms and Conditions",
            href: "support8"
          },
          {
            linkText: "Affiliate FAQ",
            href: "support9"
          },
          {
            linkText: "Sportsbet Market",
            href: "support10"
          },
          {
            linkText: "Explanations",
            href: "support11"
          },
        ],
        [
          {
            linkText: "Privacy Policy",
            href: "about1"
          },
          {
            linkText: "About Us",
            href: "about2"
          },
          {
            linkText: "Terms and Conditions",
            href: "about3"
          },
          {
            linkText: "Affiliates",
            href: "about4"
          },
          {
            linkText: "Affiliate Terms and Conditions",
            href: "about5"
          },
          {
            linkText: "Sportsbet.io",
            href: "about6"
          },
          {
            linkText: "Partnerships",
            href: "about7"
          },
          {
            linkText: "Bug Bounty",
            href: "about8"
          },
          {
            linkText: "Program",
            href: "about9"
          },
        ]
      ],
      footerSocialHeaderText: "Follow us",
      footerSocialImagesSrcArray: [
        require("@/assets/images/tweeter.jpg"),
        require("@/assets/images/tweeter.jpg"),
        require("@/assets/images/tweeter.jpg"),
        require("@/assets/images/tweeter.jpg"),
        require("@/assets/images/tweeter.jpg")
      ]
    };
  }
};
</script>
