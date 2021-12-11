<template>
	<div class="background-gradient">
		<div class="w-full main max-w-[1440px] m-auto px-4 pt-4 md:px-24 md:pt-8">
			<!-- Navbar Components -->
			<Navbar />
			<!-- Header Section -->
			<div class="w-full flex flex-col md:flex-row px-0 md:px-[105px] pb-8">
				<!-- Heading Content -->
				<div class="w-full md:w-1/2">
					<h1 class="text-[2.75rem] leading-[1.2] md:text-heading-xl mt-14 heading">Your Freelance Business In One Place</h1>
					<p class="text-sm text-gray-500 pt-2 pb-6">Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus ut esse doloribus repellat soluta, eligendi necessitatibus.</p>
					<div class="flex flex-col md:flex-row max-w-md items-center">
						<div class="w-full md:w-[50%]">
							<input type="text" id="fullname" name="fullname" placeholder="Enter your email" class="appereance-none rounded border border-gray-200 w-full py-2.5 px-4 text-gray-700 leading-tight">
						</div>
						<!-- Button Primary / Call to Action -->
						<div class="w-full md:w-[50%]">
							<NuxtLink to="/auth/login" class="font-bold no-underline inline-block bg-blue-800 text-white border-none text-sm px-4 py-3 mr-3 leading-none bg-white border rounded  hover:border-transparent mt-4 sm:mt-0">Get Started</NuxtLink>
						</div>
					</div>
				</div>
				<!-- Heading Images -->
				<div class="w-full md:w-1/2 flex justify-center items-center mt-[1.25rem] md:mt-[-.5rem]">
					<img class="scale-[1] ml-[-20px] md:ml-4 md:scale-[1.3]" src="../static/Hero.png" alt="headingImages" width="100%">
				</div>
			</div>
			<!-- Partner Section -->
			<Slider />
			<!-- Feature Section -->
			<div class="w-full flex flex-col md:flex-row my-16 md:my-24">
				<div class="w-full md:w-1/2 mr-[100px] flex items-center">
					<div>
						<h1 class="text-[2.75rem] leading-[1.2] md:text-heading-xl mt-14 heading">Simplify Your Business.</h1>
						<p class="text-sm text-gray-500 pt-2 pb-6">We integrates and automates every step of your business from proposal to invoice. Our invoicing software has made it easy to run your business billings, so you can focus on what matters.</p>
					</div>
				</div>
				<div class="w-full md:w-1/2">
					<Benefits />
				</div>
			</div>
			<!--  Main Features Section -->
			<div class="w-full my-16 md:my-24">
				<h1 class="text-[2.75rem] leading-[1.2] md:text-heading-xl mt-14 heading mb-12 text-center">Our Main Features</h1>
				<div class="flex flex-col md:flex-row">
					<div class="flex flex-row md:w-[50%]">
						<!-- Feature 1 -->
						<div class="w-[50%] md:w-[50%] rounded-[24px] bg-white shadow-shadow-2 p-6">
							<img class="rounded-lg" src="../static/Img-Features1.png" alt="feature1">
							<h1 class="text-heading-md pt-8 fontBold">Invoice</h1>
							<p class="pt-2 text-lg-regular  text-gray-500">Create and custom invoice.</p>
						</div>
						<!-- Feature 2 -->
						<div class="w-[50%] md:w-[50%] rounded-[24px] bg-white shadow-shadow-2 p-6">
							<img class="rounded-lg" src="../static/Img-Features2.png" alt="feature1">
							<h1 class="text-heading-md pt-8 fontBold">Proposal</h1>
							<p class="pt-2 text-lg-regular  text-gray-500">Craft structured proposal.</p>
						</div>
					</div>
					<div class="flex flex-row md:w-[50%]">
						<!-- Feature 3 -->
						<div class="w-[50%] md:w-[50%] rounded-[24px] bg-white shadow-shadow-2 p-6">
							<img class="rounded-lg" src="../static/Img-Features3.png" alt="feature1" />
							<h1 class="text-heading-md pt-8 fontBold">Contract</h1>
							<p class="pt-2 text-lg-regular  text-gray-500">Generate a contract.</p>
						</div>
						<!-- Feature 4-->
						<div class="w-[50%] md:w-[50%] rounded-[24px] bg-white shadow-shadow-2 p-6">
							<img class="rounded-lg" src="../static/Img-Features4.png" alt="feature1" />
							<h1 class="text-heading-md pt-8 fontBold">Client CRM</h1>
							<p class="pt-2 text-lg-regular text-gray-500">Manage your customers.</p>
						</div>
					</div>
				</div>
			</div>
			<!-- Number Proof Section -->
			<div class="w-full my-16 md:my-24">
				<h1 class="text-[2.75rem] leading-[1.2] md:text-heading-xl mt-14 heading mb-12 text-center">Trusted by 3K+ People & Businesses</h1>
				<div class="flex flex-col md:flex-row">
					<div class="w-full flex flex-row md:w-[50%]">
						<!--Counter 1 -->
						<div class="w-[50%] md:w-[50%] rounded-lg bg-[#F7F8FD] shadow-shadow-2 mx-1 md:mx-0 mr-0 md:mr-4 py-6 text-left px-4 md:px-6">
							<h1 class="text-[4rem] fontExtraBold text-blue-800">12k+</h1>
							<p class="py-2 text-lg-regular fontBold  text-gray-500">Monthly invoices sent</p>
						</div>
						<!-- Counter 2 -->
						<div class="w-[50%] md:w-[50%] rounded-lg bg-[#F7F8FD] shadow-shadow-2 mx-1 md:mx-0 mr-0 md:mr-4 py-6 px-4 md:px-6">
							<h1 class="text-[4rem] fontExtraBold text-blue-800">5k+</h1>
							<p class="py-2 text-lg-regular fontBold  text-gray-500">Proposals created</p>
						</div>
					</div>
					<div class="flex flex-row mt-[.5rem] md:mt-0 md:w-[50%]">
						<!-- Counter 3 -->
						<div class="w-[50%] md:w-[50%] rounded-lg bg-[#F7F8FD] shadow-shadow-2 mx-1 md:mx-0 mr-0 md:mr-4 py-6 text-left px-4 md:px-6">
							<h1 class="text-[4rem] fontExtraBold text-blue-800">10k+</h1>
							<p class="py-2 text-lg-regular fontBold  text-gray-500">Contract signed</p>
						</div>
						<!-- Counter 4-->
						<div class="w-[50%] md:w-[50%] rounded-lg bg-[#F7F8FD] shadow-shadow-2 mx-1 md:mx-0 mr-0 md:mr-4 py-6 px-4 md:px-6">
							<h1 class="text-[4rem] fontExtraBold text-blue-800">10k+</h1>
							<p class="py-2 text-lg-regular fontBold text-gray-500">Countries services</p>
						</div>	
					</div>
				</div>
			</div>
			<!-- Testimonials Section -->
			<div class="w-full my-16 md:my-24">
				<h1 class="text-[2.75rem] leading-[1.2] md:text-heading-xl mt-14 heading mb-12 text-center">What Did They Say</h1>
			</div>
			<!-- Call to Action -->
			<div class="w-full mt-12 mb-24 rounded-lg py-16 md:py-20 px-4 md:px-[105px] flex flex-col md:flex-row justify-between">
				<div class="w-full md:w-1/2 cta-heading">
					<h1 class="text-[28px] md:text-[36px] fontBold">Start Your Invoicing Today!</h1>
					<p class="pt-4 text-gray-500 text-lg-regular">Get your business invoicing and collecting payments in seconds.</p>
				</div>
				<div class="w-full md:w-1/2 cta-button flex flex-col md:flex-row justify-start md:justify-end items-center mt-2 md:mt-0">
					<!-- View Pricing -->
					<NuxtLink to="/auth/register" class="w-full md:w-[40%] no-underline inline-block border-none text-sm py-3 px-4 bg-[#F7F8FD] mr-3 leading-none border rounded text-blue-800  hover:border-transparent mt-4 sm:mt-0">
						<p class="text-center">View Pricing</p>
					</NuxtLink>
					<!-- Create Free Account -->
					<NuxtLink to="/auth/login" class="w-full md:w-[60%] ml-0 md:ml-1 no-underline inline-block text-sm px-4 py-3 leading-none bg-blue-800 border-blue-800 border rounded text-white  hover:border-transparent hover:bg-white hover:text-blue-800 mt-4 sm:mt-0">
						<p class="text-center">Create Free Account</p>
					</NuxtLink>
				</div>
			</div>
		</div>
		<!-- Footer Section-->
		<Footer />
	</div>
