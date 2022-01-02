<style>
    h1{
        font-size: 90px;
        line-height: 110px;
    }
    h2{
        font-size: 30px;
        line-height: 38px;
    }
    h1,h2{
        color: #020E35;
    }
    button{
        background: linear-gradient(270deg, #8C32F0 0%, #E73587 100%);
        font-size: 18px;
        line-height: 13px;
        height: 48px;
        border-radius: 0;
    }
    .footer{
        background-color: #020E35;
        color: white;
        font-size: 12px;
        height: 25px;
    }
</style>

<div class="container my-5">
    <div class="row">
        <div class="col">
            <h2>Questions, Comments, Concerns?</h2>
            <h1>We’d love to <span style="color: #E73587;">hear</span> from you!</h1>
        </div>
        <div class="col">
            <form>
                <div class="form-group">
                    <!-- svelte-ignore a11y-label-has-associated-control -->
                    <label>Your Email Address</label>
                    <input type="email" class="form-control" placeholder="something@website.com">
                </div>
                <div class="form-group">
                    <!-- svelte-ignore a11y-label-has-associated-control -->
                    <label>Subject</label>
                    <input type="text" class="form-control" placeholder="Question about your article">
                </div>
                <div class="form-group">
                    <!-- svelte-ignore a11y-label-has-associated-control -->
                    <label>Message</label>
                    <textarea class="form-control" id="exampleFormControlTextarea1" rows="5" placeholder="Your message starts with…"></textarea>
                </div>
                <button type="submit" class="btn btn-primary btn-lg btn-block ">Send a Message</button>
              </form>
        </div>
    </div>
    <!-- <h1>Section D</h1> -->
</div>

<div class="container-fluid m-0 p-0 footer">
    <div class="container h-100">
        <div class="row h-100 align-items-center">
            <div class="col">
                <p class="my-auto">2020 © All rights reserved by Your company name</p>

            </div>
        </div>
    </div>
</div>