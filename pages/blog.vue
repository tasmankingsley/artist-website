<template>
    <div>
        <span>Blog</span>
        
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Modi iusto aperiam dicta doloremque natus eos, repudiandae laborum quam. Placeat cumque quos vero voluptate enim id minima natus ipsa quo ipsam?</p>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quod animi, nihil numquam odit aliquam hic dolor, aliquid assumenda, voluptate veritatis repudiandae quibusdam sunt et quisquam ex illum quas. Nemo, nostrum.</p>

    </div>
</template>

<style scoped>
div {
    display: grid;
    grid-template-rows: 200px 1fr;
    place-items: center;
}

p {
    text-align: left;
}



@media (min-width: 600px) {
    p {
        max-width: 600px;
    }
}
</style>