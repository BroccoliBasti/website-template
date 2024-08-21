<script setup>

</script>

<template>
    <nav class="border-b-foreground bg-background border-2 pb-1.5">
        <div class="container flex flex-row justify-between items-center p-2">
            <a href="/" class="flex items-center gap-2 font-semibold text-2xl">
                <Icon name="lucide-heart" size="1.5rem" />
                <span class="font-young">Logo</span>
            </a>
            <ul class="flex flex-row justify-evenly list-none gap-4">
                <li class="flex items-center">
                    <a href="/products">
                        <Button class="min-h-11 min-w-11 px-8">Products</Button>
                    </a>
                </li>
                <li class="flex items-center">
                    <a href="/blog">
                        <Button class="min-h-11 min-w-11 px-8">Blog</Button>
                    </a>
                </li>
                <li class="flex items-center">
                    <a href="/about">
                        <Button class="min-h-11 min-w-11 px-8">About</Button>
                    </a>
                </li>
            </ul>
        </div>
    </nav>
</template>