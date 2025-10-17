<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Tinted Nook — Handmade Clay Magnets & Brooches</title>
  <meta name="description" content="Tinted Nook — handmade clay fridge magnets, brooches and custom painted bottles. Contact via WhatsApp for orders."/>
  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;600&family=Amatic+SC:wght@700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg1:#fff7e6;
      --bg2:#fef6ff;
      --accent:#e57c23;
      --muted:#666;
      --card:#fffaf2;
      --radius:12px;
      font-family: "Quicksand", system-ui, -apple-system, "Segoe UI", Roboto, Arial;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      background: linear-gradient(135deg,var(--bg1),var(--bg2));
      color:#222;
      -webkit-font-smoothing:antialiased;
      padding:20px;
      display:flex;
      justify-content:center;
    }
    .wrap{max-width:1100px;width:100%}
    header{
      display:flex;
      gap:18px;
      align-items:center;
      justify-content:space-between;
      padding:14px 18px;
      background:rgba(255,255,255,0.85);
      border-radius:14px;
      box-shadow:0 8px 30px rgba(0,0,0,0.06);
      margin-bottom:18px;
    }
    .brand{display:flex;gap:12px;align-items:center}
    .brand img{width:120px;height:auto;border-radius:8px}
    h1{margin:0;font-family:'Amatic SC',cursive;font-size:26px}
    .contact a{color:var(--accent);text-decoration:none;font-weight:600;margin-left:8px}
    main{display:grid;grid-template-columns:1fr 360px;gap:18px;align-items:start}
    .hero{
      background:linear-gradient(180deg,#ffffffcc,#fff);
      padding:18px;border-radius:12px;
      box-shadow:0 6px 18px rgba(0,0,0,0.04)
    }
    .shop-header{display:flex;align-items:center;justify-content:space-between;gap:12px}
    .shop-header h2{margin:0;font-family:'Amatic SC',cursive;font-size:26px}
    .grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(220px,1fr));gap:16px;margin-top:14px}
    .card{background:var(--card);padding:12px;border-radius:12px;box-shadow:0 4px 12px rgba(0,0,0,0.04);display:flex;flex-direction:column}
    .imgwrap{height:160px;border-radius:10px;overflow:hidden;background:#f7f7f7;display:flex;align-items:center;justify-content:center}
    .imgwrap img{width:100%;height:100%;object-fit:cover}
    .name{font-weight:700;margin:8px 0 4px 0}
    .price{color:var(--accent);font-weight:700}
    .small{font-size:13px;padding:8px;border-radius:8px;border:0;cursor:pointer}
    .cardrow{display:flex;gap:8px;justify-content:flex-end;margin-top:8px}
    .side{
      position:sticky;top:18px;
      display:flex;flex-direction:column;gap:14px;
    }
    .cart{
      background:rgba(255,255,255,0.95);padding:12px;border-radius:12px;box-shadow:0 6px 18px rgba(0,0,0,0.06)
    }
    .cart h3{margin:0 0 8px 0}
    .cart-item{display:flex;gap:10px;align-items:center;padding:8px 0;border-bottom:1px dashed rgba(0,0,0,0.06)}
    .cart-item img{width:54px;height:54px;border-radius:8px;object-fit:cover}
    .qty{display:flex;gap:6px;align-items:center}
    .qty button{padding:6px 8px;border-radius:8px;border:0;background:#eee;cursor:pointer}
    .cart-footer{display:flex;flex-direction:column;gap:8px;padding-top:8px}
    .btn{background:var(--accent);color:#fff;padding:10px 12px;border-radius:10px;border:0;font-weight:600;cursor:pointer}
    .ghost{background:transparent;border:1px solid rgba(0,0,0,0.06);padding:8px;border-radius:8px;cursor:pointer}
    .form-card{background:linear-gradient(180deg,#fff,#fffaf8);padding:12px;border-radius:12px;box-shadow:0 6px 18px rgba(0,0,0,0.04)}
    form label{display:block;margin-top:8px;font-weight:600}
    form input, form textarea {width:100%;padding:8px;border-radius:8px;border:1px solid #ddd;margin-top:6px}
    form input[type="file"]{padding:6px}
    form .small-note{font-size:13px;color:var(--muted);margin-top:6px}
    footer{margin-top:22px;text-align:center;color:var(--muted);font-size:13px;padding-bottom:22px}
    @media (max-width:980px){
      main{grid-template-columns:1fr}
      header{flex-direction:column;gap:10px;align-items:flex-start}
      .brand img{width:100px}
      .side{position:relative;top:auto}
    }
  </style>
</head>
<body>
<div class="wrap">
<header>
  <div class="brand">
    <img src="logo.png" alt="Tinted Nook logo" id="site-logo" />
    <div>
      <h1>Tinted Nook</h1>
      <div style="font-size:14px;color:var(--muted)">Handmade clay magnets, brooches & hand-painted bottles</div>
    </div>
  </div>
  <div class="contact" aria-hidden="false">
    <a href="https://www.instagram.com/tintednook" target="_blank">Instagram</a> |
    <a href="mailto:tintednook@gmail.com">tintednook@gmail.com</a> |
    <a href="https://wa.me/919231923221" target="_blank">WhatsApp</a>
  </div>
</header>

<main>
<div class="hero">
  <div class="shop-header">
    <div>
      <h2>Shop</h2>
      <div style="color:var(--muted)">Browse our handcrafted fridge magnets, brooches & bottles</div>
    </div>
    <div style="align-self:start">
      <button class="ghost" id="view-about">About</button>
      <button class="btn" id="open-cart">Cart (<span id="cart-count">0</span>)</button>
    </div>
  </div>

  <div class="grid" id="products-grid" aria-live="polite"></div>
</div>

<aside class="side">
  <div class="cart" id="cart" style="display:none" aria-hidden="true">
    <h3>Your Cart</h3>
    <div id="cart-items"></div>
    <div class="cart-footer">
      <div style="display:flex;justify-content:space-between"><strong>Total</strong><strong id="cart-total">₹0</strong></div>
      <div style="display:flex;gap:8px">
        <button class="ghost" id="clear-cart">Clear</button>
        <button class="btn" id="checkout">Checkout via WhatsApp</button>
      </div>
    </div>
  </div>

  <div class="form-card">
    <h3>Custom Request / Quote</h3>
    <div class="small-note">Send us reference images and details — we'll reply with a quote.</div>
    <form id="custom-form" action="https://formspree.io/f/yourformid" method="POST" enctype="multipart/form-data">
      <label for="name">Name *</label>
      <input id="name" name="name" required>
      <label for="contact">Contact No *</label>
      <input id="contact" name="contact" required>
      <label for="email">Email *</label>
      <input id="email" name="email" type="email" required>
      <label for="ref">Reference picture (optional)</label>
      <input id="ref" name="reference" type="file" accept="image/*">
      <label for="notes">Special instructions</label>
      <textarea id="notes" name="instructions" rows="3"></textarea>
      <label style="margin-top:8px">
        <input type="checkbox" name="permission" required> I allow Tinted Nook to contact me via WhatsApp or Email.
      </label>
      <button type="submit" class="btn">Request Quote</button>
    </form>
    <div style="margin-top:10px;font-size:13px;color:var(--muted)">
      Or message us directly on WhatsApp.
    </div>
  </div>
</aside>
</main>

<footer>
© 2025 Tinted Nook — handmade with love • Instagram: @tintednook • Email: tintednook@gmail.com
</footer>
</div>

<script>
const PRODUCTS = [
  { id:"fm-owl", name:"Goodluck Owl Fridge Magnet", price:299, short:"Handmade owl magnet", desc:"Cute hand-sculpted owl magnet. Size ~3 x 4 inches.", image:"Goodluck-Owl-FridgeMagnet.JPG", category:"Fridge Magnet" },
  { id:"fm-fairy", name:"Fairy House Fridge Magnet", price:499, short:"Mini fairy house magnet", desc:"Whimsical fairy house magnet.", image:"Fairy-House-FridgeMagnet.JPG", category:"Fridge Magnet" },
  { id:"fm-dream", name:"Mini Dream House Fridge Magnet", price:599, short:"Dream house themed magnet", desc:"Mini clay dream house magnet with delicate details.", image:"Mini-Dream-House-FridgeMagnet.JPG", category:"Fridge Magnet" },
  { id:"fm-chimney", name:"Storybook Style Chimney House Fridge Magnet", price:699, short:"Storybook style house magnet", desc:"Charming storybook-style chimney house magnet.", image:"Storybook-Style-Chimney-House-FridgeMagnet.JPG", category:"Fridge Magnet" }
];

let cart = {};
const WA_NUMBER = "919231923221"; 
function currency(n){ return "₹" + Number(n).toFixed(0); }

function saveCart(){ localStorage.setItem("tn_cart_v1", JSON.stringify(cart)); updateCartUI(); }
function loadCart(){ const r = localStorage.getItem("tn_cart_v1"); cart = r ? JSON.parse(r) : {}; updateCartUI(); }

const grid = document.getElementById("products-grid");
function renderProducts(){
  grid.innerHTML = "";
  for(const p of PRODUCTS){
    const el = document.createElement("article");
    el.className = "card";
    el.innerHTML = `
      <div class="imgwrap"><img loading="lazy" src="${p.image}" alt="${p.name}" onerror="this.style.objectFit='contain'"></div>
      <div style="padding-top:6px">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <div class="name">${p.name}</div>
          <div class="price">${p.price>0?currency(p.price):'Price on request'}</div>
        </div>
        <div style="color:var(--muted);font-size:13px;margin:6px 0">${p.short}</div>
        <div class="cardrow">
          <button class="small" data-id="${p.id}" data-action="view">View</button>
          <button class="small" data-id="${p.id}" data-action="add">Add</button>
          <button class="small" data-id="${p.id}" data-action="w">WhatsApp</button>
        </div>
      </div>
    `;
    grid.appendChild(el);
  }
}

// All other cart & WhatsApp functions remain the same as previous version
renderProducts();
loadCart();
</script>
</body>
</html>
