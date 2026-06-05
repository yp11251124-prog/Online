<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Online Store</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:#f4f7fb;
}

header{
    background:#2563eb;
    color:white;
    padding:15px;
    text-align:center;
}

.container{
    width:90%;
    max-width:1200px;
    margin:auto;
    padding:20px;
}

.card{
    background:white;
    padding:20px;
    border-radius:12px;
    box-shadow:0 2px 10px rgba(0,0,0,.1);
    margin-bottom:20px;
}

h2{
    margin-bottom:15px;
    color:#1e3a8a;
}

.products{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
}

.product{
    background:white;
    padding:15px;
    border-radius:12px;
    text-align:center;
    box-shadow:0 2px 8px rgba(0,0,0,.1);
}

.product img{
    width:100%;
    height:180px;
    object-fit:cover;
    border-radius:10px;
}

.price{
    color:green;
    font-size:20px;
    font-weight:bold;
    margin-top:10px;
}

input, textarea, select{
    width:100%;
    padding:10px;
    margin-top:10px;
    border:1px solid #ccc;
    border-radius:8px;
}

button{
    background:#2563eb;
    color:white;
    border:none;
    padding:10px 20px;
    margin-top:10px;
    border-radius:8px;
    cursor:pointer;
}

button:hover{
    background:#1d4ed8;
}

.flex{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:20px;
}

@media(max-width:768px){
    .flex{
        grid-template-columns:1fr;
    }
}

.order-item{
    background:#eef2ff;
    padding:12px;
    margin-bottom:10px;
    border-radius:10px;
}

.user-info{
    color:green;
    font-weight:bold;
    margin-bottom:10px;
}
</style>
</head>
<body>

<header>
    <h1>🛒 My Online Store</h1>
</header>

<div class="container">

    <!-- HOME -->
    <div class="card">
        <h2>Welcome</h2>
        <p>
            Browse products freely. Login is required before placing an order.
        </p>
    </div>

    <!-- PRODUCTS -->
    <div class="card">
        <h2>Products</h2>

        <div class="products">

            <div class="product">
                <img src="https://picsum.photos/300/200?1">
                <h3>Laptop</h3>
                <div class="price">$800</div>
            </div>

            <div class="product">
                <img src="https://picsum.photos/300/200?2">
                <h3>Smartphone</h3>
                <div class="price">$500</div>
            </div>

            <div class="product">
                <img src="https://picsum.photos/300/200?3">
                <h3>Headphones</h3>
                <div class="price">$120</div>
            </div>

            <div class="product">
                <img src="https://picsum.photos/300/200?4">
                <h3>Smart Watch</h3>
                <div class="price">$250</div>
            </div>

        </div>
    </div>

    <div class="flex">

        <!-- SIGNUP -->
        <div class="card">
            <h2>Signup</h2>

            <input type="email" id="signupEmail" placeholder="Email">
            <input type="password" id="signupPassword" placeholder="Password">

            <button onclick="signup()">Create Account</button>
        </div>

        <!-- LOGIN -->
        <div class="card">
            <h2>Login</h2>

            <input type="email" id="loginEmail" placeholder="Email">
            <input type="password" id="loginPassword" placeholder="Password">

            <button onclick="login()">Login</button>

            <button onclick="logout()">Logout</button>

            <div id="userInfo" class="user-info"></div>
        </div>

    </div>

    <!-- ORDER FORM -->
    <div class="card">
        <h2>Place Order</h2>

        <input type="text" id="customerName" placeholder="Customer Name">

        <select id="productName">
            <option value="Laptop">Laptop - $800</option>
            <option value="Smartphone">Smartphone - $500</option>
            <option value="Headphones">Headphones - $120</option>
            <option value="Smart Watch">Smart Watch - $250</option>
        </select>

        <input type="number" id="quantity" placeholder="Quantity">

        <input type="number" id="price" placeholder="Price">

        <textarea id="message" placeholder="Message"></textarea>

        <button onclick="placeOrder()">Submit Order</button>
    </div>

    <!-- ORDER HISTORY -->
    <div class="card">
        <h2>My Order History</h2>

        <div id="ordersContainer">
            Login to view your orders.
        </div>
    </div>

