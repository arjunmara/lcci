<template>
    <div class="my-nav">
        <!-- HEADER -->
		<div class="header-wrap">
			<header>
				<!-- LOGO -->
				<router-link to="/home">
					<figure class="logo">
						<img src="../assets/images/logo.png" alt="logo">
					</figure>
				</router-link>
				<!-- /LOGO -->

				<!-- MOBILE MENU HANDLER -->
				<div class="mobile-menu-handler left primary"
				@click="dropDown">
					<img src="../assets/images/pull-icon.png" alt="pull-icon">
				</div>
				<!-- /MOBILE MENU HANDLER -->

				<!-- LOGO MOBILE -->
				<router-link to='home'>
					<figure class="logo-mobile">
						<img src="../assets/images/logo.png" alt="logo-mobile">
					</figure>
				</router-link>
				<!-- /LOGO MOBILE -->

				<!-- MOBILE ACCOUNT OPTIONS HANDLER -->
				<div class="mobile-account-options-handler right secondary">
					<span class="icon-user"></span>
				</div>
				<!-- /MOBILE ACCOUNT OPTIONS HANDLER -->

				<!-- USER BOARD -->
				<div class="user-board">
					<!-- USER QUICKVIEW -->
					<div class="user-quickview">
						<!-- USER AVATAR -->
						<a href="author-profile.html">
						<div class="outer-ring">
							<div class="inner-ring"></div>
							<figure class="user-avatar">
								<img src="../assets/images/avatars/avatar_01.jpg" alt="avatar">
							</figure>
						</div>
						</a>
						<!-- /USER AVATAR -->

						<!-- USER INFORMATION -->
						<p class="user-name"
						@click="dropDown">Arjun</p>
						<!-- SVG ARROW -->
						<svg class="svg-arrow">
							<use xlink:href="#svg-arrow"></use>
						</svg>
						<!-- /SVG ARROW -->
						<p class="user-money">Member</p>
						<!-- /USER INFORMATION -->

						<!-- DROPDOWN -->
						<ul class="dropdown small hover-effect" v-if="opened">
							<li class="dropdown-item">
								<div class="dropdown-triangle"></div>
								<router-link to="/profile">Profile Page</router-link>
							</li>
							<li class="dropdown-item">
								<router-link to="/dashboard"> Settings</router-link>
							</li>
							<li class="dropdown-item">
								<a href="logout.php">Logout</a>
							</li>
						</ul>
						<!-- /DROPDOWN -->
					</div>
					<!-- /USER QUICKVIEW -->
				</div>
				<!-- /USER BOARD -->
			</header>
		</div>
		<!-- /HEADER -->

		<!-- SIDE MENU -->
		<div id="mobile-menu" class="side-menu left" v-if="opened">
			<!-- SVG PLUS -->
			<svg class="svg-plus">
				<use xlink:href="#svg-plus"></use>
			</svg>
			<!-- /SVG PLUS -->

			<!-- SIDE MENU HEADER -->
			<div class="side-menu-header">
				<figure class="logo small">
					<img src="../assets/images/logo.png" alt="logo">
				</figure>
			</div>
			<!-- /SIDE MENU HEADER -->

			<!-- SIDE MENU TITLE -->
			<p class="side-menu-title">Main Links</p>
			<!-- /SIDE MENU TITLE -->

			<!-- DROPDOWN -->
			<ul class="dropdown dark hover-effect interactive">
				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<router-link to="/">Home</router-link> 
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<router-link to="/about">About us</router-link>
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<router-link to="/news">News</router-link>
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<router-link to ="/gallery">Gallery</router-link>
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<router-link to="/team">Members</router-link>
				</li>
				<!-- /DROPDOWN ITEM -->
			</ul>
			<!-- /DROPDOWN -->
		</div>
		<!-- /SIDE MENU -->

		<!-- SIDE MENU -->
		<div id="account-options-menu" class="side-menu right closed">
			<!-- SVG PLUS -->
			<svg class="svg-plus">
				<use xlink:href="#svg-plus"></use>
			</svg>
			<!-- /SVG PLUS -->

			<!-- SIDE MENU HEADER -->
			<div class="side-menu-header">
				<!-- USER QUICKVIEW -->
				<div class="user-quickview">
					<!-- USER AVATAR -->
					<a href="author-profile.html">
					<div class="outer-ring">
						<div class="inner-ring"></div>
						<figure class="user-avatar">
							<img src="../assets/images/avatars/avatar_01.jpg" alt="avatar">
						</figure>
					</div>
					</a>
					<!-- /USER AVATAR -->

					<!-- USER INFORMATION -->
					<p class="user-name" @click="dropDown">Arjun Marasini</p>
					<p class="user-money">Member</p>
					<!-- /USER INFORMATION -->
				</div>
				<!-- /USER QUICKVIEW -->
			</div>
			<!-- /SIDE MENU HEADER -->

			<!-- SIDE MENU TITLE -->
			<p class="side-menu-title">Your Account</p>
			<!-- /SIDE MENU TITLE -->

			<!-- DROPDOWN -->
			<ul class="dropdown dark hover-effect" v-if="opened">
				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<a href="#">Notifications</a>
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<a href="#">Messages</a>
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<a href="#">Your Cart</a>
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<a href="#">Favourites</a>
				</li>
				<!-- /DROPDOWN ITEM -->
			</ul>
			<!-- /DROPDOWN -->

			<!-- SIDE MENU TITLE -->
			<p class="side-menu-title">Dashboard</p>
			<!-- /SIDE MENU TITLE -->

			<!-- DROPDOWN -->
			<ul class="dropdown dark hover-effect">
				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<a href="#">Profile Page</a>
				</li>
				<!-- /DROPDOWN ITEM -->

				<!-- DROPDOWN ITEM -->
				<li class="dropdown-item">
					<a href="#">Account Settings</a>
				</li>
				<!-- /DROPDOWN ITEM -->

				
			</ul>
			<!-- /DROPDOWN -->
		</div>
		<!-- /SIDE MENU -->

		<!-- MAIN MENU -->
		<div class="main-menu-wrap">
			<div class="menu-bar">
				<nav>
					<ul class="main-menu">
						<!-- MENU ITEM -->
						<li class="menu-item">
							<router-link to="/">Home</router-link>
						</li>
						<!-- /MENU ITEM -->

						<!-- MENU ITEM -->
						<li class="menu-item">
							<router-link to ="/about">About Us</router-link>
						</li>
						<!-- /MENU ITEM -->

						<!-- MENU ITEM -->
						<li class="menu-item">
							<router-link to="/news">News</router-link>
						</li>
						<!-- /MENU ITEM -->

						<!-- MENU ITEM -->
						<li class="menu-item">
							<router-link to ="/gallery">Gallery</router-link>
						</li>
						<!-- /MENU ITEM -->

						<!-- MENU ITEM -->
						<li class="menu-item">
							<router-link to="/team">Members</router-link>
						</li>
						<!-- /MENU ITEM -->
					</ul>
				</nav>
				<form class="search-form">
					<input type="text" class="rounded" name="search" id="search_news" placeholder="Search here...">
					<input type="image" src="../assets/images/search.png" alt="search-icon">
				</form>
			</div>
		</div>
		<!-- /MAIN MENU -->
    </div>
</template>
<script>
export default {
  name: "mynavbar",
  data: function() {
    return {
      opened: false
    };
  },
  methods: {
    dropDown: function() {
      return (this.opened = !this.opened);
    }
  }
};
</script>
<style>
</style>

