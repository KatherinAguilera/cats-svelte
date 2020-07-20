<script>
  import Comments from './Comments.svelte';
</script>

<style>
  .Card {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 4px;
    background-color: white;
    margin: 0 0 2em 0;
  }
  .Card-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1em;
  }
  .Card-user {
    display: flex;
    align-items: center;
    justify-content: flex-end;
  }
  .Card-user img {
    width: 32px;
    height: 32px;
    border-radius: 50%;
  }
  .Card-user h2 {
    margin: 0;
    padding: 0;
    font-size: 14px;
    font-weight: 600;
    margin: 0 0 0 1em;
    color: black;
  }
  .Card-user h2 span {
    display: block;
    font-size: 12px;
    font-weight: normal;
    color: rgba(38, 38, 38, 0.7);
  }
  .Card-photo {
    padding: 0;
    margin: 0;
  }
  .Card-photo img {
    width: 100%;
    height: auto;
  }
  .Card-photo figure {
    margin: 0;
    padding: 0;
    cursor: pointer;
  }
  .Card-settings i {
    cursor: pointer;
  }
  .Card-icons {
    padding: 1em;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .Card-icons i {
    margin: 0 1em 0 0;
    cursor: pointer;
    font-size: 20px;
  }
  .Card-icons i:last-child {
    margin: 0;
  }
  .Card-description {
    padding: 0 1em 1em 1em;
  }
  .Card-description h3 {
    font-size: 14px;
    font-weight: bold;
    color: black;
  }
  .Card-description span {
    font-size: 14px;
  }
  .active-like {
    color: #bc1888;
    animation: bounce linear 0.8s;
    animation-iteration-count: 1;
    transform-origin: 20% 20%;
  }
  .active-bookmark {
    color: #f09433;
  }

  @keyframes bounce {
    0% {
      transform: translate(0px, 0px);
    }
    15% {
      transform: translate(0px, -25px);
    }
    30% {
      transform: translate(0px, 0px);
    }
    45% {
      transform: translate(0px, -15px);
    }
    60% {
      transform: translate(0px, 0px);
    }
    75% {
      transform: translate(0px, -5px);
    }
    100% {
      transform: translate(0px, 0px);
    }
  }
</style>

<div class="Card">
  <div class="Card-container">
    <div class="Card-header">
      <div class="Card-user">
        <img src="https://lh3.googleusercontent.com/iHIi9ImZEyl0RhO39d1kH0pGPQTUyQtGuoecfKAkdzaFZ1XJS4yYqLsWmp0kzhq-hzwpW0OGLbJdNVU8GYHG21daGx6GUknuXVPdr-iO6KQDBsXnSjy6RSXayskvfuVEMOzzxhrTn-ia0rgaOLHTfYAscGgyV3rrrl_24l8vk9lMWKCxdw1VF467q4ytVF_5nUvLLzlXL-fIqHFjmDaPLKLuV-2gPcqJcZ81-0BppaBB9Xh6aSTewtMk7u_5v3-VPZqYn5njvHa6mKy_0lHr5KdTeQDvURw3IYOUnzRmVDPDqjP_zgcX72tefQ7Z3aqiLE4IIr11hT-TbfdrwXBXF5yduzSA5C598sBx5Ofyt5uQR4LqeO-voP-J33YIUAZLOoWxqJTsAgl1_RSYt0t8_hAmwJ7nN64Cd5aZt4LdCkKdMT4HATZFKikNg6bj33HxvbuZ7g-9k3jKi8VpseFUvEGpY31RCCthqJvIVo16gB7jodKLqU0QyVaqVQkEN1CV9-PkMKa2JagVAZq6cWOJSxbhXPg7_orLe2EvNl72S-WzSGwN8Gho55vK0j7SRUe-QrCFmuf3o_ZUAzebPviRFhScABotZKoaT-1ks8Vby3oyTax7O-7QFynXOu2kobXbAwFi9x1QRg8mJ9NLWzQsn1PC8rx4ehDOO6FwHvDcK9egZWpK5epA7pefYn0Xtw=w601-h801-no?authuser=1" alt="">
        <h2>Haru
          <span>Tocancipá, Colombia</span>
        </h2>
      </div>
      <div class="Card-settings">
        <i class="fas fa-ellipsis-h" />
      </div>
    </div>
    <div class="Card-photo">
      <figure>
        <img src="https://lh3.googleusercontent.com/iHIi9ImZEyl0RhO39d1kH0pGPQTUyQtGuoecfKAkdzaFZ1XJS4yYqLsWmp0kzhq-hzwpW0OGLbJdNVU8GYHG21daGx6GUknuXVPdr-iO6KQDBsXnSjy6RSXayskvfuVEMOzzxhrTn-ia0rgaOLHTfYAscGgyV3rrrl_24l8vk9lMWKCxdw1VF467q4ytVF_5nUvLLzlXL-fIqHFjmDaPLKLuV-2gPcqJcZ81-0BppaBB9Xh6aSTewtMk7u_5v3-VPZqYn5njvHa6mKy_0lHr5KdTeQDvURw3IYOUnzRmVDPDqjP_zgcX72tefQ7Z3aqiLE4IIr11hT-TbfdrwXBXF5yduzSA5C598sBx5Ofyt5uQR4LqeO-voP-J33YIUAZLOoWxqJTsAgl1_RSYt0t8_hAmwJ7nN64Cd5aZt4LdCkKdMT4HATZFKikNg6bj33HxvbuZ7g-9k3jKi8VpseFUvEGpY31RCCthqJvIVo16gB7jodKLqU0QyVaqVQkEN1CV9-PkMKa2JagVAZq6cWOJSxbhXPg7_orLe2EvNl72S-WzSGwN8Gho55vK0j7SRUe-QrCFmuf3o_ZUAzebPviRFhScABotZKoaT-1ks8Vby3oyTax7O-7QFynXOu2kobXbAwFi9x1QRg8mJ9NLWzQsn1PC8rx4ehDOO6FwHvDcK9egZWpK5epA7pefYn0Xtw=w601-h801-no?authuser=1" alt="">
      </figure>
    </div>
    <div class="Card-icons">
      <div class="Card-icons-first">
        <i class="fas fa-heart" />
        <i class="fas fa-paper-plane" />
      </div>
      <div class="Card-icons-second">
        <i class="fas fa-bookmark" />
      </div>
    </div>

    <div class="Card-description">
      <h3>Haru.cat</h3>
      <span>Hola!</span>
    </div>

    <Comments />
  </div>
</div>