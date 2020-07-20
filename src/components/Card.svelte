<script>
  import Comments from './Comments.svelte';
</script>

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
        <i class="fas fa-papper-plane" />
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