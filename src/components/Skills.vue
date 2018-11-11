<template>
	<div class="hello ">
		<div class="holder">
			<ul>
				<li v-for="(data, index) in skills" :key="index">{{ index }}. {{ data.skill }} </li>
			</ul>
			<!--<div v-bind:style="{ backgroundColor: bgColor, width: bgWidth, height: bgHeight }"></div>-->

			<!--<div v-bind:class="{ alert: showAlert,  'another-class': showClass}"></div>-->
			<!--<p v-if="skills.length > 1"> You have more than one skill</p>-->
			<!--<p v-else>You have less than or equal one skill</p>-->
		</div>
	</div>
</template>

<script>
    export default {
        name: 'Skills',
        data() {
            return {
                skills: [
					{ "skill": "Vue.js"},
					{ "skill": "Frontend Developer" }
				],
//				bgColor: "cornflowerblue",
//				bgWidth: "100%",
//				bgHeight: "30px"
//				showAlert: true,
//				showClass: true
			}
		}
    }
</script>

<style scoped>
	.alert {
		background-color: cornflowerblue;
		width: 100%;
		height: 30px;
	}
	.another-class {
		border: 3px solid black;
	}
</style>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<!--Export css style in another file-->

<!--<style src="./Skills.css" scoped>-->

<!--</style>-->
