# HTML_Project
# its an demo project to html for an  Restaurant
<!DOCTYPE html>
<head>
    <title>FoodComa</title>
    <link rel="stylesheet" href="Project.css">
</head>
<body>
    
    <header id="s1">
        <h1>FoodComa</h1>
        <h2 id="h2">Welcome to our Restaurant!!!</h2>
        <div class="cart">
            <span id="cart">0</span> Items in cart
               </div>
    </header>
    <p id="y1">Break Fast</p>
    <section class="food-list">
        <div class="cake">
            <img src="t6.jpg" alt="Dosa" class="food-img">
            <h2>Dosa</h2>
            <p>Price: $80</p>
            <button onclick="addToCart(80)">Add to Cart</button>
        </div>
        <div class="cake">
            <img src="t7.jpg" alt="Idli" class="food-img">
            <h2>Idli</h2>
            <p>Price: $75</p>
            <button onclick="addToCart(75)">Add to Cart</button>
        </div>
        <div class="cake">
            <img src="t8.jpg" alt="Chapati" class="food-img">
            <h2>Chapati</h2>
            <p>Price: $85</p>
            <button onclick="addToCart(85)">Add to Cart</button>
        </div>
        <div class="cake">
            <img src="t9.jpg" alt="Puri" class="food-img">
            <h2>Puri</h2>
            <p>Price: $100</p>
            <button onclick="addToCart(100)">Add to Cart</button>
        </div>
</section>
<p id="y1">Yum Yum</p>
    <section class="food-list">
        <div class="cake">
            <img src="t4.jpg" alt="Biriyani" class="food-img">
            <h2>Biriyani</h2>
            <p>Price: $80</p>
            <button onclick="addToCart(80)">Add to Cart</button>
        </div>
        <div class="cake">
            <img src="c.jpg" alt="Chicken Rice" class="food-img">
            <h2>Chicken Rice</h2>
            <p>Price: $75</p>
            <button onclick="addToCart(75)">Add to Cart</button>
        </div>
        <div class="cake">
            <img src="f.jpg" alt="Fish" class="food-img">
            <h2>Fish</h2>
            <p>Price: $85</p>
            <button onclick="addToCart(85)">Add to Cart</button>
        </div>
        <div class="cake">
            <img src="p.jpg" alt="Pizza" class="food-img">
            <h2>Pizza</h2>
            <p>Price: $100</p>
            <button onclick="addToCart(100)">Add to Cart</button>
        </div>
</section>
<p id="y1">Dessert</p>
<section class="food-list2">
    <div class="cake">
        <img src="a1.jpg" alt="Bun Falooda" class="food-img">
        <h2>Bun Falooda</h2>
        <p>Price: $65</p>
        <button onclick="addToCart(65)">Add to Cart</button>
    </div>
    <div class="cake">
        <img src="a2.jpg" alt="Brownie" class="food-img">
        <h2>Brownie</h2>
        <p>Price: $70</p>
        <button onclick="addToCart(70)">Add to Cart</button>
    </div>
    <div class="cake">
        <img src="a3.jpg" alt="ICE Cream" class="food-img">
        <h2>ICE Cream</h2>
        <p>Price: $60</p>
        <button onclick="addToCart(60)">Add to Cart</button>
    </div>
    <div class="cake">
        <img src="t5.jpg" alt="Brownie" class="food-img">
        <h2>Brownie</h2>
        <p>Price: $80</p>
        <button onclick="addToCart(80)">Add to Cart</button>
    </div>
</section>
<script>
    let cartcount=0;
    let total=0;
    function addToCart(Price){
cartcount++;
total+=Price;
document.getElementById("cart").innerText =cartcount;
alert(`Food added to cart! Total Cost: $${total}`);
}

document.getElementById('checkout-btn').addEventListener('click', function() {
    if (cartcount === 0) {
        alert('Your cart is empty!');
    } else {
        alert(`Proceeding to checkout.Total cost: ${total}`);
    }
});
</script>
</body>
</html>
