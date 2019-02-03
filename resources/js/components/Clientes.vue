<template>
    <div>
        <h1>Listar clientes</h1>
        <div class="uk-grid uk-grid-small uk-child-width-1-3">
        <card-cliente v-for="i in clientes" :key="i.id" :nome="i.nome" :telefone="i.telefone" :logo="i.logo"></card-cliente>
        </div>     
    </div>
</template>

<script>
export default {
    data(){
        return {
            clientes: [
                {nome:'Banco Inter',id: 1,telefone:'(31) 87989-987456',categoria_id: 1,logo:'assets/img/logo/logo1.jpg'},
                {nome:'99 Pop',id: 2,telefone:'(31) 456789-787546',categoria_id: 2,logo:'assets/img/logo/logo2.png'},
                {nome:'Empresa do UU',id: 3,telefone:'(31) 78898-787985',categoria_id: 1,logo:'assets/img/logo/logo3.jpg'},
                {nome:'Outro Banco Inter',id: 4,telefone:'(31) 87989-987456',categoria_id: 2,logo:'assets/img/logo/logo1.jpg'},
                {nome:'Copia do  Uber 99 Pop',id: 5,telefone:'(31) 456789-787546',categoria_id: 1,logo:'assets/img/logo/logo2.png'},
                {nome:'Outro Empresa do UU',id: 6,telefone:'(31) 78898-787985',categoria_id: 2,logo:'assets/img/logo/logo3.jpg'}
            ],
            categorias:[
                {nome:'Restaurante',id: 1, link:'/restaurantes', capa:['assets/img/restaurante1.jpg','assets/img/restaurante2.jpg']},
                {nome:'Academia',id: 2, link:'/academias', capa:['assets/img/academia1.jpg','assets/img/academia2.jpg']}
            ]
        }
    }
}
</script>