</div>

<script type="module">

import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js";

import {
    getAuth,
    createUserWithEmailAndPassword,
    signInWithEmailAndPassword,
    signOut,
    onAuthStateChanged
}
from "https://www.gstatic.com/firebasejs/10.12.2/firebase-auth.js";

import {
    getFirestore,
    collection,
    addDoc,
    query,
    where,
    getDocs,
    orderBy
}
from "https://www.gstatic.com/firebasejs/10.12.2/firebase-firestore.js";


// REPLACE WITH YOUR FIREBASE CONFIG
const firebaseConfig = {
  apiKey: "AIzaSyD74VC9v4BFXG-tIjd-e3THLxf0VVosuOg",
  authDomain: "onlinestore-ed0c2.firebaseapp.com",
  projectId: "onlinestore-ed0c2",
  storageBucket: "onlinestore-ed0c2.firebasestorage.app",
  messagingSenderId: "212680419196",
  appId: "1:212680419196:web:eb66965b2f13b9f5f5e6f9",
  measurementId: "G-DG50QFEPC4"
};

const app = initializeApp(firebaseConfig);

const auth = getAuth(app);
const db = getFirestore(app);

let currentUser = null;


// SIGNUP
window.signup = async () => {

    const email = document.getElementById("signupEmail").value;
    const password = document.getElementById("signupPassword").value;

    try{

        await createUserWithEmailAndPassword(
            auth,
            email,
            password
        );

        alert("Signup Successful");

    }catch(error){
        alert(error.message);
    }
};


// LOGIN
window.login = async () => {

    const email = document.getElementById("loginEmail").value;
    const password = document.getElementById("loginPassword").value;

    try{

        await signInWithEmailAndPassword(
            auth,
            email,
            password
        );

        alert("Login Successful");

    }catch(error){
        alert(error.message);
    }
};


// LOGOUT
window.logout = async () => {

    await signOut(auth);

    alert("Logged Out");
};


// AUTH STATE
onAuthStateChanged(auth, async(user)=>{

    currentUser = user;

    if(user){

        document.getElementById("userInfo").innerHTML =
        "Logged in as: " + user.email;

        loadOrders();

    }else{

        document.getElementById("userInfo").innerHTML =
        "Not Logged In";

        document.getElementById("ordersContainer").innerHTML =
        "Login to view your orders.";
    }
});


// PLACE ORDER
window.placeOrder = async () => {

    if(!currentUser){
        alert("Please login first.");
        return;
    }

    const customerName =
        document.getElementById("customerName").value;

    const productName =
        document.getElementById("productName").value;

    const quantity =
        document.getElementById("quantity").value;

    const price =
        document.getElementById("price").value;

    const message =
        document.getElementById("message").value;

    try{

        await addDoc(
            collection(db,"orders"),
            {
                userId: currentUser.uid,
                userEmail: currentUser.email,
                customerName,
                productName,
                quantity: Number(quantity),
                price: Number(price),
                message,
                orderDate: new Date().toISOString()
            }
        );

        alert("Order Saved Successfully");

        loadOrders();

    }catch(error){

        alert(error.message);
    }
};


// LOAD USER ORDERS
async function loadOrders(){

    if(!currentUser) return;

    const container =
        document.getElementById("ordersContainer");

    container.innerHTML = "Loading...";

    try{

        const q = query(
            collection(db,"orders"),
            where("userId","==",currentUser.uid),
            orderBy("orderDate","desc")
        );

        const snapshot = await getDocs(q);

        let html = "";

        snapshot.forEach(doc => {

            const order = doc.data();

            html += `
            <div class="order-item">
                <b>Customer:</b> ${order.customerName}<br>
                <b>Product:</b> ${order.productName}<br>
                <b>Quantity:</b> ${order.quantity}<br>
                <b>Price:</b> $${order.price}<br>
                <b>Message:</b> ${order.message}<br>
                <b>Date:</b> ${order.orderDate}
            </div>
            `;
        });

        if(html === ""){
            html = "No orders found.";
        }

        container.innerHTML = html;

    }catch(error){

        container.innerHTML =
        "Error loading orders.";
    }
}

</script>

</body>
</html>
