<html lang="en">
<head>
  <head>
  <meta charset="UTF-8">
  <title>Simple Toggle Website</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f4f4f4;
    }

    nav {
      background: #333;
      padding: 10px;
      text-align: center;
    }

    nav button {
      background: none;
      color: white;
      border: none;
      margin: 0 10px;
      font-size: 16px;
      cursor: pointer;
    }

    nav button:hover {
      text-decoration: underline;
    }

    .page {
      display: none;
      padding: 40px;
      background: white;
      margin: 20px;
      border-radius: 8px;
    }

    .active {
      display: block;
    }
  </style>
  <!-- Google Tag Manager -->
  <script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
  new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
  j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
  'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
  })(window,document,'script','dataLayer','GTM-KSMH3FPT');</script>
  <!-- End Google Tag Manager -->
</head>
<body>
 <!-- Navigation -->
  <nav>
    <button onclick="showPage('home')">Home</button>
    <button onclick="showPage('about')">About</button>
    <button onclick="showPage('contact')">Contact</button>
  </nav>

  <!-- Pages -->
  <div id="home" class="page active">
    <h1>Welcome</h1>
    <p>This is the Home page.</p>
  </div>

  <div id="about" class="page">
    <h1>About Us</h1>
    <p>This is the About page.</p>
  </div>

  <div id="contact" class="page">
    <h1>Contact</h1>
    <p>Email: hello@example.com</p>
  </div>

  <!-- JavaScript -->
  <script>
    function showPage(pageId) {
      const pages = document.querySelectorAll('.page');
      pages.forEach(page => page.classList.remove('active'));
      document.getElementById(pageId).classList.add('active');
    }
  </script>
  <!-- Google Tag Manager (noscript) -->
  <noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-KSMH3FPT"
  height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
  <!-- End Google Tag Manager (noscript) -->
</body>
