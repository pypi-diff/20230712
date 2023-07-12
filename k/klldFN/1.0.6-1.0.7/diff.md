# Comparing `tmp/klldFN-1.0.6.tar.gz` & `tmp/klldFN-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klldFN-1.0.6.tar", last modified: Mon May 22 09:50:35 2023, max compression
+gzip compressed data, was "klldFN-1.0.7.tar", last modified: Wed Jul 12 17:45:24 2023, max compression
```

## Comparing `klldFN-1.0.6.tar` & `klldFN-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 09:50:35.815198 klldFN-1.0.6/
--rw-r--r--   0 runner    (1000) runner    (1000)     1135 2023-05-22 09:50:35.815198 klldFN-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      670 2023-03-23 09:54:58.000000 klldFN-1.0.6/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 09:50:35.811198 klldFN-1.0.6/klldFN/
--rw-r--r--   0 runner    (1000) runner    (1000)    67131 2023-05-21 19:02:20.000000 klldFN-1.0.6/klldFN/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-05-22 09:50:35.811198 klldFN-1.0.6/klldFN.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1135 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      127 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-05-22 09:50:35.000000 klldFN-1.0.6/klldFN.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      393 2023-02-19 12:22:33.000000 klldFN-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-05-22 09:50:35.815198 klldFN-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      810 2023-05-19 14:02:19.000000 klldFN-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 17:45:24.297060 klldFN-1.0.7/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2023-07-12 17:45:24.297060 klldFN-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)       47 2023-07-12 17:45:01.000000 klldFN-1.0.7/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 17:45:24.297060 klldFN-1.0.7/klldFN/
+-rw-r--r--   0 runner    (1000) runner    (1000)    69939 2023-07-12 16:03:19.000000 klldFN-1.0.7/klldFN/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-12 17:45:24.297060 klldFN-1.0.7/klldFN.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      351 2023-07-12 17:45:24.000000 klldFN-1.0.7/klldFN.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-07-12 17:45:24.000000 klldFN-1.0.7/klldFN.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-12 17:45:24.000000 klldFN-1.0.7/klldFN.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      127 2023-07-12 17:45:24.000000 klldFN-1.0.7/klldFN.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        7 2023-07-12 17:45:24.000000 klldFN-1.0.7/klldFN.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      471 2022-10-20 21:31:04.000000 klldFN-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-12 17:45:24.297060 klldFN-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      809 2023-07-11 22:44:07.000000 klldFN-1.0.7/setup.py
```

### Comparing `klldFN-1.0.6/klldFN/__init__.py` & `klldFN-1.0.7/klldFN/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 except ModuleNotFoundError as e:
     print(f'Error: {e}\nAttempting to install packages now.')
 
     for module in (
         'pytz',
         'crayons',
         'PirxcyPinger',
-        'fortnitepy==3.6.7',
         'BenBotAsync',
         'FortniteAPIAsync',
         'sanic==20.6.3',
         'aiohttp',
         'requests'
     ):
         subprocess.check_call([sys.executable, "-m", "pip", "install", module])
