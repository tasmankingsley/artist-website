<template>
    <div>
        <Nav/>
        <div class="slot">
            <slot/>
        </div>
    </div>
</template>

<style scoped>
a {
    color: red;
}

@media (min-width: 600px) {
    .slot {
        margin-left: 25%;
        margin-right: 25%;
    }
}
</style>