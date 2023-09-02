<script>
export default {
  data() {
    return {
      columns: [
        {
          title: "Address",
          items: ["Item 1", "Item 2", "Item 3"],
        },
        {
          title: "Explore",
          items: [
            ["Item 4", "Item 5", "Item 6"],
            ["Item 7", "Item 8", "Item 9"],
          ],
        },
        {
          title: "Information",
          items: ["Item 10", "Item 11", "Item 12", "Item 13"],
        },
      ],
      socialIcons: [
        "fab fa-facebook",
        "fab fa-twitter",
        "fab fa-instagram",
        "fab fa-linkedin",
      ],
    };
  },
};
</script>

<template>
  <footer class="footer">
    <div class="container pt-5">
      <div class="row">
        <!-- COL 1 -->
        <div class="col-6">
          <h3 class="footer-title">Address</h3>
          <ul class="list-unstyled">
            <li v-for="(item, i) in columns[0].items" :key="i">{{ item }}</li>
          </ul>
          <!-- ICONS -->
          <div class="social-icons">
            <i
              v-for="(icon, i) in socialIcons"
              :key="i"
              :class="icon"
              :style="{ paddingLeft: i === 0 ? '0' : '1rem' }"
            ></i>
          </div>
        </div>

        <!-- COL 2 -->
        <div class="col-3">
          <h3 class="footer-title">Explore</h3>
          <div class="row">
            <div class="col-6">
              <ul class="list-unstyled">
                <li v-for="(item, i) in columns[1].items[0]" :key="i">
                  {{ item }}
                </li>
              </ul>
            </div>
            <div class="col-6">
              <ul class="list-unstyled">
                <li v-for="(item, i) in columns[1].items[1]" :key="i">
                  {{ item }}
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- COL 3 -->
        <div class="col-3">
          <h3 class="footer-title">Information</h3>
          <ul class="list-unstyled">
            <li v-for="(item, i) in columns[2].items" :key="i">{{ item }}</li>
          </ul>
        </div>
      </div>
      <div class="row">
        <div class="col text-center mt-5">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer {
  background-color: rgb(248, 248, 248);
  color: rgb(105, 105, 105);
  padding: 20px 0;

  ul {
    padding: 0;
  }

  ul li {
    margin-bottom: 10px;
    font-size: 0.9rem;
  }

  .footer-title {
    font-size: 1rem;
    font-weight: 700;
    margin-bottom: 10px;
    color: rgb(51, 51, 51);
  }

  .social-icons {
    font-size: 24px;
    color: rgb(177, 177, 177);
    margin-top: 10px;
  }

  //   & i:first-child {
  //     padding-left: 0;
  //     padding-right: 1rem;
  //   }

  p {
    font-size: 0.7rem;
    color: rgb(177, 177, 177);
  }
}
</style>
