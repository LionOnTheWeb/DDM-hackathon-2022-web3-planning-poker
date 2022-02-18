<script>
export let number = 0;
export let img='';
export let name='';
</script>

<div class="card">
   <div><span>{number}</span></div>
   <img src="/images/img{img}.png"/>
   <span class="username">{name}</span>
</div>
<style>
.card {
        flex-wrap: wrap;
        margin: 25px 20px;
        width: 80px;
        display: flex;
       justify-content: center;
    }
    .card div {
      display: flex;
      align-items: center;
       width: 80px;
       height: 80px;
       background: #FFFF66;
       color: black;
       font-size: 24px;
       margin-bottom: 20px;
    }
.card .username {
  color: black;
  font-size: 20px; 
}
    .card  div span {
      text-align: center;
      margin-left: auto;
      margin-right: auto;
      display: block;
      vertical-align: middle;
    }

    img {
      height: 80px;
    }
</style>