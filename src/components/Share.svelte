  
<style>
  .Share {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 4px;
    background-color: white;
    margin: 0 0 2em 0;
    width: 300px;
    height: 80px;
    position: absolute;
    top: 300px;
    left: 30%;
    z-index: 9;
    padding: 1em;
  }
  .share-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .share-head h2 {
    font-size: 16px;
  }
  .share-head i {
    cursor: pointer;
  }
  .share-content a {
    display: flex;
    align-items: center;
    text-decoration: none;
    color: black;
    font-size: 14px;
    margin: 2em 0 0 0;
  }
  .share-content i {
    color: #3b5998;
    margin: 0 0.5em 0 0;
    font-size: 20px;
  }
</style>

<div class="Share">
  <div class="share-head">
    <h2>Compartir</h2>
    <i class="fas fa-times-circle" on:click />
  </div>
  <div class="share-content">
    <a
      target="_blank"
      href="https://www.facebook.com/sharer/sharer.php?&u=https://pugstagram.co">
      <i class="fab fa-facebook-square" />
      Compartir en Facebook
    </a>
  </div>
</div>

<!-- Share.svelte -->