<script>
  import Card from '../components/Card.svelte';

  export let userName = "";

  let numbers = [0,1,2,3,5,8,13,21];
</script>

  <div class="header">
      <h2>Hello {userName}!</h2>
  </div>
  
  <p>{userName || "Player name"}</p>
  <p>Acive Ticket title</p>
  
  <div class="card">
  {#each numbers as number}
      <Card userNumber={number}/>
  {/each}
  </div>

<style lang="scss">
    h2 {
        text-transform: uppercase;
        font-size: 4em;
        font-weight: 100;
    }
    p {
        font-size: 2em;
        padding-left: 65px;
    }
    .header {
        display: flex;
        justify-content: space-around;
        height: 80px;
        margin-top: -25px;
    }
    .card {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        margin: 25px 50px;
    }
</style>