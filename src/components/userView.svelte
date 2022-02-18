<script>
    import Card from '../shared/Card.svelte';
    export let userName;
    </script>
    <div className="app">
        <div class="header">
            <div class="header-img"></div>
            <h2>Hello {userName}!</h2>
        </div>
        <p>Ticket 1</p>
        <p>Ticket title</p>
        <div class="card">
            <Card userNumber="1"/>
            <Card userNumber="1"/>
            <Card userNumber="1"/>
            <Card userNumber="1"/>
            <Card userNumber="1"/>
            <Card userNumber="1"/>
            <Card userNumber="1"/>
            <Card userNumber="1"/>
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