<script lang="ts">
    export let valor: string

    $: tamanhoFonte = valor.length > 20 ? 'pequena' : `s-${valor.length }`
</script>

<div class={`tela ${tamanhoFonte}`}>
    <span>{valor}</span>
</div>

<style>
    .tela{
        display: flex;
        flex: 1;
        justify-content: flex-end;
        align-items: center;
        padding: 0px 5px;
        font-size: 1.7rem;
        background-color: aliceblue;
        overflow: hidden;
        margin: 2px 1px;
        border-top-right-radius: 5px;
        border-top-left-radius: 5px;
    }

    .s-10{font-size: 1.55rem;}
    .s-11{font-size: 1.40rem;}
    .s-12{font-size: 1.30rem;}
    .s-13{font-size: 1.20rem;}
    .s-14{font-size: 1.12rem;}
    .s-15{font-size: 1.05rem;}
    .s-16{font-size: 0.98rem;}
    .s-17{font-size: 0.93rem;}
    .s-18{font-size: 0.87rem;}
    .s-19{font-size: 0.82rem;}
    .s-20{font-size: 0.77rem;}
    .pequena{font-size: 0.6rem;}
</style>