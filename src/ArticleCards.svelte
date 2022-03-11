<script>
    	import Card from "./Card.svelte"
</script>

<article>
    <h2>Article with cards</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil inventore repellat saepe aperiam nulla quasi quia ut velit minus dignissimos ullam, nesciunt odio nemo quibusdam eius dolorem illum deleniti iure?</p>
        <div>
			<Card />
			<Card />
		</div>
        
    <pre>
        <code>
            &lt;script&gt;
                import Card from "./Card.svelte"
            &lt;/script&gt;
            <br>
            &lt;div&gt;
                &lt;Card /&gt;
                &lt;Card /&gt;
            &lt;/div&gt;
        </code>
    </pre>
</article>

<style>
     article {
        border: 2px solid #3E4450;
        margin-bottom: 50px;
        border-radius: 10px;
        padding: 25px;
    }
    h2 {
        margin: 0;
        margin-top: 25px;
        margin-bottom: 50px;
    }
    p {
        margin: 0;
        margin-bottom: 40px;
    }
    @media only screen and (min-width: 800px) {
        article {
            padding-left: 100px;
            padding-right: 100px;
        }
    }
    div {
        display: grid;
        grid-template-columns: repeat( auto-fit, minmax(150px, 1fr) );
        gap: 50px;
    }
</style>