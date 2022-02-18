<script>
  export let userNumber;
let val='';
let timer;
const debounce = v => {
  clearTimeout(timer);
  timer = setTimeout(() => {
    val = v;
  }, 350);
}
</script>

<div class="card">
  <div class="container">
      {userNumber}
  </div>
</div>


<style lang="scss">
  .card{
      background: #fff;
      padding: 13px 25px;
      border-radius: 25px;
      box-shadow: 0px 4px 8px 0 rgba(0,0,0,0.2);
      width: 200px;
      height: 150px;
      margin: 25px 10px;
  }
  .card:hover {
      box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
  }
  .container {
      font-size: 60px;
      text-align: center;
      line-height: 2.5;
  }
</style>