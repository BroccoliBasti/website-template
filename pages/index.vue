<template>
    <TheNavbar></TheNavbar>

    <main class="flex flex-row justify-center h-svh bg-hero-image bg-cover">

        <div
            class="container flex flex-col justify-evenly md:justify-center gap-2 md:gap-8 bg-background/25 backdrop-blur-sm p-2 md:p-8">

            <h1 class="font-bold text-3xl md:text-7xl">Company name</h1>
            <p class="text-base md:text-2xl">We unlock your <span
                    class="bg-clip-text text-transparent bg-gradient-to-r from-orange-600 to-pink-500 drop-shadow">full
                    potential</span> by using the right <span
                    class="bg-clip-text text-transparent bg-gradient-to-r from-orange-600 to-pink-500 drop-shadow">keywords.</span>
            </p>
            <Button class="w-fit">Call to action</Button>
        </div>

        <div>
            <Icon name="lucide-hop" size:></Icon>
        </div>

    </main>

    <TheFooter></TheFooter>
</template>