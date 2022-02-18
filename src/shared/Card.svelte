
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
        <input on:keyup={({ target: { value } }) => debounce(value)} />
        <h1> {val}</h1>


    </div>
</div>

  
  <style lang="scss">
    .card{
        background: #fff;
        padding: 20px 25px;
        border-radius: 5px;
        box-shadow: 0px 4px 8px 0 rgba(0,0,0,0.2);
        width: 250px;
        height: 300px;
        margin: 25px 10px;
    }
    h1 {
        font-size: 70px;
        text-align: center;
    }
  </style>