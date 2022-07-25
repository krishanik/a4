{#each Array(50) as x}
<page>
    <div style="width:100%;height:100%; background-color: yellow; border:2px solid green;">
    <h1>Welcome to SvelteKit</h1>
    <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
    </div>
</page>
{/each}

<style>
	:global(html),
	:global(body) {
		background: rgb(204, 204, 204);
		margin: 0px!important;
		pading: 0px!important;
		-webkit-print-color-adjust: exact;
	}

	*,
	*:before,
	*:after {
		-webkit-box-sizing: border-box;
		-moz-box-sizing: border-box;
		box-sizing: border-box;
	}

	page {
		background: white;
		display: block;
	}

    @media only screen{
        page {
		    margin: 0 auto;
            margin-bottom: 0.5cm;
            box-shadow: 0 0 0.5cm rgba(0, 0, 0, 0.5);
        }
	}

    @page {
        /* size: auto; */
        size: A4 landscape;
    }

	page{
        width: 297mm;
        height: 209.81mm;
	}

	@media print {

		body,
		page {
			margin: 0;
			box-shadow: 0;
		}
	}
</style>