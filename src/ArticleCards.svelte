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
            CODE IN APP.SVELTE:
            &lt;script&gt;
                import ArticleCards from "./ArticleCards.svelte";
            &lt;/script&gt;

            &lt;main&gt;
                &lt;ArticleCards /&gt;
            &lt;/main&gt;
            <br>
            CODE IN ARTICLECARDS.SVELTE:
            &lt;script&gt;
                import Card from "./Card.svelte"
            &lt;/script&gt;
            
            &lt;div&gt;
                &lt;Card /&gt;
                &lt;Card /&gt;
            &lt;/div&gt;
            <br>
            CODE IN CARD.SVELTE:
            &lt;script&gt;
                import BadgeSecondary from "./BadgeSecondary.svelte";
                import BadgeGhost from "./BadgeGhost.svelte";
                import ButtonPrimary from "./ButtonPrimary.svelte";
            &lt;/script&gt;

            &lt;article&gt;
                &lt;img src="/card_img.jpg" alt=""&gt;
                &lt;div class="content"&gt;
                    &lt;div class="h2AndBadge"&gt;
                        &lt;h2&gt;Shoes!&lt;/h2&gt;
                        &lt;BadgeSecondary&gt;New&lt;/BadgeSecondary&gt;
                        &lt;/div>
                    &lt;p&gt;If a dog chews shoes whose shoes does he choose?&lt;/p&gt;
                    &lt;div class="ghostBadges"&gt;
                        &lt;BadgeGhost&gt;Fashion&lt;/BadgeGhost&gt;
                        &lt;BadgeGhost&gt;Products&lt;/BadgeGhost&gt;
                    &lt;/div&gt;
                    &lt;div class="buttonPrimary"&gt;
                        &lt;ButtonPrimary>Buy now&lt;/ButtonPrimary&gt;
                    &lt;/div&gt;
                &lt;/div&gt;
            &lt;/article&gt;

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