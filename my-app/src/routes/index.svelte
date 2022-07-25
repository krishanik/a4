{#each Array(50) as x}
<div class="page">
    <div style="width:100%;height:100%; background-color: yellow; border:2px solid green">
    <h1>Welcome to SvelteKit</h1>
    <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
    </div>
</div>
{/each}

<style>
	:global(html,body) {
		background: rgb(204, 204, 204);
		margin: 0px!important;
		padding: 0px!important;
		-webkit-print-color-adjust: exact;
	}
    h1{
        margin:0;
    }

    :global(*,
	*:before,
	*:after) {
		-webkit-box-sizing: border-box;
		-moz-box-sizing: border-box;
		box-sizing: border-box;
	}

	.page{
        padding: 0;
        width: 297mm;
        height: 209.8185mm;
	}

</style>