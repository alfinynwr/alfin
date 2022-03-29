# alfin
create my address
<!DOCTYPE html>
<html lang="en">

<head>
  <title>$(identity) </title>
  <link rel="icon" type="image/x-icon" href="img/favicon.ico">
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0">
  <meta http-equiv="pragma" content="no-cache" />
  <meta http-equiv="expires" content="-1" />

  <link href="css/bootstrap.min.css" rel="stylesheet">
  <link href="css/bootstrap.css" rel="stylesheet">
  <link href="css/style.css" rel="stylesheet">



</head>

<body>




  <!--Navbar Open-->
  <nav class="navbar navbar-default example6 navbar-fixed-top">
    <div class="container">
      <div class="navbar-header">
        <button type="button" class="navbar-toggle collapsed tombol-nav" data-toggle="collapse" data-target="#navbar6">
          <span class="sr-only">Toggle navigation</span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </button>
        <a class="navbar-brand text-hide" href="login.html">Brand Text
        </a>
      </div>
      <div id="navbar6" class="navbar-collapse collapse">
        <ul class="nav navbar-nav navbar-right ">

          <li><a href="login.html" class="link-aktif">Home</a></li>


          <!--jika login-->
          $(if logged-in == 'yes')
          <li class="dropdown">
            <a class="dropdown-toggle dodown" class="tanpa-link" data-toggle="dropdown" href="#">Status
              <span class="caret"></span></a>
            <ul class="dropdown-menu">
              <li><a href="status.html">Cek Masa Aktif</a></li>
              <li><a href="logout.html">Logout</a></li>

            </ul>
          </li>
          $(endif)
          <!--jika login-->

        </ul>
      </div>

    </div>

  </nav>
  <!--Navbar Close-->

  <!--konten open-->
  <div class="container">
    <div class="col-md-10 col-md-offset-1 col-sm-8 col-sm-offset-2 box-utama" style="padding:0px;">



      <!--kiri open-->
      <div class="col-md-4 col-sm-12" style="padding:15px;">

        <img src="img/logo.png" class="img-responsive" style="margin-bottom:5px;">

      
     $(if error)
        <div style="color:#DF1A23; font-weight:bold; margin-bottom:5px;" class="kecil">
          <script type="text/javascript">
            var error = "$(error)";
            var error1 = "user $(username) has reached uptime limit";
            var error2 = "invalid password";
            var error3 = "no valid profile found";
            var error4 = "user &lt;$(username)&gt; not found";
            var error5 = "no more sessions are allowed for user $(username)";
            var error6 = "session limit reached ($(error-orig))";
            var error7 = "web browser did not send challenge response (try again, enable JavaScript)";
            var error8 = "invalid username or password";
            var error9 = "user $(username) is not allowed to log in from this MAC address";
            var error10 = "simultaneous session limit reached";
            var error11 = "user $(username) has reached traffic limit";
            var error12 = "uptime limit reached";
            var error13 = "invalid Calling-Station-Id";



            if (error == error1) {
              window.location.href = "expired.html";
            } else if (error == error2) {
              window.location.href = "exinvalid.html";
            } else if (error == error3) {
              window.location.href = "exnotfound.html";
            } else if (error == error4) {
              window.location.href = "exnotfound.html";
            } else if (error == error5) {
              window.location.href = "exterpakai.html";
            } else if (error == error6) {
              window.location.href = "exterpakai.html";
            } else if (error == error7) {
              window.location.href = "exbrowser.html";
            } else if (error == error8) {
              window.location.href = "exinvalid.html";
            } else if (error == error9) {
              window.location.href = "exmac.html";
            } else if (error == error10) {
              window.location.href = "exterpakai.html";
            } else if (error == error11) {
              window.location.href = "exkuota.html";
            } else if (error == error12) {
              window.location.href = "expired.html";
            } else if (error == error13) {
              window.location.href = "excalling.html";
            } else {
              document.write("$(error)");
            }
          </script>
        </div>
        $(endif)    

        <p style="text-align: center; font-weight: 400; color:#777878; font-size:11px; margin-top:14px;">Silahkan login dengan <b>kode voucher</b> agar dapat <br>menikmati layanan internet cepat & stabil</p>


        <button type="button" class="btn btn-lg tombol-29 hijaumuda" style="font-size:12px !important;">KODE VOUCHER</button>
        <button onclick="window.location='https://laksa19.github.io/myqr';" type="button" class="btn btn-lg tombol-29 hijaumuda" style="font-size:12px !important;">SCAN QR CODE</button>

        <!--form login-->
        <form name="login" action="$(link-login-only)" method="post" $(if chap-id) onSubmit="return doLogin()" $(endif)>
          <input type="hidden" name="dst" value="$(link-orig)" />
          <input type="hidden" name="popup" value="true" />


      
                 <input type="text" class="form-control kolom-input" name="username" placeholder="USERNAME" value="$(username)"
                  required="required" autocomplete="off" style="margin-top:10px;"/>
            

        
                <input type="text" class="form-control kolom-input" name="password" placeholder="PASSWORD" required="required"
                  autocomplete="off" /> 
