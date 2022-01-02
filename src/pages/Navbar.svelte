<script>
</script>

<style>
    .navbar{
        box-shadow: 0px 2px 10px rgba(0, 0, 0, 0.1);
    }
    .nav-item{
        margin-right: 60px;
    }
    .nav-link{
        font-size: 12px;
        letter-spacing: 0.8px;
        font-weight: normal;
        line-height: 15px;
        color: black;
    }

    .nav-button{
        background: linear-gradient(270deg, #8C32F0 0%, #E73587 100%);
        color: white;
        border-radius: 0;
        width: 107px;
        height: 40px;
        text-align: left;
        font-size: 12px;
        line-height: 15px;
    }

    .nav-icon{
        position: absolute;
        top: 0;
    }
</style>

<div>
	<!-- <h1>Navbar</h1> -->
	<nav class="navbar navbar-expand-lg navbar-light bg-white py-3">
        <div class="container">
            <button
                class="navbar-toggler"
                type="button"
                data-toggle="collapse"
                data-target="#navbarTogglerDemo03"
                aria-controls="navbarTogglerDemo03"
                aria-expanded="false"
                aria-label="Toggle navigation"
            >
                <span class="navbar-toggler-icon" />
            </button>
            <img class="img-fluid nav-icon" src="images/navbar/nav-icon.svg" alt="">
            <a class="navbar-brand" href="/">Navbar</a>
    
            <div class="collapse navbar-collapse" id="navbarTogglerDemo03">
                <ul class="navbar-nav ml-auto mt-2 mt-lg-0 mr-4">
                    <li class="nav-item active">
                        <a class="nav-link" href="/">HOME</a>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="/">ABOUT</a>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="/">SERVICE</a>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="/">PORTOFOLIO</a>
                    </li>
                    
                </ul>
                <form class="form-inline my-2 my-lg-0">
                    <button
                        class="btn btn-outline-success my-2 my-sm-0 nav-button"
                        type="submit">CONTACT US</button
                    >
                </form>
            </div>

        </div>
	</nav>
</div>
