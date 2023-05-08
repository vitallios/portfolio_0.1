<template>
    <div>

        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 justify-between flex">
                <ul class="flex gap-4">
                    <li>
                        <NuxtLink to="/">To home</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/contacts">To contacts</NuxtLink>
                    </li>
                </ul>
                <div>
                    <NuxtLink class="btn" to="/products">To products</NuxtLink>
                </div>
            </nav>

        </header>

        <div class="container mx-auto p-4">
            <slot />
        </div>

    </div>
</template>