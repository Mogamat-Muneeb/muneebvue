<template>


<h1><span style="color:#f01212;">CONTACT ME</span> </h1>
  <div class="containe d-flex justify-content-center" id="contact">
<!-- 
    <div class="row">
        <div class="col-xs-12 col-sm-12 col-md-12 col-lg-12 text-center">                        
          
        </div>
    </div> -->

    <div class="row">

        <div class="  ">
                <div class="call  row "> 
                <div class="call-holder col-md-4 col-lg-4"  > <i class="fas fa-phone-alt " ></i> 
                  <br> 
                      <div class="call-me fw-bold ">Call Me On:</div>
                      <div class="call-me-1 text-muted">+ 27 76 162 1649</div>
                </div>

                <div class="call-holder  col-md-4 col-lg-4"> <i class="fas fa-map-marker-alt"  ></i> 
                  <br> 
                      <div class="call-me fw-bold">Home:</div>
                      <div class="call-me-1 text-muted">Cape Town, South Africa</div>
                </div>

                <div class="call-holder  col-md-4 col-lg-4"> <i class="fas fa-envelope" ></i> 
                  <br> 
                      <div class="call-me fw-bold">Email:</div>
                      <div class="call-me-1 text-muted">davimuneeb785@gmail.com</div>
                </div>
            </div>
            <form id="contact-form" name="myForm" class="form" action="https://formspree.io/f/mvodnnke" onsubmit="return validateForm()" method="POST" role="form" target="_blank">

                <div class="form-group">
                    <label class="form-label" id="nameLabel" for="name"></label>
                    <input type="text" class="form-control" id="name" name="name" placeholder="Your name" tabindex="1">
                </div>

                <div class="form-group">
                    <label class="form-label" id="emailLabel" for="email"></label>
                    <input type="email" class="form-control" id="email" name="email" placeholder="Your Email" tabindex="2">
                </div>

                <div class="form-group">
                    <label class="form-label" id="subjectLabel" for="sublect"></label>
                    <input type="text" class="form-control" id="subject" name="subject" placeholder="Subject" tabindex="3">
                </div>

                <div class="form-group">
                    <label class="form-label" id="messageLabel" for="message"></label>
                    <textarea rows="6" cols="60" name="message" class="form-control" id="message" placeholder="Your message" tabindex="4"></textarea>                                 
                </div>

                <div class="text-center margin-top-25">
                    <button type="submit" class="btn btn-mod btn-border btn-large">Send Message</button>
                    <button type="reset" value="Reset" class="btn btn-mod btn-border btn-large">reset</button>
                </div>

            </form>
          
        </div>

    </div>
    
  </div>
</template>

<script>
export default {

}
</script>

<style>
.containe {
  display:flex;
  padding: none;
}
/* contact */
#success-message {
  opacity: 0;
}

.col-xs-12.col-sm-12.col-md-12.col-lg-12 {
  padding: 0 20% 0 20%;
}

.margin-top-25 {
  margin-top: 25px;
}

.form-title {
  padding: 25px;
  font-size: 30px;
  font-weight: 300;
  font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
}

.form-group .form-control {
  background-color: #f8f9fa;
  border-bottom: 1px;
  border-style: none none solid none;
  border-radius:0; 
  border-color: #000;
}

.form-group .form-control:focus {
	box-shadow: none;
  border-width: 0 0 2px 0;
  border-color: #000;
  
}

textarea {
  resize: none;
}

.btn-mod.btn-large {
    height: auto;
    padding: 13px 52px;
    font-size: 15px;
}

.btn-mod.btn-border {
    color: #2c3e50;
    border: 1px solid #000000;
    background: transparent;
}

.btn-mod, a.btn-mod {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    padding: 4px 13px;
    color: #fff;
    background: rgba(34,34,34, .9);
    border: 1px solid transparent;
    font-size: 11px;
    font-weight: 400;
    text-transform: uppercase;
    text-decoration: none;
    letter-spacing: 2px;
    -webkit-border-radius: 0;
    -moz-border-radius: 0;
    border-radius: 0;
    -webkit-box-shadow: none;
    -moz-box-shadow: none;
    box-shadow: none;
    -webkit-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -moz-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -o-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    -ms-transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
    transition: all 0.2s cubic-bezier(0.000, 0.000, 0.580, 1.000);
}

.btn-mod.btn-border:hover, .btn-mod.btn-border:active, .btn-mod.btn-border:focus, .btn-mod.btn-border:active:focus {
    color: white;
    border-color: #000;
    background:#f01212;
    outline: none;
    
}

@media only screen and (max-width: 500px) {
    .btn-mod.btn-large {
       padding: 6px 16px;
       font-size: 11px;
    }
  
    .form-title {
        font-size: 20px;
  }
  .containe{
    padding: 80px;
  }
}
/* .call{
  margin-left: 35%;
} */

.fas{
  display:flex;
  justify-content: center;
  font-size:35px;
  /* padding-bottom:10px; */
  color:#f01212;
}

.call-me{
  display:flex;
  justify-content: center;
}

.call-me-1{
  display:flex;
  justify-content: center;
  /* padding-top: 10px; */
}
.call-holder{
  padding-top: 15px;
}
.fas:hover{
  color:#2c3e50;
}
</style>