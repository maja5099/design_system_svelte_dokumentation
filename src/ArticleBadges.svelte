<script>
    import BadgeNeutral from "./BadgeNeutral.svelte";
    import BadgePrimary from "./BadgePrimary.svelte";
    import BadgeSecondary from "./BadgeSecondary.svelte";
    import BadgeAccent from "./BadgeAccent.svelte";
    import BadgeGhost from "./BadgeGhost.svelte";
</script>

<article>
    <h2>Article with badges</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil inventore repellat saepe aperiam nulla quasi quia ut velit minus dignissimos ullam, nesciunt odio nemo quibusdam eius dolorem illum deleniti iure?</p>
    <div>
        <BadgeNeutral> Neutral </BadgeNeutral>
        <BadgePrimary> Primary </BadgePrimary>
        <BadgeSecondary> Secondary </BadgeSecondary>
        <BadgeAccent> Accent </BadgeAccent>
        <BadgeGhost> Ghost </BadgeGhost>
    </div>
    <pre>
        <code>
            CODE IN APP.SVELTE:
            &lt;script&gt;
                import ArticleBadges from "./ArticleBadges.svelte";
            &lt;/script&gt;
            <br>
            &lt;main&gt;
                &lt;ArticleBadges /&gt;
            &lt;/main&gt;
            <br>
            CODE IN ARTICLEBADGES.SVELTE:
            &lt;script&gt;
                import BadgeNeutral from "./BadgeNeutral.svelte";
                import BadgePrimary from "./BadgePrimary.svelte";
                import BadgeSecondary from "./BadgeSecondary.svelte";
                import BadgeAccent from "./BadgeAccent.svelte";
                import BadgeGhost from "./BadgeGhost.svelte";
            &lt;/script&gt;
    
            &lt;div&gt;
                &lt;BadgeNeutral&gt; Neutral &lt;/BadgeNeutral&gt;
                &lt;BadgePrimary&gt; Primary &lt;/BadgePrimary&gt;
                &lt;BadgeSecondary&gt; Secondary &lt;/BadgeSecondary&gt;
                &lt;BadgeAccent&gt; Accent &lt;/BadgeAccent&gt;
                &lt;BadgeGhost&gt; Ghost &lt;/BadgeGhost&gt;
            &lt;/div&gt;
            <br>
            CODE IN INDIVIDUAL BADGE.SVELTE
            &lt;div&gt;
                &lt;p&gt;
                    &lt;slot /&gt;
                &lt;/p&gt;
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
        margin-bottom: 25px;
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