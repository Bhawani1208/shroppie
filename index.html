/*
FILE: app.js
ROLE: Application logic
CONNECTED TO: index.html via <script src="app.js">
*/

// ===== App State =====
let vendors = [];
let products = [];
let cart = [];
let currentVendor = null;

// ===== DOM Elements =====
const vendorMsg = document.getElementById("vendorMsg");
const productSection = document.getElementById("productSection");
const productList = document.getElementById("productList");
const checkoutSection = document.getElementById("checkout");
const checkoutItems = document.getElementById("checkoutItems");
const totalPriceEl = document.getElementById("totalPrice");
const paymentMsg = document.getElementById("paymentMsg");

// ===== Vendor Registration =====
document.getElementById("registerVendorBtn").onclick = () => {
  const name = vendorName.value.trim();
  const email = vendorEmail.value.trim();
  const plan = vendorPlan.value;

  if (!name || !email || !plan) {
    vendorMsg.innerText = "❌ Fill all fields";
    return;
  }

  currentVendor = { name, email, plan };
  vendors.push(currentVendor);

  vendorMsg.innerText = "✅ Vendor registered (payment step later)";
  productSection.classList.remove("hidden");
};

// ===== Add Product =====
document.getElementById("addProductBtn").onclick = () => {
  const name = productName.value.trim();
  const price = Number(productPrice.value);

  if (!name || price <= 0) return;

  products.push({
    name,
    price,
    vendor: currentVendor.name
  });

  renderProducts();
  productName.value = "";
  productPrice.value = "";
};

// ===== Render Products =====
function renderProducts() {
  productList.innerHTML = "";

  products.forEach((p, i) => {
    productList.innerHTML += `
      <div class="card">
        <span class="badge">FREE AD</span>
        <h3>${p.name}</h3>
        <p>Sold by ${p.vendor}</p>
        <strong>$${p.price}</strong><br><br>
        <button onclick="addToCart(${i})">Add to Cart</button>
      </div>
    `;
  });
}

window.addToCart = (index) => {
  cart.push(products[index]);
  loadCheckout();
};

// ===== Checkout =====
function loadCheckout() {
  checkoutSection.classList.remove("hidden");
  checkoutItems.innerHTML = "";
  let total = 0;

  cart.forEach(item => {
    checkoutItems.innerHTML += `<li>${item.name} – $${item.price}</li>`;
    total += item.price;
  });

  totalPriceEl.innerText = total.toFixed(2);
}

document.getElementById("payBtn").onclick = () => {
  paymentMsg.innerText = "✅ Payment successful (real Stripe later)";
  cart = [];
};
