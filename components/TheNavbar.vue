<script setup>

</script>

<template>
    <nav class="border-b-foreground border-2 pb-1.5">
        <div class="container flex flex-row justify-between items-center p-2">
            <div class="flex items-center gap-2 font-semibold text-4xl">
                <Icon name="lucide-heart" size="2rem" />
                <span>Logo</span>
            </div>
            <ul class="flex flex-row justify-evenly list-none gap-4">
                <li class="flex items-center">
                    <a href="#">
                        <Button class="min-h-11 min-w-11 px-8">Link</Button>
                    </a>
                </li>
                <li class="flex items-center">
                    <a href="#">
                        <Button class="min-h-11 min-w-11 px-8">Link</Button>
                    </a>
                </li>
                <li class="flex items-center">
                    <a href="#">
                        <Button class="min-h-11 min-w-11 px-8">Link</Button>
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>