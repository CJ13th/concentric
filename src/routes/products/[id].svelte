<script>
    import products from '../products/product'
    import { page } from '$app/stores'

    let filtered_item = products.filter(item => item.id == $page.params.id)[0]

    const item1 = JSON.stringify(filtered_item, null, 2)
</script>

<pre>{item1}</pre>

<div class="flex">
    <img class="m-20" src={filtered_item.image} alt="test">
    <div class="m-20">
        <strong>{filtered_item.name}</strong>
        <p>{filtered_item.description}</p>
        <p>{filtered_item.base_price}</p>
    </div>
</div>