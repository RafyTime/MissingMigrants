<script lang="ts">

import PowerBITest from "./components/PowerBITest.svelte";
import Story from "./components/Story.svelte";
</script>


<main>
    <div class="flex flex-col gap-12">
        <div class="flex flex-col gap-8 mb-10">
            <div>
                <h1>Unveiling The Journey | Missing Migrants</h1>
                <h2>something to put here</h2>
            </div>
            <div class="border-4">
                <PowerBITest class="https://app.powerbi.com?tenant=f419c9fe-f7b0-4d87-bee8-e8dfb2190cab&UPN=damian.romeikat@iu-study.org" />
            </div>
        </div>

        <div class="mb-10">
            <Story />
        </div>
    </div>
</main>

