<script>
    export let title
    export let description
    export let imagen
</script>

<div class="card" style="width: 18res;">
    <img src={imagen} alt={title} width="100%" height="200">
    <div class="card-body">
        <h5 class="card-title">{title}</h5>
        <p class="card-text">{description}</p>
        <button class="btn btn-primary">More...</button>
        <button class="btn btn-danger">Favorite </button>
    </div>
</div>