</template>

<script>
// import Navbar Components
import Navbar from "~/components/Navbar.vue"
// import Primary Button Components
import PrimaryButton from "~/components/Button/PrimaryButton.vue"
// import Benefit Components
import Benefits from "~/components/Benefits.vue"
// import Footer Components
import Footer from "../components/Footer.vue"
// import Slider Components
import Slider from "~/components/Slider.vue"
export default {
	name: "Homepage",
	data() {
		return {
		}
	},
	components: {
		Navbar,
		PrimaryButton,
		Benefits,
		Footer,
		Slider
	},
	head: {
		title: "Timvoice - Homepage",
		meta: [
			{ charset: "utf-8" },
			{ name: "viewport", content: "width=device-width, initial-scale=1"},
			{
				hid: "invoice product",
				name: "invoice product - homepage",
				content: "invoice product - homepage"
			}
		],
		link: [
			{ rel: "icon", type: "image/x-icon", href: "/favicon.ico"},
			{ rel: "stylesheets", href: "https://fonts.googleapis.com/css2?family=Mulish:wght@400;500;600;700;800&display=swap"}
		]
	}
}
</script>

<style>
	* {
		font-family: "Mulish", sans-serif;
		box-sizing: border-box;
		margin: 0;
		padding: 0;
	}
	.background-gradient {
		height: 620px;
		background: linear-gradient(180deg, rgba(215, 221, 244, 0.5) 0%, rgba(215, 221, 244, 0) 100%);
	}
	.heading {
		font-weight: 700;
	}
	.fontBold {
		font-weight: 700;
	}
	.fontExtraBold {
		font-weight: 800;
	}
</style>