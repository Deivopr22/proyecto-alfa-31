<script>

    const {name, description, image} = $props()

</script>

<section>
    <div>
        <img src={image} alt="">
    </div>

    <div>
        <p>{name}</p>
        <p>{description}</p>
    </div>
</section>