<!-- 
                  <div class="form-group">
                    <div class="input-group">
                      <span class="input-group-addon" style="background-color:transparent; border:none;"><i class="glyphicon glyphicon-user" aria-hidden="true" style="color:#000; background-color:#fff; border:2px solid #000; padding:3px; border-radius:40px;"></i></span>
                      <input type="text" class="form-control kolom-input" name="username" placeholder="USERNAME" value="$(username)"
                      required="required" autocomplete="off" />
                  </div>
                </div>
      
                <div class="form-group">
                <div class="input-group">
                  <span class="input-group-addon" style="background-color:transparent; border:none;"><i class="glyphicon glyphicon-lock" aria-hidden="true" style="color:#000; background-color:#fff; border:2px solid #000; padding:3px; border-radius:40px;"></i></span>
                  <input type="text" class="form-control  kolom-input" name="password" placeholder="PASSWORD" required="required"
                  autocomplete="off" />		
              </div>
            </div>
            -->


                  <p style="margin-top:-5px;"></p>
     
  <!-- $(if logged-in == 'yes')
          <button type="button" class="btn btn-lg tombol-29 abutua disabled" style="font-size:12px !important;">
           LIMITED</button>
          $(else)
          $(if trial == 'yes')
          <a href="$(link-login-only)?dst=$(link-orig-esc)&amp;username=T-$(mac-esc)" data-toggle="tooltip"
            data-placement="top">
            <button type="button" class="btn btn-lg tombol-29 hijaumuda" style="font-size:12px !important;">FREE</button></a>
          $(else)
          <button style="font-size:12px !important;" type="button" class="btn btn-lg abutua tombol-29 disabled" data-toggle="popover" data-placement="top"
            data-content="Server Offline">LIMITED</button>
          $(endif)
          $(endif)    -->
    

       <center><button style="font-size:12px !important;" type="submit" class="btn btn-lg tombol-29 merah">LOGIN</button></center>
        </form>
        <!--form login-->



        <div class="sedang">
          <font color="#3A3A3C"><b></b><b></b></font>
        </div>

     <hr style="margin-bottom:3px; margin-top:3px;">
        
        <p style="font-size:85%;  font-weight:800; text-align: center; "><font color="#2F8F01">GUNAKAN INTERNET DENGAN BIJAK!</font></p>
        <hr style="margin-top:-6px;">

        <!--slide teks open-->
