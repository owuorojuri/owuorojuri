
<html>
    <head>
        <title>super metro</title>
        <link rel="stylesheet" href="dest/output.css">
        <link rel="stylesheet" href="dest/output.css?v=0.0.0.0.0.5">
        <link rel="stylesheet" href="dest/font-awesome.min.css">
        <link rel="stylesheet" href="//fonts.googleapis.com/css?family=Muli:300,400,400i,700,700i|Nunito:400,700,900" media="all">
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
        <link href="dest/Roboto+Condensed.css" rel="stylesheet" type="text/css"/>
        <base href="/" />
        <style>
            [ng\:cloak], [ng-cloak], [data-ng-cloak], [x-ng-cloak], .ng-cloak, .x-ng-cloak {
                display: none !important;
            }
        </style>
    </head>
    <body ng-app="ENAApp" ng-cloak ng-controller="parentController"  ng-csp="no-unsafe-eval" ng-class="{test :continue}" ng-cloak>
    <toast></toast>
   
    <div class="row" style="background-color: #242424;padding-bottom: 20px;">
        <div class="col-lg-5 col-xs-6" style="position:relative;"><img src="assets/big-logo.png" style="width: 80%;position: absolute;top:-25px"></div>
        <div class="col-lg-7 col-xs-6"><img src="assets/amenity.png" style="width: 300px;"></div>
    </div>
    <nav class="navbar navbar-default">
        <div class="container-fluid" style="padding: 0 73px;">
            <div class="navbar-header">
                <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#myNavbar">
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
            </div>
            <div class="collapse navbar-collapse" id="myNavbar">
                <ul class="nav navbar-nav">
                    <li><a ui-sref="home"  class="menu-font">Home</a></li>
                    <li><a ui-sref="about"  class="menu-font">About Us</a></li>
                    <li><a ui-sref="contact"  class="menu-font">Contact Us</a></li>
                    <li><a ui-sref="printticket"  class="menu-font">Print Ticket</a></li>
                    <li><a ui-sref="gallery"  class="menu-font">Gallery</a></li>
                    <li class="menu-font">
                        <a  ng-if="!$root.isLogin" class="color pointer" ng-click="openModal()">Sign In / Register</a></li>
                    <li class="dropdown pointer" ng-if='$root.isLogin'><a class="dropdown-toggle" data-toggle="dropdown"><i class="fa fa-user-circle-o" style="font-size:25px"></i><span class="caret"></span></a>
                        <ul class="dropdown-menu">
                            <li class="padding-top-bottom-2"><a ng-click="goProfile('0')">My Trips</a></li>
                            <li class="padding-top-bottom-2"><a ng-click="goProfile('2')">My Profile</a></li>
                            <li class="padding-top-bottom-2"><a ng-click="goProfile('3')">Change Password</a></li>
                            <li class="padding-top-bottom-2"><a ng-click="goProfile('1')">Wallet</a></li>
                            <li class="padding-top-bottom-2"><a ng-click="signOut()">Sign Out</a></li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
    <div class="container" style="min-height: 430px">
        <ui-view></ui-view>
    </div>

    <footer class="footer">
        <div class="row" style="background-color: #000;padding-top: 12px;padding-bottom: 10px;color:#cbcbcb">
            <div class="col-lg-2">
                Copyright <span class="copyightsymbolcircle" style="margin-right:5px">C</span>{{date| date:'yyyy'}}
            </div>
            <div class="col-lg-6" style="text-align: center">
                <span style="border-right: solid 1px #ddd;padding-right: 5px;font-size:16px"><b><a ui-sref="privacypolicy" style="color:#cbcbcb">Privacy Policy</a></b></span>
                <span style="font-size:16px"><b><a ui-sref="termcondition" style="color:#cbcbcb">Terms & Conditions</a></b></span>
            </div>
            <div class="col-lg-4" style="text-align: right">
                <span style="border-right: solid 1px #ddd;padding-right: 3px"><a ui-sref="home" style="color:#cbcbcb">Home</a></span>
                <span style="border-right: solid 1px #ddd;padding-right: 3px"><a ui-sref="about" style="color:#cbcbcb">About</a></span>
                <span style="border-right: solid 1px #ddd;padding-right: 3px"><a ui-sref="printticket" style="color:#cbcbcb">Print Ticket</a></span>
                <span><a ui-sref="contact" style="color:#cbcbcb">Contact Us</a></span>
            </div>
        </div>
    </footer>
    <!--Start of Tawk.to Script-->

    <script type="text/javascript">

        var Tawk_API = Tawk_API || {}, Tawk_LoadStart = new Date();
        (function(){

        var s1 = document.createElement("script"), s0 = document.getElementsByTagName("script")[0];
        s1.async = true;
        s1.src = 'https://embed.tawk.to/5d52849177aa790be32eaca9/default';
        s1.charset = 'UTF-8';
        s1.setAttribute('crossorigin', '*');
        s0.parentNode.insertBefore(s1, s0);
        })();
    </script>

    <!--End of Tawk.to Script-->
    <script type="text/javascript" src="dest/output.js?v=0.0.0.0.2.0"></script>
    <script src="dest/templates.js?v=0.0.0.0.2.1" type="text/javascript"></script>
    <!--<script src="https://apis.google.com/js/platform.js" async defer></script>-->
</body>
</html>
