<script lang="ts">
    let { title, is_paid, description, link, rating } = $props(); 
</script>

<div class="border bg-white rounded-lg p-2 shadow-md m-2">
    <h2 class="font-bold">{title}</h2>
    <p>{rating}/10</p>
    <p>{description}</p>
    <p>{is_paid}</p>
    <a href={link} target="_blank" class="text-blue-500 hover:underline">Check it out</a>
</div>