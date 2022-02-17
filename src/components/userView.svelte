<script>
    import Card from '../shared/Card.svelte';
    export let userName;
    </script>
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
    </div>
  
  <style lang="scss">
      h2 {
          color: $primary-blue;
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
        margin-right: 100px;
      }
      .card {
          display: flex;
          justify-content: space-between;
      }
  </style>