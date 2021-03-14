<template>
<div>
    <todoamount :todos="todos"/>

	<div v-for="(item, i) in todos" :key="item.id">
		<p>
		<span class="todo_id">{{ i+1 }}. </span>
		<span class="todo_text" :class="{isShow: item.isComplete}">{{ item.text }}</span>
		<input v-model="item.isComplete" type="checkbox" />
		<br>
		<button @click="removeItem(i)">Remove ToDo</button>
		</p>
	</div>
</div>
</template>

<script>
 import todoamount from './todoamount.vue';

export default({
	components:{
		todoamount
	},
	props:{
		todos: {
			type: [Object, Array],
			required: true
		},
		removeTodo:{
			type: Function
		}
	},
	methods: {
		removeItem(index){
			this.$emit('removeTodo', index);
		}
	},
})
</script>
