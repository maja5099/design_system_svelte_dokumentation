<script>
    // STATE FUNCTION (NAV BAR)
	let open = false;
  	function toggle() {
    open = !open;
  	}
</script>

<!-- STATE FUNCTION (NAV BAR) -->
<div>
    <nav class="topNav">
        <button class="ham" on:click={toggle}><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="iconify iconify--quill" width="32" height="32" preserveAspectRatio="xMidYMid meet" viewBox="0 0 32 32"><path fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 8h22M5 16h22M5 24h22"></path></svg></button>
    </nav>
    <nav class="sideNav" class:showNav={open}>
        <button class="menuX" on:click={toggle}><svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" aria-hidden="true" role="img" class="iconify iconify--radix-icons" width="32" height="32" preserveAspectRatio="xMidYMid meet" viewBox="0 0 15 15"><path fill="currentColor" fill-rule="evenodd" d="M11.782 4.032a.575.575 0 1 0-.813-.814L7.5 6.687L4.032 3.218a.575.575 0 0 0-.814.814L6.687 7.5l-3.469 3.468a.575.575 0 0 0 .814.814L7.5 8.313l3.469 3.469a.575.575 0 0 0 .813-.814L8.313 7.5l3.469-3.468Z" clip-rule="evenodd"></path></svg></button>
        <ul>
          <li><a class="menuLink" href="#home">Home</a></li>
          <li><a class="menuLink" href="#profile">Profile</a></li>
          <li><a class="menuLink" href="#about">About</a></li>
          <li><a class="menuLink" href="#contacts">Contacts</a></li>
        </ul>
    </nav>
</div>

<style>
	.topNav {
	  position: fixed;
	  top: 0;
	  left: 0;
	  right: 0;
	  width: 100%;
	  height: 4rem;
	  display: flex;
	  align-items: center;
	  background-color: #3E4450;
	}
	.ham {
	  position: relative;
	  width: 2rem;
	  height: 2rem;
	  margin-left: 0.5rem;
	  background: none;
	  border: none;
	  cursor: pointer;
	  color: #D3D4D6;
	}
	.menuX {
	  position: absolute;
	  top: 4.5rem;
	  right: 2rem;
	  width: 2rem;
	  height: 2rem;
	  margin-left: 0.5rem;
	  background: none;
	  border: none;
	  cursor: pointer;
	  color: #D3D4D6;
	}
	.sideNav {
	  position: fixed;
	  top: 0;
	  left: 0;
	  bottom: 0;
	  z-index: 101;
	  background: #4e5565;
	  width: 300px;
	  height: 100vh;
	  overflow: hidden;
	  color: #D3D4D6;
	  /* hide the menu above the screen by default */
	  transform: translateX(-100%);
	  transition: transform 0.5s ease;
	}
	.showNav {
	  transform: translateX(0);
	}
	.sideNav ul {
	  width: 100%;
	  height: 100%;
	  list-style: none;
	  display: flex;
	  flex-flow: column nowrap;
	  align-items: center;
	  padding-top: 8rem;
	}
	.sideNav ul li a {
	  display: block;
	  color: #D3D4D6;
	  padding-bottom: 5px;
	  margin-top: 3rem;
	  border-bottom: 1.5px solid #4e5565;
	  text-decoration: none;
	  font-family: "Open Sans", sans-serif;
	  font-size: 1.2rem;
	}
	.sideNav ul li a:hover,
	.sideNav ul li a:focus {
	  border-bottom: 1.5px solid #D3D4D6;
	}
</style>