<template>
	<div class="p-heading">
		<img class="p-heading__logo" src="~/assets/images/leccafe_logo.svg" alt="lec cafeロゴ">
		<hr class="p-heading__hr">
		<h2 class="p-heading__title">手軽に始める<br><br>プログラミング<br><br>スクール</h2>
		<div class="p-heading__description">
			<img class="p-heading__descriptionImage" src="~/assets/images/p-hero_img01@2x.png" alt="スクールイラスト">
			<p class="p-heading__descriptionText">Lec Cafeは学生や社会人を対象とした<br>大阪のプログラミングスクールです。</p>
		</div>
		<div class="p-heading__descriptionBtns">
			<router-link class="p-heading__descriptionBtnsItem c-buttonWhite c-fs20 c-fwBold" to="">資料請求</router-link>
			<router-link class="p-heading__descriptionBtnsItem c-buttonRed c-fs20 c-fwBold" to="">申し込み</router-link>
		</div>
	</div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "~/assets/scss/mixins/container.scss";
@import "~/assets/scss/component/button.scss";

	.p-heading {
		@include container();
		padding: 81px 20px 0;
		&__logo {
			width: 200px;
			height: 46px;
		}
		&__hr {
			margin: 30px 0 20px 0;
			height: 1px;
			width: 160px;
			background-color: #E15F52;
		}
		&__title {
			font-size: 18px;
			font-weight: bold;
		}
		&__description {
			text-align: right;
			position: relative;
			top: -45px;
			margin-bottom: 20px;
		}
		&__descriptionText {
			text-align: left;
		}
		&__descriptionBtns {
			display: flex;
			justify-content: space-around;
			position: relative;
			top: -45px;
		}
		&__descriptionBtnsItem {
			width: 160px;
			height: 50px;
		}
		&__descriptionBtnsItem:nth-child(odd):hover {
            @include buttonWhiteHover();
		}
		&__descriptionBtnsItem:nth-child(even):hover {
            @include buttonRedHover();
		}
		&__descriptionImage {
			width: 90%;
			margin-bottom: 20px;
		}
	}

	@media screen and (min-width: 768px) {
	.p-heading {
		height: 800px;
		padding-top: 100px;
		&__logo {
			width: 302px;
			height: 65px;
		}
		&__hr {
			width: 244px;
		}
		&__title {
			font-size: 24px;
		}
		&__descriptionImage {
			width: 600px;
			position: relative;
			top: -150px;
		}
		&__descriptionText {
			position: relative;
			top: -225px;
		}
		&__descriptionBtns {
			position: relative;
			top: -250px;
			justify-content: left;
		}
		&__descriptionBtnsItem {
			margin-right: 20px;
			width: 200px;
			height: 50px;
			font-size: 24px;
		}
	}
}

</style>
