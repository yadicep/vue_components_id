<template>
    <aside>
        <div>
            <span>CEDULA DE INDENTIDAD</span>
            <img :src="imgBandera" width="40"/>
        </div>
        <img :src="imgFoto"/>
        <p>{{ run }}</p>
    </aside>
</template>

<script>
    import imgBandera from '../assets/img/chile_bandera.png';
    import imgFoto from '../assets/img/foto_elon.jpg';
    export default{
        name: 'Aside',
        data(){
            return{
                imgBandera,
                imgFoto,
                run: '22.222.222-2'    
            };
        }
    };
</script>  

<style>
    aside div{
        display: flex;
    }

    aside > img{
        margin-top: 15px;
        width: 100%;
    }

    aside p{
        text-align: center;
        font-size: 12px;
        font-weight: bold;
        margin-top: 0;
        color: black;
    }
    
    aside span{
        text-align: start;
    }
</style>