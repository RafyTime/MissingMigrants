<script lang="ts">
    import * as DropdownMenu from "$lib/components/ui/dropdown-menu";
    import * as Popover from "$lib/components/ui/popover";
    import {Button} from "$lib/components/ui/button";
    import {Menu} from "lucide-svelte";

</script>

<header class="bg-accent sticky top-0 z-50 border-b-2 p-4">
    <div class="mx-auto max-w-screen-2xl px-8">
        <div class="flex h-16 items-center justify-between">
            <div class="md:flex md:items-center md:gap-12">
                <a class="block" href="/">
                    <h1>IU Bombicka</h1>
                </a>
            </div>

            <Popover.Root>
                <Popover.Trigger asChild let:builder>
                    <Button builders={[builder]} variant="outline">
                        <Menu />
                    </Button>
                </Popover.Trigger>
                <Popover.Content class="flex flex-col w-auto items-center" align="left-end" sideOffset="2">
                    <div class="rounded-sm p-2 w-full mx-2 text-center hover:bg-accent">
                        <a href="/">Home</a>
                    </div>
                    <div class="rounded-sm p-2 w-full mx-2 text-center hover:bg-accent">
                        <a href="/stories">Stories</a>
                    </div>
                    <div class="rounded-sm p-2 w-full mx-2 text-center hover:bg-accent">
                        <a href="/about">About</a>
                    </div>
                    <div class="rounded-sm p-2 w-full mx-2 text-center hover:bg-accent">
                        <a href="/contact">Contact</a>
                    </div>
                </Popover.Content>
            </Popover.Root>
        </div>
    </div>
</header>