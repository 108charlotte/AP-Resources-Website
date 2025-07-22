<script lang="ts">
    let { title, is_paid, description, link, rating } = $props(); 
</script>

<div class="border bg-white rounded-lg p-2 shadow-md m-2">
    <h2 class="font-bold">{title}</h2>
    <p class="text-green-500">{rating}/10</p>
    <p class="text-yellow-500">{is_paid}</p>
    <p>{description}</p>
    <a href={link} target="_blank" class="text-blue-500 hover:underline">Check it out</a>
</div>