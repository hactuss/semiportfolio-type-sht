<script>
	let svelte_logo = 'https://upload.wikimedia.org/wikipedia/commons/1/1b/Svelte_Logo.svg';
	let javascript_logo =
		'https://imgs.search.brave.com/2Lop95efMN3mNn8YORMHw4gXlmuiYbR1SXVpQQV4NCo/rs:fit:500:0:0:0/g:ce/aHR0cHM6Ly91cGxv/YWQud2lraW1lZGlh/Lm9yZy93aWtpcGVk/aWEvY29tbW9ucy90/aHVtYi85Lzk5L1Vu/b2ZmaWNpYWxfSmF2/YVNjcmlwdF9sb2dv/XzIuc3ZnLzI1MHB4/LVVub2ZmaWNpYWxf/SmF2YVNjcmlwdF9s/b2dvXzIuc3ZnLnBu/Zw';
	//let screenshot = [ss_ccenter, ss_Worldclock, ss_spookymonth];

	let cypher = ['a', 1, 'b', 2, 'c', 3];

	function decrypt() {
		console.log('hello'.slice(2));
	}
	decrypt();

	let number = $state(1);
	$effect(() => {
		setInterval(() => {
			return number++;
		}, 1000);
	});
</script>

{#if false}
	<div>
		<FAQCard
			question="What does HAJ mean?"
			answer="HAJ is an alias for domains that I use. For example, the website
                  uses this alias to shorten the URL. Otherwise, this would be unnecisarely
                  long if it was called hactuss-links.vercel.app.
              "
		/>
	</div>
{/if}
