
<script>
    export let product
</script>


<div class="card text-center shadow-2xl">
    <figure class="px-10 pt-10 flex justify-center">
      <img src={product.image} class="rounded-xl image">
    </figure> 
    <div class="card-body">
      <h2 class="card-title">{product.name}</h2> 
      <p>{product.description}</p> 
      <div class="justify-center card-actions">
        <a href={`/products/${product.id}`} class="btn btn-outline btn-primary">More info</a>
      </div>
    </div>
  </div>


<style>
    .image {
        max-width: 200px;
        max-height: 200px;
    }
</style>