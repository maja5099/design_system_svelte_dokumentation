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
        background-color: #3e445000;
        color: #4D2AEE;
    }
    button:hover {
        color: #4D2AEEda;
    }
</style>