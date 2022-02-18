<script>
    import Card from '../shared/Card.svelte';
    export let userName;

    let numbers = [0,1,2,3,5,8,13,21];
    </script>
    <div className="app">

        <div class="header">
            <div class="header-img"></div>
            <h2>Hello {userName}!</h2>
        </div>
        <p>Player name</p>
        <p>Acive Ticket title</p>
        <div class="card">
        {#each numbers as number}
            <Card userNumber={number}/>
        {/each}
        </div>
    </div> 
 
  <style lang="scss">
      .app {
          padding: 25px 80px 50px 50px;
      }
      h2 {
          text-transform: uppercase;
          font-size: 4em;
          font-weight: 100;
      }
      p {
          font-size: 2em;
      }
      .header {
          display: flex;
      }
      .header-img {
        width: 200px;
        height: 200px;
        background: url('https://image.shutterstock.com/image-photo/red-apple-isolated-on-white-260nw-1727544364.jpg');
        background-size: cover;
        margin-right: 200px;
      }
      .card {
          display: flex;
          justify-content: space-between;
          flex-wrap: wrap;
          margin: 25px 50px;
      }
  </style>