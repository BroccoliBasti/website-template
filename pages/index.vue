<template>
    <TheNavbar></TheNavbar>

    <main class="h-fit bg-hero-image bg-cover">
        <div class="container grid grid-cols-2 items-center justify-evenly w-full h-full min-h-svh">

            <Card
                class="flex flex-col gap-2 md:gap-4 justify-evenly md:justify-center bg-background rounded-lg border-2 border-accent/25 w-fit p-2 md:p-8 drop-shadow-[.5rem_.5rem_0_hsl(var(--foreground))] ">

                <h1 class="font-young font-bold text-3xl md:text-7xl">Company name</h1>
                <p class="text-base md:text-2xl">We unlock your <span
                        class="bg-clip-text text-transparent bg-gradient-to-t from-sky-700 to-sky-600 drop-shadow">full
                        potential</span> by using the right <span
                        class="bg-clip-text text-transparent bg-gradient-to-t from-rose-700 to-rose-600 drop-shadow">keywords</span>.
                </p>
                <Button class=" flex gap-2 w-fit mt-8">
                    Call to action
                    <Icon name="lucide-arrow-right" size="1rem"></Icon>
                </Button>
            </Card>

            <div
                class="flex flex-col size-fit drop-shadow-[.25rem_.5rem_0_hsl(var(--foreground))] bg-pine bg-cover bg-fixed hover:animate-bounce">
                <!-- <Icon name="lucide-hop" size="10rem" class="text-background"></Icon> -->
            </div>

        </div>
    </main>

    <TheFooter></TheFooter>
</template>