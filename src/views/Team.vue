<template>
    <div class="my-team">
		<myNavbar></myNavbar>
			<!-- SECTION HEADLINE -->
		<div class="section-headline-wrap">
			<div class="section-headline">
				<h2>Our Members</h2>
				<p>Home<span class="separator">/</span>Members<span class="separator">/</span><span class="current-section">Team</span></p>
			</div>
		</div>
		<!-- /SECTION HEADLINE -->

		<!-- SECTION -->
		<div class="section-wrap">
			<div class="section">
				<!-- PRODUCT SHOWCASE -->
				<div class="product-showcase">
					<!-- PRODUCT LIST -->
					<div class="product-list grid column4-wrap">
						<!-- PRODUCT ITEM -->
						<div class="product-item column">
							<!-- PRODUCT PREVIEW ACTIONS -->
							<div class="product-preview-actions">
								<!-- PRODUCT PREVIEW IMAGE -->
								<figure class="product-preview-image">
									<img src="../assets/images/items/westeros_m.jpg" alt="product-image">
								</figure>
								<!-- /PRODUCT PREVIEW IMAGE -->
							</div>
							<!-- /PRODUCT PREVIEW ACTIONS -->

							<!-- PRODUCT INFO -->
							<div class="product-info">
								<router-link to="/team-single">
									<p class="text-header">Arjun Designs</p>
								</router-link>
								<p class="product-description">Lorem ipsum dolor sit urarde...</p>
							</div>
							<!-- /PRODUCT INFO -->
							<hr class="line-separator">

							<!-- USER RATING -->
							<div class="user-rating">
								<a href="author-profile.html">
									<figure class="user-avatar small">
										<img src="../assets/images/avatars/avatar_01.jpg" alt="user-avatar">
									</figure>
								</a>
								<a href="author-profile.html">
									<p class="text-header tiny">Arjun Marasini</p>
								</a>
							</div>
							<!-- /USER RATING -->
						</div>
						<!-- /PRODUCT ITEM -->
						<!-- PRODUCT ITEM -->
						<div class="product-item column">
							<!-- PRODUCT PREVIEW ACTIONS -->
							<div class="product-preview-actions">
								<!-- PRODUCT PREVIEW IMAGE -->
								<figure class="product-preview-image">
									<img src="../assets/images/items/westeros_m.jpg" alt="product-image">
								</figure>
								<!-- /PRODUCT PREVIEW IMAGE -->
							</div>
							<!-- /PRODUCT PREVIEW ACTIONS -->

							<!-- PRODUCT INFO -->
							<div class="product-info">
								<router-link to="/team-single">
									<p class="text-header">Arjun Designs</p>
								</router-link>
								<p class="product-description">Lorem ipsum dolor sit urarde...</p>
							</div>
							<!-- /PRODUCT INFO -->
							<hr class="line-separator">

							<!-- USER RATING -->
							<div class="user-rating">
								<a href="author-profile.html">
									<figure class="user-avatar small">
										<img src="../assets/images/avatars/avatar_01.jpg" alt="user-avatar">
									</figure>
								</a>
								<a href="author-profile.html">
									<p class="text-header tiny">Arjun Marasini</p>
								</a>
							</div>
							<!-- /USER RATING -->
						</div>
						<!-- /PRODUCT ITEM -->
					</div>
					<!-- /PRODUCT LIST -->
				</div>
				<!-- /PRODUCT SHOWCASE -->

				<div class="clearfix"></div>

				<!-- PAGER -->
				<div class="pager primary">
					<div class="pager-item"><p>1</p></div>
					<div class="pager-item active"><p>2</p></div>
					<div class="pager-item"><p>3</p></div>
					<div class="pager-item"><p>...</p></div>
					<div class="pager-item"><p>17</p></div>
				</div>
				<!-- /PAGER -->
			</div>
		</div>
		<!-- /SECTION -->
		<myFooter></myFooter>
    </div>
</template>
<script>
import myNavbar from '../components/Navbar.vue'
import myFooter from '../components/Footer.vue'
export default {
  name:'home',
  data:function(){
    return{
      
    }
  },
  components:{
    myNavbar,
    myFooter
  }
}
</script>

