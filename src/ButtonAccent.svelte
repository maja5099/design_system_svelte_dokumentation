<div>
      <button>
        <slot />
    </button>
</div>

<style>
    button {
        font-weight: 600;
        text-transform: uppercase;
	    border-radius: 10px;
	    padding-left: 20px;
        padding-right: 20px;
        padding-top: 15px;
        padding-bottom: 15px;
	    outline: none;
        width: fit-content;
        border: none;
        background-color: #67CABE;
        color: #fff;
    }
    button:hover {
        background-color: #67CABEda;
    }
</style>