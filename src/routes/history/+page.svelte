<script>
	import {
		Timeline,
		TimelineItem,
		TimelineSeparator,
		TimelineDot,
		TimelineConnector,
		TimelineContent,
		TimelineOppositeContent
	} from 'svelte-vertical-timeline';

	const options = [
		{
			title: 'Data Science Intern',
			description: {
				year: '2022',
				name: 'Direct Supply',
				link: 'https://www.directsupply.com/'
			}
		},
		{
			title: 'App developer',
			description: {
				year: '2021',
				name: 'Circa',
				link: 'https://circaworks.com/'
			}
		},
		{
			title: 'Research Assistant',
			description: {
				year: '2020',
				name: 'Inception Health',
				link: 'https://inceptionlabs.org/'
			}
		},
		{
			title: 'IT Student worker',
			description: {
				year: '2019',
				name: 'Martin Luther College',
				link: 'https://mlc-wels.edu/'
			}
		},
		{
			title: 'Student Tutor',
			description: {
				year: '2019',
				name: 'MSOE',
				link: 'https://www.msoe.edu/'
			}
		}
	];
</script>

<p>Previous experience:</p>
<Timeline position="alternate">
	{#each options as option}
		<TimelineItem>
			<TimelineOppositeContent slot="opposite-content">
				{#if 'description' in option}
					<p id="desc">
						{option.description.year} -
						<a target="_blank" href={option.description.link}>{option.description.name}</a>
					</p>
				{/if}
			</TimelineOppositeContent>
			<TimelineSeparator>
				<TimelineDot />
				<TimelineConnector />
			</TimelineSeparator>
			<TimelineContent>
				<p>{option.title}</p>
			</TimelineContent>
		</TimelineItem>
	{/each}
</Timeline>

<style>
	#desc, a {
		color: grey;
	}
</style>
