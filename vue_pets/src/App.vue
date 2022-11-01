<template>
  <div id="wrapper">

    <nav class="navbar navbar-expand-sm navbar-info bg-info">
      <div class="container-fluid">

        <a class="logo navbar-brand" href="#">
          <img src="../src/assets/logoPet.png" alt="Avatar Logo" style="width:100px;"> 
        </a>

        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#mynavbar">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="navitem collapse navbar-collapse" id="mynavbar">
          <ul class="navbar-nav me-auto ">
            <li class="nav-item">
              <a class="nav-link" href="/">Home</a>
            </li>

            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown">Gatos</a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="/cat_v">Vestuário</a></li>
                <li><a class="dropdown-item" href="/cat_b">Brinquedos</a></li>
                <li><a class="dropdown-item" href="cat_all">Tudo</a></li>
              </ul>
            </li>

            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown">Cachorros</a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="/dog_v">Vestuário</a></li>
                <li><a class="dropdown-item" href="/dog_b">Brinquedos</a></li>
                <li><a class="dropdown-item" href="/dog_all">Tudo</a></li>
              </ul>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="/all">Todos</a>
            </li>
          </ul>
          
          
          <router-link to="/login" class="botao btn btn-primary" style="margin-right: 1%">Login</router-link>

          <router-link to="/cart" class="botao btn btn-primary">
            <span class="icon"><i class="fas fa-shopping-cart"></i></span>
            <span>Carrinho</span>
          </router-link>

        </div>
      </div>
    </nav>

    <section class="section">
      <router-view/>
    </section>

  </div>
</template>

<style lang="scss">
.navitem {
  font-size: 22px;
  text-align: end;
  align-items: center;
}
.searchBotao {
  background-color: rgb(255, 102, 0);
}
.nav-link {
  color: rgb(0, 8, 126);
}
.logo {
  margin-right: 3%;
  margin-left: 1%;
}
.botao {
  background-color: rgb(255, 102, 0);
}


</style>
