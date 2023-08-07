<script lang="ts">
    import Masonry from "svelte-bricks";

    import type { PageData } from "./$types";
    export let data: PageData;

    $: items = data.items;

    let [minColWidth, maxColWidth, gap] = [400, 600, 20];
</script>

<head>
    <title>Phatsanphon's Gallery</title>
</head>

<div>
    <div>
        <Masonry {items} {minColWidth} {maxColWidth} {gap} let:item>
            <img alt="" src={item} />
        </Masonry>
    </div>
</div>
