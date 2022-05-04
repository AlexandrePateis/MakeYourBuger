<template>
    <div>
        <p>Componente de Mensagem</p>
        <div>
            <form class="burger-form">
                <div class="input-container">
                    <label for="nome">Nome do cliente:</label>
                    <input type="text" id="nome" name="nome" v-model="nome" placeholder="Digite o seu nome">
                </div>
                <div class="input-container">
                    <label for="pao">Escolha o pão:</label>
                    <select name="pao" id="pao" v-model="pao">
                        <option value="">Selecioneo seu pao</option>
                        <option value="integral">Integral</option>
                    </select>
                </div>
                <div class="input-container">
                    <label for="carne">Escolha a carne do seu burger:</label>
                    <select name="carne" id="carne" v-model="carne">
                        <option value="">Selecioneo seu carne</option>
                        <option value="maminha">Maminha</option>
                    </select>
                </div>
                <div  class="input-container">
                    <label for="opcionais">Selecione os opcionais:</label>
                    <div class="checkbox-container" id="opcionais-contanier">
                        <input type="checkbox" name="opcioanis" id="opcionais" v-model="opcionais" value="salame">
                        <span class="title-op">Salame</span>
                    </div>
                    <div class="checkbox-container" id="opcionais-contanier">
                        <input type="checkbox" name="opcioanis" id="opcionais" v-model="opcionais" value="salame">
                        <span class="title-op">Salame</span>
                    </div>
                    <div class="checkbox-container" id="opcionais-contanier">
                        <input type="checkbox" name="opcioanis" id="opcionais" v-model="opcionais" value="salame">
                        <span class="title-op">Salame</span>
                    </div>
                </div>
                <div class="input-container">
                   <input type="submit" class="submit-btn" value="Criar meu Burger">
                </div>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name:"BurgerForm"
}
</script>

<style scoped>

.burger-form{
    width: 25em;
    margin: 0 auto;
}
.input-container{
    display: flex;
    flex-direction: column;
    margin-bottom: 30px;
}
input, select{
    padding: 10px;
}
label {
    font-weight: bold;
    margin-bottom: 15px;
    color: #222;
    border-left: 4px solid yellow;
    padding: 5px 10px;
}
.checkbox-container{
    display: flex;
    align-items: flex-start;
    width: 50%;
    margin-bottom: 20px;
}
#opcionais-contanier{
    flex-direction: row;
    flex-wrap: wrap;
}
.title-op{
    width: 100%;
}
.checkbox-container span, .checkbox-container input{
    width: auto;

}
.checkbox-container span{
    margin-left: 6px;
    font-weight:  bold;
}
.submit-btn{
    cursor: pointer;
    color: yellow;
    font-weight: bold;
    border: 2px solid #222;
    padding: 10px;
    font-size: 16px;
    margin: 0 auto;
    background: black;
    border-radius:10px;
    transition: 0.2s linear;
    width: 15em;
}
.submit-btn:hover{
    background:transparent;
    color: black;
}
</style>