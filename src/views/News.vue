<template>
    <div class="my-news">
		<my-navbar></my-navbar>
			<!-- SECTION HEADLINE -->
		<div class="section-headline-wrap">
			<div class="section-headline">
				<h2>Latest News</h2>
				<p>Home<span class="separator">/</span><span class="current-section">News</span></p>
			</div>
		</div>
		<!-- /SECTION HEADLINE -->

		<!-- SECTION -->
		<div class="section-wrap">
			<div class="section">
				<!-- BLOG POST PREVIEW -->
				<div class="blog-post-preview v1 column3-wrap">
					<!-- BLOG POST PREVIEW ITEM -->
					<div class="blog-post-preview-item column"
					v-for="item in news" :key="item.title">
						<a href="#">
							<figure class="product-preview-image big liquid">
								<img src="../assets/images/blog/01s.jpg" alt="">
							</figure>
						</a>
						<!-- BLOG POST PREVIEW ITEM INFO -->
						<div class="blog-post-preview-item-info">
							<p class="text-header mid">
								<a href="#">{{item.title}}</a>
							</p>
							<div class="meta-line">
								<a href="#">
									<p class="category primary">Design Inspires</p>
								</a>
								<p>March 15th, 2015</p>
							</div>
							<p class="description-preview">{{item.body}}</p>
							<a href="#" class="more-button primary">Read More...</a>
						</div>
						<!-- /BLOG POST PREVIEW ITEM INFO -->
					</div>
					<!-- /BLOG POST PREVIEW ITEM -->
				</div>
				<!-- /BLOG POST PREVIEW -->

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
		<my-footer></my-footer>
    </div>
</template>
<script>
import myNavbar from '../components/Navbar.vue'
import myFooter from '../components/Footer.vue'
export default {
  name:'news',
  data:function(){
    return{
      news:[
		  {title:'news 1',body:'alskjdfl jsdjflsakdj kjdklj ds jsdkjjlds lkjdlfjd jf'},
		  {title:'news 2',body:'alskjdfl jfgdakdj dfgdfj ds jsdkjjlds lkjdlfjd gsddg'},
		  {title:'news 3',body:'alskjdfl jsdjfldgdfgkdj kjdklj dfg jsdkjjlds lkjdlfjd jf'},
		  {title:'news 4',body:'alskjdfl jsdjflsakdj kjdklj ds jsdkjjlds lkjdlfjd fgdsf'}
	  ],
	  arjun:'hello'
    }
  },
  components:{
    myNavbar,
    myFooter
  }
}
</script>