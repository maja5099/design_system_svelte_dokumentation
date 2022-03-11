<script>
	// IF ELSE FUNCTION (COOKIES)
    let acceptedCookies = false;
	function accept(){
		acceptedCookies = true;
	}
</script>

<!-- IF ELSE FUNCTION (COOKIES) -->
{#if acceptedCookies === false}
	<div>
		<p>
			This site uses cookies.
		</p>
		<button on:click={accept}>
			Accept
		</button>
	</div>
{/if}

<style>
	* {
		box-sizing:border-box;
	}
	div {
		position:fixed;
		bottom:0;
		left:0;
		width:100vw;
		background: #4e5565;
		display:flex;
		justify-content: space-between;
		padding:2rem;
	}
    button {
        margin-right: 20px;
        margin-bottom: 0;
		font-weight: 600;
        text-transform: uppercase;
	    border-radius: 10px;
	    padding-left: 15px;
        padding-right: 15px;
		color: #4e5565;
    }
	p {
		color: #e7e7e7;
		font-weight: 450;
	}
</style>