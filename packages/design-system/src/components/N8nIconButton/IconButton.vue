<template functional>
	<n8n-button v-bind="props" v-on="listeners" />
</template>

<script lang="ts">
import N8nButton from '../N8nButton';

export default {
	name: 'n8n-icon-button',
	components: {
		N8nButton,
	},
	props: {
		type: {
			type: String,
		},
		title: {
			type: String,
		},
		size: {
			type: String,
			default: 'medium',
		},
		loading: {
			type: Boolean,
			default: false,
		},
		disabled: {
			type: Boolean,
			default: false,
		},
		icon: {
			required: true,
		},
		theme: {
			type: String,
		},
		circle: {
			type: Boolean,
			default: true,
		},
	},
};
</script>
