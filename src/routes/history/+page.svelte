<script>
	import {
		Timeline,
		TimelineItem,
		TimelineSeparator,
		TimelineDot,
		TimelineConnector,
		TimelineContent
	} from 'svelte-vertical-timeline';

	const options = [
		{ title: 'Data Science Intern' },
		{ title: 'App developer' },
		{ title: 'Research Assistant' },
		{ title: 'IT Student worker' },
		{ title: 'Student Tutor' }
	];
</script>

<p>Previous experience:</p>
<Timeline position="alternate">
	{#each options as option}
		<TimelineItem>
			<TimelineSeparator>
				<TimelineDot />
				<TimelineConnector />
			</TimelineSeparator>
			<TimelineContent>
				<a href="/">{option.title}</a>
			</TimelineContent>
		</TimelineItem>
	{/each}
</Timeline>

<style>
</style>
