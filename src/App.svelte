<script>
	export let year;
	import Header from "./Header.svelte"
	import ArticleBadges from "./ArticleBadges.svelte"
	import ArticleButtons from "./ArticleButtons.svelte"
	import ArticleCards from "./ArticleCards.svelte"
	import Cookies from "./Cookies.svelte"
	import Footer from "./Footer.svelte"
</script>

<body>
	<main>	
		<!-- H1 -->
		<h1>Design System with Svelte</h1>

		<!-- SVELTE COMPONENTS -->
		<Header />
		<ArticleBadges />
		<ArticleButtons />
		<ArticleCards />

		<Cookies />
		<Footer />
	</main>
</body>

  <style>
	  h1 {
		margin-top: 100px;
		margin-bottom: 50px;
	  }
  </style>