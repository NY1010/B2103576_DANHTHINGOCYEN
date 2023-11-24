<template>
  <footer class="page-footer orange">
    <div class="container">
      <div class="row">
        <div class="col l6 s12">
          <h5 class="white-text">Company Bio</h5>
          <p class="grey-text text-lighten-4">
            This is a silver bracelet store that brings out the delicate beauty
            of each customer when they come to buy. And we are increasingly
            developing to bring the best choice to express symbols of love,
            trust and luck to customers.
          </p>
        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Address</h5>
          <ul>
            <li>
              <a class="white-text" href="#!"
                >Xuan Khanh - Ninh Kieu - Can Tho</a
              >
            </li>
            <li>
              <a Nga class="white-text" href="#!">Nga Nam - Soc Trang </a>
            </li>
            <li>
              <a class="white-text" href="#!">Mang Thit-Vinh Long</a>
            </li>
            <li>
              <a class="white-text" href="#!">Thoi Binh - Ca Mau</a>
            </li>
          </ul>
        </div>
        <div class="col l3 s12">
          <h5 class="white-text">Connect</h5>
          <ul>
            <li><a class="white-text" href="#!">Facebook</a></li>
            <li><a class="white-text" href="#!">Zalo</a></li>
            <li><a class="white-text" href="#!">Instagram</a></li>
            <li><a class="white-text" href="#!">Tiktok</a></li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-copyright">
      <div class="container">
        Made by
        <a class="orange-text text-lighten-3" href="#">Dtny</a>
      </div>
    </div>
  </footer>
</template>

<script>
import axios from 'axios';
import swal from 'sweetalert2';
import store from '../../vuex/store';

export default {
  name: 'AppFooter',

  data() {
    return {
      page: 0,
    };
  },

  computed: {
    user: function () {
      return store.getters.getUser;
    },

    login: function () {
      return store.getters.getLogin;
    },
  },
};
</script>
