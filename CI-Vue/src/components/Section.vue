<template>
    <section>
        <article>
            <header>APELLIDOS</header>
            <span>{{apellidos}}</span>
        </article>
        <article>
            <header>NOMBRES</header>
            <span>{{nombres}}</span>
        </article>

        <div class="grid-2-colums">
            <article>
                <header>NACIONALIDAD</header>
                <span>{{nacionalidad}}</span>
            </article>
            <article>
                <header>SEXO</header>
                <span>{{sexo}}</span>
            </article>
        </div>
        <div class="grid-2-colums">
            <article>
                <header>FECHA DE NACIMIENTO</header>
                <span>{{nacimiento}}</span>
            </article>
            <article>
                <header>NÙMERO DOCUMENTO</header>
                <span>{{documento}}</span>
            </article>
        </div>
        <div class="grid-2-colums">
            <article>
                <header>FECHA DE EMISIÒN</header>
                <span>{{emision}}</span>
            </article>
            <article>
                <header>FECHA DE VENCIMIENTO</header>
                <span>{{vencimiento}}</span>
            </article>
        </div>

        <article>
            <header>FIRMA DEL TITULAR</header>
            <span>X Æ A-12</span>
        </article>
    </section>
</template>


<script>
    export default{
        name: 'Section',
        data(){
            return{
                apellidos: 'MUSK',
                nombres: 'ELON REEVE',
                nacionalidad: 'SUDAFRICANO',
                sexo: 'M',
                nacimiento: '28 JUN 1971',
                documento: '222.222.222',
                emision: '01 ENE 2025',
                vencimiento: '01 ENE 2030',  
            };
        }
    };
</script> 


<style>
    article{
        margin: 0;
        margin-bottom: 5px;
    }

    header{
        font-weight: bold;
        color: #0235a4;
        font-size: 8px;
        margin-bottom: -6px;
    }

    p{
        font-size: 20px;
        margin: 0;
        font-weight: bold;
        color: #0235a4;
    }

    section{
        margin-top: 30px;
        text-align: start;
    }

    section .grid-2-colums{
        display: grid;
        grid-template-columns: 50% 50%;
    }

    .grid-2-colums span{
        font-size: 13px;
        font-weight: 700;
        margin-bottom: 25px;
    }

    article span{
        font-size: 13px;
        font-weight: 700;
        margin-bottom: 25px;
    }

</style>