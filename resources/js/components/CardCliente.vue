<template>
    <div>
        <div class="uk-card uk-card-default">
            <div class="uk-card-media-top">
                <img :src="logo" :alt="nome" />
            </div>
            <div class="uk-card-body">
                <h3 class="uk-card-title">{{ nome }}</h3>
                <p>{{ telefone }}</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props:['nome','telefone','logo']
}
</script>