<!--
        <hr style="margin-bottom:1px; margin-top:10px;">
        <div class="sedang">
          <script>
            $('.carousel').carousel({
                interval: 3000
              })
            </script>

          <div id="carousel-example-generic1" class="carousel slide" data-ride="carousel" data-interval="3000">
         
            <ol class="carousel-indicators">
              <li data-target="#carousel-example-generic1" data-slide-to="0" class="active" style="background:transparent; border:none;"></li>
              <li data-target="#carousel-example-generic1" data-slide-to="1" style="background:transparent; border:none;"></li>
              <li data-target="#carousel-example-generic1" data-slide-to="2" style="background:transparent; border:none;"></li>


            </ol>

         
            <div class="carousel-inner">

              <div class="item active ">
                <b>Silahkan <b>Beli Voucher Wifi</b><br>Agar dapat terhubung internet
                </b>
              </div>



            

            </div>

          </div> 

        </div>
        <hr style="margin-top:3px; margin-bottom:5px;">

       
      -->



        <!--kiri close-->
      </div>

      <div class="hidden-sm hidden-lg hidden-md" style="margin-top:-20px;"></div>
      <div class="col-md-8 col-sm-12" style="padding:0px;">

        <script>
          $('.carousel').carousel({
              interval: 4000
            })
          </script>

        <div id="carousel-example-generic" class="carousel slide" data-ride="carousel" data-interval="4000">
          <!-- Indicators -->
          <ol class="carousel-indicators">
            <li data-target="#carousel-example-generic" data-slide-to="0" class="active" style="background:transparent; border:none;"></li>
            <li data-target="#carousel-example-generic" data-slide-to="1" style="background:transparent; border:none;"></li>
            <li data-target="#carousel-example-generic" data-slide-to="2" style="background:transparent; border:none;"></li>
            <li data-target="#carousel-example-generic" data-slide-to="3" style="background:transparent; border:none;"></li>

          </ol>

          <!-- Wrapper for slides -->
          <div class="carousel-inner">
            <div class="item active">
              <img src="img/banner1.jpg" alt="...">
            </div>

          

          </div>

          <!-- Controls -->
          <a class="left carousel-control" href="#carousel-example-generic" role="button" data-slide="prev" style="background:transparent;">

          </a>
          <a class="right carousel-control" href="#carousel-example-generic" role="button" data-slide="next" style="background:transparent;">

          </a>
        </div> <!-- Carousel -->

  <!--marquue-->
  <div style="font-size:11px;">
    <marquee scrollamount="3" >
<b><font color="#5f5f5f"><i>Agar dapat tersambung ke jaringan internet, silahkan login menggunakan kode voucher yang sudah anda miliki. agar tetap terhubung ke jarinngan internet</i></font></b>
    </marquee>
  </div>
  <!--marquue-->

      </div>



    </div>
  </div>
  <!--konten close-->

  <div class="col-sm-6 col-sm-offset-3 copyright-teks ">
    <span class='credit-link'>&copy; $(identity) </span>
</div> 

  <script src="js/jquery.js"></script>
  <script src="js/bootstrap.min.js"></script>
  <script src="js/modal.js"></script>


  $(if chap-id)
  <form name="sendin" action="$(link-login-only)" method="post">
    <input type="hidden" name="username" />
    <input type="hidden" name="password" />
    <input type="hidden" name="dst" value="$(link-orig)" />
    <input type="hidden" name="popup" value="true" />
  </form>
  <script type="text/javascript" src="md5.js"></script>

  <script type="text/javascript">
    function doLogin() {
      document.sendin.username.value = document.login.username.value;
      document.sendin.password.value = hexMD5('$(chap-id)' + document.login.password.value + '$(chap-challenge)');
      document.sendin.submit();
      return false;
    }
  </script>
  $(endif)

  <style>
    .blink {
      animation: blink-animation 1s steps(5, start) infinite;
      -webkit-animation: blink-animation 1s steps(5, start) infinite;
    }

    @keyframes blink-animation {
      to {
        visibility: hidden;
      }
    }

    @-webkit-keyframes blink-animation {
      to {
        visibility: hidden;
      }
    }
  </style>




</body>

</html>
