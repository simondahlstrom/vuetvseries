<template>
    <nav valign="bottom" class="container navbar navbar-expand-md navbar-light bg-light">
    <a href="/" class="navbar-brand"></a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar5">
        <span class="navbar-toggler-icon"></span>
    </button>
    <div class="navbar-collapse collapse justify-content-stretch" id="navbar5">
        <ul class="navbar-nav">
            <li class="nav-item active">
                <a class="nav-link" href="#">Movies <span class="sr-only">Home</span></a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#">Series</a>
            </li>           
        </ul>
        <form class="ml-3 my-auto d-inline w-100">
            <div class="input-group">
                <input type="text" class="form-control border-right-0" placeholder="...">
                <div class="input-group-append">
                    <button class="btn btn-outline-primary border-left-0" type="button">SÖK</button>
                </div>
            </div>
        </form>
    </div>
</nav>

</template>

<script>
export default {
    name: 'Navigation'
}
</script>

<style scoped>
    nav{
        padding: 15px;
    }
</style>