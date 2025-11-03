<script>
    import { derived } from "svelte/store";

    export let title;
    export let discription;
    export let url;
    export let buildtime;
</script>

<main>
    <h2>{title}</h2>
    <p>built {buildtime}</p>
    <p>{discription}</p>
    <a href={url}>Visit ⇱</a>
</main>

<style>
    main {
        background-color: transparent;
        color: white;
        border: white solid 1px;
        border-radius: 10px;
        padding: 5px;
    }
    div {
        display: flex;
    }
    img {
        display: inline;
        width: 24px;
        height: 24px;
    }
</style>
