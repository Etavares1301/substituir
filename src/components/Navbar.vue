<template>
  <div id="nav">
    <router-link to="/" id="logo-url">
        <img :src="logo" :alt="alt" id="logo">
    </router-link>          
    <router-link to="../views/releases">Lançamentos</router-link>
    <router-link to="../views/AccountRegistration">Cadastro de Contas</router-link>
    <router-link to="../views/reports">Relatórios</router-link>
    <router-link to="../views/dashboards">Análises</router-link>    
    <p>bem vindo,</p>
    <label for="name">{Eduardo}</label>
    <router-link to="/login">Sair</router-link>
  </div>  
</template>
<script>
export default {
    name: "Navbar",
    props: ["logo", "alt"]
};
</script>
<style>
#nav {
    background-color: #222;
    border-bottom: 4px solid #0000;
    padding: 15px 50px;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    max-height: 70px;      
}

#nav #logo-url {
    margin: auto;
    margin-left: 0;
}

#logo {
    width: 250px;
    height: 50px;
    margin-top: -5px;
}

#nav a {
    color:chartreuse;
    text-decoration: none;
    margin: 12px;
    transition: .5s;
    margin-top: 17px;
}

#nav a:hover {
    color: #fcba03;
}

.nav p {
    color: #dcdcdc;
}
</style>