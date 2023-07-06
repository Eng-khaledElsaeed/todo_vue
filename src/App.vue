<template>
	<h1>My Todo List</h1>
<div class="grid">
	<todo_list></todo_list>
	<todo_history></todo_history>
</div>
</template>

<script>
import todo_list from "./components/todo.vue";
import todo_history from "./components/todo_history.vue";

export default {
components: {
	todo_list,
	todo_history
}
}
</script>
  


<style lang="scss">
$size1: 6px;
$size2: 12px;
$size3: 18px;
$size4: 24px;
$size5: 48px;

$backgroundColor: #27292d;
$textColor: white;
$primaryColor: #a0a4d9;
$secondTextColor: #1f2023;
body {
	margin: 0;
	padding: 0;
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	background-color: $backgroundColor;
	color: $textColor;
	h1{
		font-weight: bold;
		text-align: center;
	}
	.grid{
    display: grid;
    grid-template-columns: 1fr 1fr;
	margin-left: auto;
	margin-right: auto;
	padding: 20px;
	max-width: 90%;
    gap:.5rem 2rem;
}
}
</style>
