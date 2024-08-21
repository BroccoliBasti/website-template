<script setup lang="ts">
import CardHeader from '~/components/ui/card/CardHeader.vue';

const products = [
    {
        name: 'Product 1',
        url: 'https://picsum.photos/320/320?random=1',
        price: 300,
    },
    {
        name: 'Product 2',
        url: 'https://picsum.photos/320/320?random=2',
        price: 300,
    },
    {
        name: 'Product 3',
        url: 'https://picsum.photos/320/320?random=3',
        price: 300,
    },
    {
        name: 'A super long title that will be too long to display at once',
        url: 'https://picsum.photos/320/320?random=4',
        price: 300,
    },
    {
        name: 'Product 5',
        url: 'https://picsum.photos/320/320?random=5',
        price: 300,
    },
    {
        name: 'Product 6',
        url: 'https://picsum.photos/320/320?random=6',
        price: 300,
    },
    {
        name: 'Product 7',
        url: 'https://picsum.photos/320/320?random=7',
        price: 300,
    },
    {
        name: 'Product 8',
        url: 'https://picsum.photos/320/320?random=8',
        price: 300,
    },
    {
        name: 'Product 9',
        url: 'https://picsum.photos/320/320?random=9',
        price: 300,
    },
    {
        name: 'Product 10',
        url: 'https://picsum.photos/320/320?random=10',
        price: 300,
    },
];

</script>

<template>
    <TheNavbar></TheNavbar>

    <main class="flex flex-col h-fit bg-hero-image bg-cover bg-fixed">
        <div class="backdrop-blur-md w-full h-full min-h-svh bg-background/25 p-8">
            <div class="container">
                <div class="grid grid-cols-1 sm:grid-cols-2 justify-between">
                    <h1 class="font-young text-4xl drop-shadow-[1px_2px_0_hsl(var(--background))]">
                        Products
                    </h1>
                    <div class="relative w-full sm:max-w-sm items-center mt-1 sm:place-self-end">
                        <Input id="search" type="text" placeholder="Search..." class="bg-card pl-10"></Input>
                        <span class="absolute start-0 inset-y-0 flex items-center justify-center px-2">
                            <Icon name="lucide-search" class="size-6 text-muted-foreground" />
                        </span>
                    </div>
                </div>
                <hr class="border-t-2 border-muted mt-2 mb-8">
                <section
                    class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 xl:grid-cols-5 gap-4 h-fit justify-items-center justify-center">
                    <Card v-for="(pic, index) in products" :key="index"
                        class="flex flex-col w-fit max-w-64 h-fit bg-card">
                        <CardContent class="p-2">
                            <a href="#" class="hover:drop-shadow-[2px_2px_2px_hsl(var(--accent))] transition-all">
                                <NuxtImg :src="pic.url" loading="lazy" width="320" height="320" class="rounded-sm">
                                </NuxtImg>
                            </a>
                        </CardContent>
                        <CardHeader class="px-2 py-0">
                            <CardTitle class="text-foreground line-clamp-1 text-ellipsis text-base leading-8">
                                {{ pic.name }}
                            </CardTitle>
                            <CardDescription class="-mt-2">
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis magnam deleniti
                                similique aspernatur maxime, delectus itaque modi nisi amet odit.
                            </CardDescription>
                        </CardHeader>
                        <CardFooter type="currency" class="flex flex-row justify-between p-2 pt-8 text-sm font-thin">
                            <a href="#">
                                <Button class="flex flex-row gap-4 group">
                                    Buy
                                    <Icon name="lucide-shopping-cart" size="1rem"
                                        class="motion-safe:group-hover:animate-wiggle">
                                    </Icon>
                                </Button>
                            </a>
                            <span class="text-lg cursor-default">
                                {{ pic.price }}€
                            </span>
                        </CardFooter>
                    </Card>
                </section>
                <UPagination class="flex justify-center pt-8"></UPagination>
            </div>
        </div>
    </main>

    <TheFooter></TheFooter>
</template>