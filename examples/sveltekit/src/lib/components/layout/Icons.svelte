<script lang="ts">
	// https://icones.js.org/
	import CodeIcon from '~icons/heroicons-outline/code';
	import CogIcon from '~icons/heroicons-outline/cog';
	import CollectionIcon from '~icons/heroicons-outline/collection';
	import ColorSwatchIcon from '~icons/heroicons-outline/color-swatch';
	import DatabaseIcon from '~icons/heroicons-outline/database';
	import GlobeAltIcon from '~icons/heroicons-outline/globe-alt';
	import LightningBoltIcon from '~icons/heroicons-outline/lightning-bolt';
	import ShieldCheckIcon from '~icons/heroicons-outline/shield-check';
	import TemplateIcon from '~icons/heroicons-outline/template';
	import GitHub from '~icons/mdi/github';
	import Twitter from '~icons/mdi/twitter';
	import MailIcon from '~icons/heroicons-outline/mail';
	import PasswordIcon from '~icons/wpf/password1';

	export let name;

	export let strokeWidth = 2;
	export let height = 24;
	export { extraClass as class };

	let extraClass = '';
</script>

{#if name === 'SupabaseIcon'}
	<svg fill="none" viewBox="0 0 109 113" {height} class={extraClass}>
		<path
			d="M63.708 110.284c-2.86 3.601-8.658 1.628-8.727-2.97l-1.007-67.251h45.22c8.19 0 12.758 9.46 7.665 15.874l-43.151 54.347Z"
			fill="url(#a)"
		/>
		<path
			d="M63.708 110.284c-2.86 3.601-8.658 1.628-8.727-2.97l-1.007-67.251h45.22c8.19 0 12.758 9.46 7.665 15.874l-43.151 54.347Z"
			fill="url(#b)"
			opacity="0.2"
		/>
		<path
			d="M45.317 2.071c2.86-3.601 8.657-1.628 8.726 2.97l.442 67.251H9.83c-8.19 0-12.759-9.46-7.665-15.875L45.317 2.072Z"
			fill="#3ECF8E"
		/>
		<defs>
			<linearGradient
				id="a"
				x1="53.974"
				y1="54.974"
				x2="94.163"
				y2="71.829"
				gradientUnits="userSpaceOnUse"
			>
				<stop stop-color="#249361" />
				<stop offset="1" stop-color="#3ECF8E" />
			</linearGradient>
			<linearGradient
				id="b"
				x1="36.156"
				y1="30.578"
				x2="54.484"
				y2="65.081"
				gradientUnits="userSpaceOnUse"
			>
				<stop />
				<stop offset="1" stop-opacity="0" />
			</linearGradient>
		</defs>
	</svg>
{:else if name === 'KitQL'}
	<svg width="24" height="24" viewBox="0 0 217 217" fill="none" xmlns="http://www.w3.org/2000/svg">
		<path
			fill-rule="evenodd"
			clip-rule="evenodd"
			d="M126.053 199.73C126.053 200.576 125.971 201.401 125.843 202.212C125.827 202.315 125.815 202.416 125.797 202.516C124.472 210.127 117.835 215.935 109.851 215.935C102.732 215.935 96.686 211.312 94.5152 204.917L27.0999 165.999C20.4144 162.139 16.2986 155.004 16.2986 147.29V81.7362C18.7957 82.5821 21.4584 83.0611 24.2415 83.0611C26.7386 83.0611 29.1478 82.6822 31.4215 81.9946V147.29C31.4215 149.596 32.6612 151.744 34.6639 152.899L97.552 189.207C100.526 185.737 104.93 183.526 109.851 183.526C115.205 183.526 119.942 186.143 122.896 190.156C122.949 190.229 123.004 190.299 123.057 190.372C123.263 190.665 123.459 190.964 123.647 191.273C123.719 191.391 123.792 191.506 123.862 191.627C124.028 191.91 124.181 192.201 124.329 192.495C124.41 192.653 124.485 192.811 124.558 192.972C124.686 193.245 124.804 193.521 124.916 193.802C124.997 194.003 125.067 194.204 125.14 194.407C125.23 194.663 125.318 194.922 125.393 195.183C125.469 195.434 125.524 195.685 125.587 195.933C125.644 196.169 125.704 196.402 125.75 196.641C125.813 196.954 125.853 197.271 125.898 197.589C125.92 197.783 125.958 197.966 125.976 198.157C126.023 198.676 126.053 199.198 126.053 199.73ZM208.963 58.2163C208.963 63.0775 206.805 67.4339 203.402 70.4052V147.29C203.402 155.004 199.288 162.139 192.6 165.999L134.681 199.437C134.616 193.965 132.767 188.929 129.7 184.848L185.039 152.899C187.039 151.744 188.279 149.596 188.279 147.29V73.776C181.521 71.8282 176.556 65.5971 176.556 58.2163C176.556 54.6225 177.749 51.31 179.736 48.622C179.764 48.5794 179.797 48.5368 179.829 48.4943C180.203 47.9972 180.605 47.5178 181.033 47.0661L181.091 47.0034C181.98 46.0775 182.974 45.2642 184.058 44.569C184.171 44.4962 184.288 44.4311 184.404 44.3584C184.833 44.1024 185.272 43.8589 185.724 43.6407C185.857 43.578 185.99 43.5101 186.126 43.4498C186.69 43.1938 187.273 42.9579 187.872 42.7723C187.875 42.7723 187.875 42.7723 187.875 42.7699C189.418 42.2804 191.057 42.012 192.761 42.012C201.697 42.012 208.963 49.2795 208.963 58.2163ZM16.2986 72.3253C11.3748 69.542 8.03705 64.2645 8.03705 58.2163C8.03705 49.2795 15.3049 42.012 24.2415 42.012C26.5579 42.012 28.7563 42.5111 30.7514 43.3895L99.0477 3.95875C102.388 2.02887 106.122 1.06519 109.849 1.06519C113.581 1.06519 117.313 2.02887 120.653 3.95875L178.913 37.5974C174.627 40.4886 171.307 44.6895 169.485 49.611L113.091 17.0563C112.107 16.4867 110.986 16.188 109.849 16.188C108.715 16.188 107.595 16.4867 106.609 17.0563L40.185 55.4081C40.3455 56.3215 40.4436 57.255 40.4436 58.2163C40.4436 65.188 36.009 71.1281 29.8204 73.4095C29.7727 73.4271 29.7225 73.4472 29.6773 73.4621C29.1829 73.6353 28.6885 73.7884 28.1791 73.9162C28.0762 73.9415 27.9758 73.9717 27.8729 73.9918C27.4061 74.0994 26.9293 74.185 26.45 74.2526C26.3195 74.2702 26.1915 74.2951 26.0585 74.3104C25.4612 74.3779 24.8564 74.4209 24.2415 74.4209C23.5815 74.4209 22.9315 74.3679 22.289 74.2903C22.1184 74.2702 21.9502 74.2401 21.7771 74.2124C21.2852 74.1372 20.8034 74.042 20.324 73.9214C20.1785 73.8837 20.0304 73.8511 19.8824 73.8085C18.62 73.4521 17.4179 72.9578 16.2986 72.3253Z"
			fill="#FFF"
		/>
		<path
			d="M152.111 60.4977C146.844 52.8264 138.85 47.4651 129.767 45.5128C120.684 43.5604 111.2 45.1647 103.259 49.997L75.3568 67.7792C71.5859 70.1472 68.3543 73.2843 65.8721 76.9865C63.3899 80.6887 61.7127 84.8732 60.9495 89.2678C59.5934 96.6532 60.7672 104.281 64.2803 110.914C61.8799 114.531 60.2673 118.615 59.5476 122.899C58.7578 127.366 58.8624 131.946 59.8552 136.373C60.8481 140.799 62.7094 144.983 65.3307 148.682C70.6103 156.335 78.5959 161.689 87.6679 163.657C96.7399 165.625 106.219 164.06 114.183 159.28L142.104 141.479C145.861 139.102 149.08 135.961 151.552 132.26C154.023 128.558 155.694 124.379 156.455 119.99C157.795 112.628 156.615 105.028 153.106 98.4231C156.732 92.7232 158.576 86.0662 158.398 79.3078C158.221 72.5495 156.032 65.9987 152.111 60.4977V60.4977ZM100.474 150.226C96.0913 151.369 91.4638 151.133 87.2185 149.552C82.9733 147.971 79.3153 145.12 76.74 141.385C73.5063 136.896 72.3213 131.353 73.2559 125.848L73.8017 123.195L74.3063 121.553L75.8054 122.55C79.0885 125.014 82.7801 126.878 86.7099 128.055L87.723 128.407L87.6071 129.404C87.5099 130.791 87.9174 132.35 88.7174 133.542C90.3548 135.903 93.1959 137.034 95.9398 136.292C96.5416 136.097 97.1285 135.903 97.6332 135.588L125.439 117.806C126.84 116.906 127.738 115.561 128.085 113.961C128.376 112.323 128.019 110.636 127.091 109.257C126.295 108.136 125.179 107.283 123.89 106.809C122.601 106.336 121.199 106.264 119.868 106.604C119.267 106.818 118.624 107.054 118.115 107.365L107.599 114.058C102.8 116.919 97.0977 117.849 91.6415 116.661C86.1853 115.473 81.3813 112.256 78.1979 107.657C76.6074 105.434 75.4776 102.913 74.8753 100.244C74.2731 97.5757 74.2105 94.813 74.6914 92.1197C75.1743 89.4528 76.2109 86.9173 77.7339 84.6778C79.257 82.4382 81.2325 80.5445 83.5324 79.1194L111.278 61.3371C113.052 60.2497 114.964 59.4088 116.964 58.8375C121.343 57.6986 125.966 57.9318 130.209 59.5056C134.452 61.0794 138.113 63.9184 140.698 67.6405C142.542 70.2427 143.758 73.2382 144.251 76.3915C144.744 79.5448 144.5 82.7697 143.539 85.8125L143.035 87.4727L141.595 86.4759C138.273 84.0415 134.569 82.1808 130.635 80.9707L129.64 80.6784L129.738 79.6815C129.83 78.1988 129.441 76.726 128.627 75.4842C127.844 74.3489 126.729 73.4844 125.436 73.0093C124.143 72.5343 122.735 72.472 121.405 72.8309C120.814 72.9965 120.246 73.2331 119.711 73.5355L91.8501 91.4714C90.4482 92.4083 89.551 93.7162 89.2595 95.3538C88.9679 96.9541 89.3566 98.7117 90.2538 100.001C91.8501 102.362 94.751 103.359 97.4388 102.654C98.046 102.499 98.6295 102.262 99.1734 101.95L109.805 95.1552C111.549 94.0158 113.462 93.1596 115.472 92.6181C119.855 91.466 124.486 91.6966 128.733 93.2786C132.98 94.8606 136.638 97.7171 139.207 101.459C140.796 103.672 141.931 106.18 142.546 108.837C143.161 111.494 143.243 114.247 142.788 116.936C142.327 119.596 141.313 122.128 139.81 124.368C138.307 126.609 136.35 128.506 134.066 129.936L106.261 147.677C104.453 148.773 102.508 149.626 100.478 150.215L100.474 150.226Z"
			fill="#FFF"
		/>
	</svg>
{:else if name === 'CalendarIcon'}
	<svg
		viewBox="0 0 24 24"
		fill="none"
		stroke="currentColor"
		stroke-width="2"
		stroke-linecap="round"
		stroke-linejoin="round"
		class={extraClass}
	>
		<rect x="3" y="4" width="18" height="18" rx="2" ry="2" />
		<path d="M16 2v4M8 2v4M3 10h18" />
	</svg>
{:else if name === 'TrashIcon'}
	<svg
		viewBox="0 0 24 24"
		fill="none"
		stroke="currentColor"
		stroke-width="2"
		stroke-linecap="round"
		stroke-linejoin="round"
		class={extraClass}
	>
		<path
			d="M3 6h18M19 6v14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V6m3 0V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2"
		/>
	</svg>
{:else if name === 'CommentIcon'}
	<svg
		viewBox="0 0 24 24"
		fill="none"
		stroke="currentColor"
		stroke-width="2"
		stroke-linecap="round"
		stroke-linejoin="round"
		class={extraClass}
	>
		<path
			d="M21 11.5a8.38 8.38 0 01-.9 3.8 8.5 8.5 0 01-7.6 4.7 8.38 8.38 0 01-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 01-.9-3.8 8.5 8.5 0 014.7-7.6 8.38 8.38 0 013.8-.9h.5a8.48 8.48 0 018 8v.5z"
		/>
	</svg>
{:else if name === 'PointIcon'}
	<svg viewBox="0 0 24 24" stroke="currentColor" fill="none" class={extraClass}>
		<path
			stroke-width="2"
			stroke-linecap="round"
			stroke-linejoin="round"
			d="M13 10V3L4 14h7v7l9-11h-7z"
		/>
	</svg>
{:else if name === 'UserIcon'}
	<svg
		viewBox="0 0 24 24"
		stroke="currentColor"
		stroke-width="2"
		fill="none"
		stroke-linecap="round"
		stroke-linejoin="round"
		class={`w-4 h-4 mr-1 ${extraClass}`}
	>
		<path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2" />
		<circle cx={12} cy={7} r="4" />
	</svg>
{:else if name === 'ChevronUpIcon'}
	<svg
		viewBox="0 0 24 24"
		stroke="currentColor"
		stroke-width={strokeWidth}
		fill="none"
		stroke-linecap="round"
		stroke-linejoin="round"
		class={`w-4 h-4 mr-1 ${extraClass}`}
	>
		<path d="m18 15-6-6-6 6" />
	</svg>
{:else if name === 'ChevronDownIcon'}
	<svg
		viewBox="0 0 24 24"
		stroke="currentColor"
		stroke-width={strokeWidth}
		fill="none"
		stroke-linecap="round"
		stroke-linejoin="round"
		class={`w-4 h-4 mr-1 ${extraClass}`}
	>
		<path d="m6 9 6 6 6-6" />
	</svg>
{:else if name === 'CodeIcon'}
	<svelte:component this={CodeIcon} class={extraClass} />
{:else if name === 'CogIcon'}
	<svelte:component this={CogIcon} class={extraClass} />
{:else if name === 'CollectionIcon'}
	<svelte:component this={CollectionIcon} class={extraClass} />
{:else if name === 'ColorSwatchIcon'}
	<svelte:component this={ColorSwatchIcon} class={extraClass} />
{:else if name === 'DatabaseIcon'}
	<svelte:component this={DatabaseIcon} class={extraClass} />
{:else if name === 'GlobeAltIcon'}
	<svelte:component this={GlobeAltIcon} class={extraClass} />
{:else if name === 'LightningBoltIcon'}
	<svelte:component this={LightningBoltIcon} class={extraClass} />
{:else if name === 'ShieldCheckIcon'}
	<svelte:component this={ShieldCheckIcon} class={extraClass} />
{:else if name === 'TemplateIcon'}
	<svelte:component this={TemplateIcon} class={extraClass} />
{:else if name === 'GitHub'}
	<svelte:component this={GitHub} class={extraClass} />
{:else if name === 'Twitter'}
	<svelte:component this={Twitter} class={extraClass} />
{:else if name === 'MailIcon'}
	<svelte:component this={MailIcon} class={extraClass} />
{:else if name === 'PasswordIcon'}
	<svelte:component this={PasswordIcon} class={extraClass} />
{:else}
	NOT FOUND
{/if}
