<script>
    import {onMount, onDestroy} from 'svelte'
    const scrollNavBar = 60
    let show = false

    onMount(() => {
        window.onscroll = () => {
            if (window.scrollY > scrollNavBar) {
                show = true
            } else {
                show = false
            }
        }
    })
    
    onDestroy(() => {
        window.onscroll = () => {}
    })
</script>

<style>

    .scrolled { 
        transform: scale(0.6);
        transform-origin: top;
               
    }
    .scrolled:hover{
        height: 120px;
        transform: scale(1.15);
    }
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
        padding-top: 12px;
        padding-bottom: 12px;
        text-align: left;
        font-size: 12px;
        line-height: 15px;
    }

    .nav-icon{
        position: absolute;
        top: 0;
        /* height: 120px; */
    }
    .btn{
        border: none;
        transition: all 0.2s ease-in-out
    }
    .btn:hover{
        transform: scale(1.1);
    }
</style>

<div>
	<!-- <nav class:scrolled={show} style="position: fixed; z-index:9999;transition: 0.5s ease">
        elemnt
    </nav> -->
	<nav class="navbar navbar-expand-lg navbar-light bg-white py-3 fixed-top">
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
            <a class="navbar-brand" href="#home">
                <img class:scrolled={show} class="nav-icon" src="images/navbar/nav-icon.svg" alt="" style="transition: all 0.5s ease-in-out">
              </a>
    
            <div class="collapse navbar-collapse" id="navbarTogglerDemo03">
                <ul class="navbar-nav ml-auto mt-2 mt-lg-0 mr-4">
                    <li class="nav-item active">
                        <a class="nav-link" href="#home">HOME</a>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="#about">ABOUT</a>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="#services">SERVICE</a>
                    </li>
                    <li class="nav-item active">
                        <a class="nav-link" href="#portofolio">PORTOFOLIO</a>
                    </li>
                    
                </ul>
                <form class="form-inline my-0 my-lg-0 ">
                    <a class="btn nav-button border-0 m-0" href="#contact">CONTACT US</a>
                    <!-- <button class="btn btn-outline-success my-2 my-sm-0 nav-button" onclick="window.location.href='#contact'">CONTACT US</button> -->
                </form>
            </div>

        </div>
	</nav>
</div>
