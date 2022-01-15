<script>
    function scroll(event) {
        event.preventDefault();
        if (event.deltaY > 0) {
            scrollRight();
        } else {
            scrollLeft();
        }
    }

    function scrollRight() {
        // document.getElementById('content').scrollLeft += 150
        document.getElementById('content').scrollBy({
            top: 0,
            left: +380,
            behavior: 'smooth'
        })
    }
    function scrollLeft() {
        document.getElementById('content').scrollBy({
            top: 0,
            left: -380,
            behavior: 'smooth'
        })
    }

    let card = [
        { images : 'images/section-B/card-1.svg',bkg: '#FDF8E3' },
        { images : 'images/section-B/card-2.svg',bkg: '#F0F3FA' },
        { images : 'images/section-B/card-3.svg',bkg: '#FEEFF0' },
        { images : 'images/section-B/card-1.svg',bkg: '#FDF8E3' },
        { images : 'images/section-B/card-2.svg',bkg: '#F0F3FA' },
        { images : 'images/section-B/card-3.svg',bkg: '#FEEFF0' },
        { images : 'images/section-B/card-1.svg',bkg: '#FDF8E3' },
        { images : 'images/section-B/card-2.svg',bkg: '#F0F3FA' },
        { images : 'images/section-B/card-3.svg',bkg: '#FEEFF0' },
    ]
</script>

<style>
    ::-webkit-scrollbar {
        display: none;
    }
    h1{
        color: #020E35;
;
    }
    p{
        color: #2B2B2B;
        font-size: 20px;
        line-height: 25.17px;
        font-weight: 500;
    }

    .oval{
        position: absolute;
        left: 0;
    }
    button{
        background: linear-gradient(270deg, #8C32F0 0%, #E73587 100%);
        color: white;
        border-radius: 0;
        width: 140px;
        height: 40px;
        font-size: 12px;
        line-height: 15.1px;
        border: none;
    }

    .card{
        border-radius: 0;
        border: none;
        height: 583px;
        min-width: 350px;
    }

    .background{
        background: linear-gradient(0deg, rgba(2,14,53,1) 50%, rgba(255,255,255,1) 50%);
    }

    #about, #services{
        scroll-margin-top: 100px;
    }

    .arrow{
        height: 76px;
        width: 76px;
        border-radius: 100%;
        border: 2px solid white;
    }
</style>

<div id="about" class="container mt-5">
    <div class="row align-items-center">
        <img class="oval" src="images/section-B/oval.svg" alt="" srcset="">
        <div class="col px-5 text-center">
            <h1 style="margin-bottom: -10px;">About Us</h1>
            <img src="images/line.svg" alt="" srcset="">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
        </div>
    </div>

    <div id="services" class="row mt-5">
        <div class="col text-center">
            <h1 style="margin-bottom: -10px;">Our Valuable Services</h1>
            <img src="images/line.svg" alt="" srcset="">
        </div>
    </div>
</div>

<div class="container-fluid p-0 mt-4 background">

    <div class="row m-0 align-items-center justify-content-md-center">
        <div class="col-md-auto m-0 p-0">
            <button class="arrow" on:click={scrollLeft} ><img src="images/section-B/arrow.svg" alt="" srcset="" style="transform: scaleX(-1);"></button>
        </div>
        <div class="col-md-auto m-0 p-0">
            <div class="container">
                <div on:mousewheel={scroll} id="content" class="row d-flex flex-row flex-nowrap overflow-auto">

                    {#each card as {images, bkg}}
                        <div class="col">
                            <div class="card" style=" background: {bkg};">
                                <img src="{images}" class="card-img-top" alt="...">
                                <div class="card-body text-center">
                                    <p class="card-title">App Development</p>
                                    <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
                                    <button href="/" class="btn">READ MORE</button>
                                </div>
                            </div>
                        </div>
                    {/each}
                    
                </div>
            </div>
        </div>
        <div class="col-md-auto m-0 p-0">
            <button class="arrow" on:click={scrollRight} ><img src="images/section-B/arrow.svg" alt="" srcset=""></button>
        </div>
    </div>

    
</div>