@@ -136,90 +135,112 @@
             {
                 "status": "online"
             }
         )
 
     return sanic.response.html(
         """
-<!DOCTYPE html>
-<html lang="en">
-<head>
-	<meta charset="UTF-8">
-	<meta name="viewport" content="width=device-width, initial-scale=1.0">
+<html lang="en"><head>
 
-	<!-- Boxicons -->
-	<link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
 
-
-	<!-- My CSS -->
 <link href='https://unpkg.com/boxicons@2.1.1/css/boxicons.min.css' rel='stylesheet'>
-    <link href="https://cdn.klld.42web.io/dashfiles?path=css/sb-admin-2.min.css" type="text/css" rel="stylesheet">
 
-<link rel="stylesheet" href="https://unicons.iconscout.com/release/v4.0.0/css/line.css">
-  
-  <link href="https://raw.githubusercontent.com/nohello-net/site/main/src/css/styles.css" type="text/css" rel="stylesheet">
+<link rel="stylesheet" href="https://html.klldtop.repl.co/style.css">
+<link rel="stylesheet" href="https://html.klldtop.repl.co/s.css">
+<link rel="stylesheet" href="https://navbar-with-mega-dropdown-menu-1.4klld.repl.co/style.css">
+
+    
+        <meta charset="utf-8">
+        <meta http-equiv="X-UA-Compatible" content="IE=edge">
+        <title>klldFN | """ + f""" {name} """ + """</title>
+        <meta name="description" content="klldFN">
+        <meta name="keywords" content="">
+        <meta name="author" content="klldFN Developing Team">
+        <link rel="icon" type="image/png" href="../favicon.png">
+        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
+        <!-- START: Styles -->
+        <!-- Adobe Fonts -->
+        <link href="https://fonts.googleapis.com/css2?family=Markazi+Text&amp;display=swap" rel="stylesheet">
+        <!-- Bootstrap -->
   
-  <link href="https://cdn.klld.42web.io/dashfiles?path=vendor/fontawesome-free/css/all.min.css" rel=stylesheet type=text/css>
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/bootstrap.min.css">
+        <!-- Swiper -->
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/swiper-bundle.min.css">
+        <!-- Fancybox -->
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/jquery.fancybox.min.css">
+        <!-- Revolution Slider -->
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/settings.css">
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/layers.css">
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/navigation.css">
+        <!-- MonsterPlay -->
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/respect.css">
+      
+        <!-- Custom Styles -->
+        <link rel="stylesheet" href="https://html.klldtop.repl.co/public/css/custom.css">
+        <!-- END: Styles -->
+        <!-- jQuery -->
+        <script src="https://html.klldtop.repl.co/public/js/jquery.min.js"></script>
+        <!-- Preloader -->
+        <script src="https://html.klldtop.repl.co/public/js/preloader.min.js"></script>
+    </head>
+    <body>
+        <!-- Preloader -->
+        <div class="mpl-preloader">
+            <div class="mpl-preloader-content">
+                <div class="mpl-preloader-title display-1 h1">klldFN | """ + f""" {name} """ + """</div>
+                <div class="mpl-preloader-progress">
+                    <div></div>
+                </div>
+            </div>
+        </div>
+        <div class="mpl-preloader-bg"></div>
+        <!-- /Preloader -->
+        <div class="content-wrap">
+            <div class="mpl-navbar-mobile-overlay"></div>
 
-<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/tiny-slider.css" rel="stylesheet">
-<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/Cookies.css" rel="stylesheet">
-<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/Click.css" rel="stylesheet">
-<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/tobii.min.css" rel="stylesheet">
-<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/style.min.css" class="theme-opt" rel="stylesheet" type="text/css" />
-<link href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/style.css" class="theme-opt" rel="stylesheet" type="text/css" />
 
-  <link rel="stylesheet" href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/style1.css">
+        <!-- /Preloader -->
   
-	<link rel="stylesheet" href="https://klld.repl.co/style.css">
-	<link rel="stylesheet" href="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/adminhub.css">
 
-	<title>klldFN</title>
-<meta name="viewport" content="width=device-width, initial-scale=1.0">
-<meta name="description" content="">
-<meta name="keywords" content="klld">
-<meta name="author" content="klld">
-<meta name="email" content="klld@email.com">
-<meta name="website" content="https://www.klld.42web.io/">
-<meta name="Version" content="v1.0.6">
-<link rel="shortcut icon" href="https://www.authcode.tk/klld.png">
-</head>
-<body>
 
-<nav>
-		<div class="container">
-			<div class="nav__wrapper">
-				<a href="#" class="nav__brand">
-					<span class="nav__logo">FN</span>
-					<span class="nav__logo__name">klld</span>
-				</a>
-				<div class="nav__list__wrapper">
-					<div class="nav__list">
-						<div class="nav__menu">
-							<a href="https://www.klld.42web.io/" class="nav__menu__item">Home</a>
 
-						<div class="nav__menu">
-							<a href="https://discord.gg/ybr7evg4q5" class="bx bxl-discord btn btn-blue">discord</a>
-						</div>
-						</div>
-					</div>
-				</div>
-				<i class='bx bx-menu nav__toggle'></i>
-			</div>
-		</div>
-	</nav>
 
+ <section class="section mt-60" style="height: auto !important;">
+        <div class="container mt-lg-3" style="height: auto !important;">
+            <div class="row" style="height: auto !important;">
+                <div class="col-lg-12 col-12" style="height: auto !important;">
+                    <div class="row align-items-center mt-4" style="height: auto !important;">
+                        <div class="col">
+                            <ul class="nav nav-tabs overflow-x">
+
+                                <li class="nav-item">
+                                    <a href="public-helpers.html" class="nav-link active">
+                                        <i class="uil uil-cog align-middle"></i> Dashboard
+                                    </a>
+                                </li>
+                                <li class="nav-item">
+                                    <a href="https://www.klld.000.pe/" class="nav-link">
+                                        <i class="uil uil-robot"></i> website
+                                    </a>
+                                </li>
+                                
+                            </ul>
+                        </div><div class="google-auto-placed" style="width: 100%; height: auto !important; clear: both; text-align: center;"></div>
+                    </div>
 
-<header>
-		<div class="container">
-			<div class="header__wrapper">
-				<div class="header__content">
-	<section id="testimonial">
-		<div class="container">
-			<h4 class="header__title">klldFN</h4>
-			<div class="testimonial__list">
+                    
+                        <div class="card-body">
+                            <div class="border-bottom pb-4">
+                                
+                            </div>
+ <div id="lobby-helpers-div" class="row">
+        
+            
+                          
+                            <div class="testimonial__list">
 				<div class="testimonial__item">
 					
 
 					<div class="testimonial__item__user">
 		<img src="https://www.just.edu.jo/Units_and_offices/Offices/IRO/PublishingImages/Pages/Mobility%20Calls/MobilityCalls/green2.gif" alt="">
 						<div class="testimonial__item__user__profile">
 							<h4>Online now</h4>
@@ -262,40 +283,18 @@
                 <div class="testimonial__list">
 				<div class="testimonial__item">
 
 									<div class="testimonial__item__user">
 						
 						<div class="testimonial__item__user__profile">
 							<h4>Friends</h4>
-              <h>""" + f"""{friendlist} """ + """ / 9500</h>
+              <h>""" + f"""{friendlist} """ + """ / 9999</h>
               </div>
 					</div>
 				</div>
-
-
-
-
-              
-              
-              
-                </div>
-					    </div> 
-						</div>
-					</div>
-				</div>
-			</div>
-		</div>
-	</section>
-
-
-
-
-<section id="testimonial">
-		<div class="container">
-
                 <div class="testimonial__list">
 				<div class="testimonial__item">
 <div class="testimonial__item__user">
 <img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{skin}""" + """/smallicon.png" alt="">
 						<div class="testimonial__item__user__profile">
 
 							<h4>Outfit</h4>
@@ -324,77 +323,86 @@
 <img src="https://fortnite-api.com/images/cosmetics/br/""" + f"""{pickaxe}""" + """/smallicon.png" alt="">	
 						<div class="testimonial__item__user__profile">
 							<h4>Pickaxe</h4>
              <h>""" + f"""{pickaxe} """ + """</h>
 
 						</div>
 					</div>
-				</div>
+				</div></div>
 
-
-
-
-
-
-              
-              
-              
+                            
+                                </div>
+                            </div>
+                        </div>
+                    </div>
                 </div>
-					    </div> 
-						</div>
-					</div>
-				</div>
-			</div>
-		</div>
-	</section>
-	<!-- HEADER -->
-
-	<!-- ABOUT -->
-
-
-
-	<!-- TESTIMONIAL -->
-	<section id="testimonial">
+            </div>
+        </div>
+    </section>    
+
+          <!-- Footer -->
+       
+	<footer>
 		<div class="container">
-			<h2 class="section__title">Developer</h2>
-			
-			<div class="testimonial__list">
-				<div class="testimonial__item">
+			<div class="footer__wrapper">
+				<a href="#" class="footer__brand">
 					
-
-					<div class="testimonial__item__user">
-						<img src="https://www.authcode.tk/klld.png" alt="">
-						<div class="testimonial__item__user__profile">
-							<h4>klld</h4>
-							<p>Owner</p>
-						</div>
-					</div>
-				</div>
-				
-						</div>
-					</div>
+					<span class="footer__logo__name">klldFN</span>
+				</a>
+				<p>Copyright &copy;2023 All Right Reserved</p>
+				<div class="footer__social__link">
+					<a href="https://www.youtube.com/@klld" class="footer__link"><i class='bx bxl-youtube'></i></a>
+					<a href="https://www.tiktok.com/@4.klld" class="footer__link"><i class='bx bxl-tiktok' ></i></a>
+					<a href="https://discord.gg/aUX5dupzdh" class="footer__link"><i class='bx bxl-discord' ></i></a>
 				</div>
 			</div>
 		</div>
-    <ul class="circles p-0 mb-0">
-<li></li><li></li><li></li><li></li><li></li><li></li><li></li><li></li><li></li><li></li>
-</ul>
-	</section>
-
-  
-	
-	<!-- CONTENT -->
-	
- <script src="https://dashboard-panel.klld.repl.co/script.js"></script>
-  <script src="https://04e5b1ec-2c32-4b1a-b5a0-ccf6bb46f16e.id.repl.co/css/script.js"></script>
-<script src="https://klld.repl.co/script.js"></script>
-<script src="https://cdn.klld.42web.io/dashfiles?path=vendor/jquery/jquery.min.js"></script><script src="https://cdn.klld.42web.io/dashfiles?path=vendor/bootstrap/js/bootstrap.bundle.min.js"></script><script src="https://cdn.klld.42web.io/dashfiles?path=vendor/jquery-easing/jquery.easing.min.js"></script><script src="https://cdn.klld.42web.io/dashfiles?path=vendor/chart.js/Chart.min.js">
-
-</body>
-</html>
+	</footer>
+     
+        <!-- START: Scripts -->
+        <!-- Popper -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/@popperjs/core/dist/umd/popper.min.js?v=2.11.0"></script>
+        <!-- ScrollReveal -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/scrollreveal/dist/scrollreveal.min.js?v=4.0.9"></script>
+        <!-- Animejs -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/animejs/lib/anime.min.js?v=3.2.1"></script>
+        <!-- Bootstrap -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/bootstrap/dist/js/bootstrap.min.js?v=5.1.3"></script>
+        <!-- Jarallax -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/jarallax/dist/jarallax.min.js?v=1.12.8"></script>
+        <!-- Swiper -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/swiper/swiper-bundle.min.js?v=6.8.2"></script>
+        <!-- Fancybox -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/fancybox/dist/jquery.fancybox.min.js?v=3.5.7"></script>
+        <!-- jQuery Countdown -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/jquery-countdown/dist/jquery.countdown.min.js?v=2.2.0"></script>
+        <!-- Moment.js -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/moment/min/moment.min.js?v=2.29.1"></script>
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/moment-timezone/builds/moment-timezone-with-data.min.js?v=0.5.34"></script>
+        <!-- Revolution Slider -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/slider-revolution/js/jquery.themepunch.tools.min.js?v=5.4.8"></script>
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/slider-revolution/js/jquery.themepunch.revolution.min.js?v=5.4.8"></script>
+        <!-- ImagesLoaded -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/imagesloaded/imagesloaded.pkgd.min.js?v=4.1.4"></script>
+        <!-- Isotope -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/isotope-layout/dist/isotope.pkgd.min.js?v=3.0.6"></script>
+        <!-- Ion Range Slider -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/ion-rangeslider/js/ion.rangeSlider.min.js?v=2.3.1"></script>
+        <!-- Bootstrap TouchSpin -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/bootstrap-touchspin/dist/jquery.bootstrap-touchspin.min.js?v=4.3.0"></script>
+        <!-- Bootstrap Validator -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/vendor/bootstrap-validator/dist/validator.min.js?v=0.11.9"></script>
+        <!-- MonsterPlay -->
+        <script src="https://respectcfw.com/RTWEB/public/assets/js/monsterplay.min.js?v=1.2.0"></script>
+        <script src="https://respectcfw.com/RTWEB/public/assets/js/monsterplay-init.js?v=1.2.0"></script>
+              <script src="https://cdn2.klld.cloudns.nz/script.js"></script>
+          <script src="https://navbar-with-mega-dropdown-menu.4klld.repl.co/script.js"></script>
+        <!-- END: Scripts -->
+    
+</div></div><div class="mpl-cursor" style="transform: matrix(1, 0, 0, 1, -100, -100) translate3d(0px, 0px, 0px);"></div><div class="mpl-cursor-outer" style="transform: matrix(1, 0, 0, 1, -100, -100) translate3d(0px, 0px, 0px);"></div></body></html>
         """
     )
 
 
 @sanic_app.route("/default")
 async def index(request):
     return sanic.response.json(
@@ -1063,15 +1071,15 @@
     async def event_party_message(self, message: fortnitepy.FriendMessage) -> None:
         if not self.has_friend(message.author.id):
             try:
                 await self.add_friend(message.author.id)
             except: pass    
 
     async def event_friend_message(self, message: fortnitepy.FriendMessage) -> None:
-        if not message.author.display_name != "ʏᴏᴜᴛᴜʙᴇ ᴋʟʟᴅ":
+        if not message.author.display_name != "klld َََََ":
             await self.party.invite(message.author.id)
 
     async def event_party_message(self, message = None) -> None:
         if self.party.me.leader:
             if message is not None:
                 if message.content in self.bl_msg:
                     if not message.author.display_name in self.adminx:
@@ -1321,33 +1329,15 @@
             cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaPickaxe")
             await self.party.me.set_pickaxe(asset=cosmetic.id)
             await ctx.send(f'Pickaxe set to {cosmetic.name}.')
 
         except FortniteAPIAsync.exceptions.NotFound:
             pass
  
-    @commands.command(aliases=['news'])
-    @commands.cooldown(1, 10)
-    async def new(self, ctx: fortnitepy.ext.commands.Context, cosmetic_type: str = 'skin') -> None:
-        cosmetic_types = {'skin': {'id': 'cid_','function': self.party.me.set_outfit},'backpack': {'id': 'bid_','function': self.party.me.set_backpack},'emote': {'id': 'eid_','function': self.party.me.set_emote},{'CHARACTER': {'id': 'CHARACTER_','function': self.party.me.set_outfit,}
-
-        if cosmetic_type not in cosmetic_types:
-            return await ctx.send('Invalid cosmetic type, valid types include: skin, backpack & emote.')
-
-        new_cosmetics = await self.fortnite_api.cosmetics.get_new_cosmetics()
-
-        for new_cosmetic in [new_id for new_id in new_cosmetics if
-                             new_id.id.lower().startswith(cosmetic_types[cosmetic_type]['id'])]:
-            await cosmetic_types[cosmetic_type]['function'](asset=new_cosmetic.id)
-
-            await ctx.send(f"{cosmetic_type}s set to {new_cosmetic.name}.")
-
-            await asyncio.sleep(3)
-
-        await ctx.send(f'Finished equipping all new unencrypted {cosmetic_type}s.')      
+    
  
     @commands.command()
     async def purpleskull(self, ctx: fortnitepy.ext.commands.Context) -> None:
         await self.party.me.set_outfit(asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants(clothing_color=1))
         await ctx.send(f'Skin set to Purple Skull Trooper!')
         
     @commands.command()
@@ -1848,8 +1838,8 @@
         print(f"Removed {friend.id}")
       await ctx.send(
           f"""
 Total Friends Removed: {total}
 Online Friends Removed: {online}
 Offline Friends Removed: {offline} 
           """
-        )
+        )
```

### Comparing `klldFN-1.0.6/setup.py` & `klldFN-1.0.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="klldFN",
-    version="1.0.6",
+    version="1.0.7",
     author="klld",
     description="klldFN",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.klld.42web.io",
     packages=setuptools.find_packages(),
     classifiers=[
@@ -24,8 +24,8 @@
           'BenBotAsync==3.0.1',
           'FortniteAPIAsync==0.1.6',
           'sanic==20.6.3',
           'aiohttp',
           'uvloop',
           'requests'  
       ],
-)
+)
```

