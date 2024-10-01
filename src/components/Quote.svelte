<script>
  import kazumaImg from "$lib/assets/kazuma.png"
  import { kazuma } from "$lib/quotes.ts"
  let quote = randomQuote();

  function randomQuote() {
    return kazuma[Math.floor(Math.random()*kazuma.length)];
  }
</script>

<div class="text-box">
  <img alt="kazuma" class="text-box-image" src={kazumaImg}>
  <span class="text">{quote}</span>
</div>

<style>
  .text-box-image {
    width: 100%;
    height: 100%;
  }

  .text-box {
    position: relative;
    text-align: left;
  }

  .text {
    position: absolute;
    top: 75.5%;
    left: 20%;
    margin-right: 20%;
    color: white;
    font-size: 22pt;
    font-family: TGAABody;
    src:url(/fonts/TGAA.otf);
  }
</style>
