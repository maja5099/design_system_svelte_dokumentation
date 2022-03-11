<script>
    import ButtonNeutral from "./ButtonNeutral.svelte";
    import ButtonPrimary from "./ButtonPrimary.svelte";
    import ButtonSecondary from "./ButtonSecondary.svelte";
    import ButtonAccent from "./ButtonAccent.svelte";
    import ButtonGhost from "./ButtonGhost.svelte";
    import ButtonLink from "./ButtonLink.svelte";
</script>

<article>
    <h2>Article with buttons</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil inventore repellat saepe aperiam nulla quasi quia ut velit minus dignissimos ullam, nesciunt odio nemo quibusdam eius dolorem illum deleniti iure?</p>
    <div>
        <ButtonNeutral> Neutral </ButtonNeutral>
        <ButtonPrimary> Primary </ButtonPrimary>
        <ButtonSecondary> Secondary </ButtonSecondary>
        <ButtonAccent> Accent </ButtonAccent>
        <ButtonGhost> Ghost </ButtonGhost>
        <ButtonLink> Link </ButtonLink>
    </div>
    <pre>
        <code>
            CODE IN APP.SVELTE:
            &lt;script&gt;
                import ArticleButtons from "./ArticleButtons.svelte";
            &lt;/script&gt;

            &lt;main&gt;
                &lt;ArticleButtons /&gt;
            &lt;/main&gt;
            <br>
            CODE IN ARTICLEBUTTONS.SVELTE:
            &lt;script&gt;
                import ButtonNeutral from "./ButtonNeutral.svelte";
                import ButtonPrimary from "./ButtonPrimary.svelte";
                import ButtonSecondary from "./ButtonSecondary.svelte";
                import ButtonAccent from "./ButtonAccent.svelte";
                import ButtonGhost from "./ButtonGhost.svelte";
                import ButtonLink from "./ButtonLink.svelte";
            &lt;/script&gt;
        
            &lt;div&gt;
                &lt;ButtonNeutral&gt; Neutral &lt;/ButtonNeutral&gt;
                &lt;ButtonPrimary&gt; Primary &lt;/ButtonPrimary&gt;
                &lt;ButtonSecondary&gt; Secondary &lt;/ButtonSecondary&gt;
                &lt;ButtonAccent&gt; Accent &lt;/ButtonAccent&gt;
                &lt;ButtonGhost&gt; Ghost &lt;/ButtonGhost&gt;
                &lt;ButtonLink&gt; Link &lt;/ButtonLink&gt;
            &lt;/div&gt;
            <br>
            CODE IN INDIVIDUAL BUTTON.SVELTE
            &lt;div&gt;
                &lt;button&gt;
                    &lt;slot /&gt;
                &lt;/button&gt;
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
    }
</style>