<template>
    <aside class="main-sidebar sidebar-dark-primary elevation-4">
        <!-- Brand Logo -->
        <a href="#" class="brand-link">
            <img
                :src="ruta + '/img/AdminLTELogo.png'"
                alt="Sistema Logo"
                class="brand-image img-circle elevation-3"
                style="opacity: .8"
            />
            <span class="brand-text font-weight-light">Sistema</span>
        </a>

        <!-- Sidebar -->
        <div class="sidebar">
            <!-- Sidebar user (optional) -->
            <div class="user-panel mt-3 pb-3 mb-3 d-flex">
                <div class="image">
                    <img
                        :src="ruta + '/img/avatar.png'"
                        class="img-circle elevation-2"
                        alt="Wiliam"
                    />
                </div>
                <div class="info">
                    <a href="#" class="d-block">Wiliam</a>
                </div>
            </div>

            <!-- SidebarSearch Form -->
            <div class="form-inline">
                <div class="input-group" data-widget="sidebar-search">
                    <input
                        class="form-control form-control-sidebar"
                        type="search"
                        placeholder="Search"
                        aria-label="Search"
                    />
                    <div class="input-group-append">
                        <button class="btn btn-sidebar">
                            <i class="fas fa-search fa-fw"></i>
                        </button>
                    </div>
                </div>
            </div>

            <!-- Sidebar Menu -->
            <nav class="mt-2">
                <ul
                    class="nav nav-pills nav-sidebar flex-column"
                    data-widget="treeview"
                    role="menu"
                    data-accordion="false"
                >
                    <!-- Add icons to the links using the .nav-icon class
                         with font-awesome or any other icon font library -->
                    <li class="nav-item menu-open">
                        <router-link class="nav-link" :to="'/'">
                            <i class="nav-icon fas fa-tachometer-alt"></i>
                            <p>
                                Dashboard
                            </p>
                        </router-link>
                    </li>
                    <li class="nav-header">OPERACIONES</li>
                    <li class="nav-item">
                        <router-link class="nav-link" :to="'/order'">
                            <i class="nav-icon fas fa-cash-register"></i>
                            <p>
                                Pedidos
                            </p>
                        </router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" :to="'/customer'">
                            <i class="nav-icon fas fa-user-friends"></i>
                            <p>
                                Clientes
                            </p>
                        </router-link>
                    </li>
                    <li class="nav-header">CONFIGURACION</li>
                    <li class="nav-item">
                        <router-link class="nav-link" :to="'/category'">
                            <i class="nav-icon fas fa-sitemap"></i>
                            <p>Categorias</p>
                        </router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" :to="'/product'">
                            <i class="nav-icon fas fa-apple-alt"></i>
                            <p>Productos</p>
                        </router-link>
                    </li>
                    <li class="nav-header">ADMINISTRACION</li>
                    <li class="nav-item">
                        <router-link class="nav-link" :to="'/user'">
                            <i class="nav-icon fas fa-users"></i>
                            <p class="text">Usuarios</p>
                        </router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" :to="'/role'">
                            <i class="nav-icon fas fa-users"></i>
                            <p>Roles</p>
                        </router-link>
                    </li>
                    <li class="nav-item">
                        <router-link class="nav-link" :to="'/permit'">
                            <i class="nav-icon fas fa-key"></i>
                            <p>Permisos</p>
                        </router-link>
                    </li>
                </ul>
            </nav>
            <!-- /.sidebar-menu -->
        </div>
        <!-- /.sidebar -->
    </aside>
</template>

<script>
export default {
    props: ['ruta'],
    name: 'SidebarComponent'
};
</script>

<style scoped></style>
