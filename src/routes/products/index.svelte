<script>
    import products from '../products/product'
    import Card from '../../components/card.svelte'

</script>

<div class="grid gap-4 md:grid-cols-3 grid-cols-1">
{#each products as product}
    <Card product={product}/>    
{/each}
</div>