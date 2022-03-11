<script>
    import BadgeSecondary from "./BadgeSecondary.svelte"
    import BadgeGhost from "./BadgeGhost.svelte"
    import ButtonPrimary from "./ButtonPrimary.svelte";
</script>

<article>
    <img src="/card_img.jpg" alt="">
    <div class="content">
        <div class="h2AndBadge">
            <h2>Shoes!</h2>
            <BadgeSecondary>New</BadgeSecondary>
        </div>
        <p>If a dog chews shoes whose shoes does he choose?</p>
        <div class="ghostBadges">
            <BadgeGhost>Fashion</BadgeGhost>
            <BadgeGhost>Products</BadgeGhost>
        </div>
        <div class="buttonPrimary">
            <ButtonPrimary>Buy now</ButtonPrimary>
        </div>
    </div>
</article>

<style>
     article {
        margin-bottom: 20px;
        background-color: #ffffff;
        border-radius: 10px;
        width: 400px;
        text-align: left;
    }
    .content {
        padding-left: 20px;
        padding-right: 20px;
        padding-bottom: 20px;
    }
    h2 {
        margin: 0;
        text-align: left;
        margin-top: 13px;
    }
    img {
        height: auto;
        width: 400px;
    }
    .buttonPrimary {
        text-align: right;
    }
    .h2AndBadge {
        display: flex;
        flex-direction: row;
        gap: 20px;
        margin-top: 10px;
    }
    .ghostBadges {
        display: flex;
        flex-direction: row;
        gap: 20px;
    }
</style>