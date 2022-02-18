<script>
  import Usercard from '../components/Usercard.svelte';
  export let userName;
  let numbers = [0,3,5,2,3,5];
  let iterates = [1,2,3,4,5,6];
  let names = ["Brian","Asad", "Safie", "Gouled","John","Vik"];
  </script>
      <div class="header">
          <h2>Hello Asad!</h2>
      </div>
      <p class="ticketname">Ticket N1: Defect | Image Cropping for HP Daily News Block is not correct</p>
      <div class="facilitator">
      {#each iterates as i}
          <Usercard img="{iterates[--i]}" number={numbers[i]} name={names[i]}/>
      {/each}
      </div>
 <style lang="scss">
 .facilitator {
     display: flex;
     justify-content: space-between;
 }
    h2 {
        text-transform: uppercase;
        font-size: 24px;
        text-align: left;
        font-weight: 100;
    }
    p {
        font-size: 22px;
        text-align: left;
        padding-left: 20px;
    }
    .header {
        display: flex;
        justify-content: left;
        height: 80px;
        font-size: 24px;
        margin-top: 0px;
        padding-left: 20px;
        font-weight: bold;
    }
    .card {
        display: flex;
        justify-content: space-between;
        flex-wrap: wrap;
        margin: 25px 50px;
    }
</style>