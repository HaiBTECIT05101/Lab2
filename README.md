# Lab2
<!DOCTYPE html>
<html>
<head>
    <title>Website bán hàng</title>
    <link rel="stylesheet" type="text/css" href="style.css">
    <script src="script.js"></script>
</head>
<body>
    <header>
        <h1>Website bán hàng</h1>
    </header>

    <nav>
        <ul>
            <li><a href="#">Home Page</a></li>
            <li><a href="#">Product</a></li>
            <li><a href="#">Cart</a></li>
            <li><a href="#">Log in</a></li>
        </ul>
    </nav>

    <main>
        <section>
            <h2>Latest product</h2>
            <div class="product">
                <img src="product1.jpg" alt="Sản phẩm 1">
                <h3>Product 1</h3>
                <p>Price: $10</p>
                <button onclick="addToCart(1)">Thêm vào giỏ hàng</button>
            </div>
            <div class="product">
                <img src="product2.jpg" alt="Product 2">
                <h3>Product 2</h3>
                <p>Price: $15</p>
                <button onclick="addToCart(2)">Add to cart</button>
            </div>
        </section>
    </main>

    <footer>
        <p>Copyright © 2023 - Sales Website</p>
    </footer>
</body>
<!-- Add a checkout button to each product -->
<div class="product">
    <img src="product1.jpg" alt="Product 1">
    <h3>Product 1</h3>
    <p>Price: $10</p>
    <button onclick="addToCart(1)">Add to cart</button>
    <button onclick="checkout(1)">Pay</button>
</div>
<!-- Add a form to each product -->
<div class="product">
    <img src="product1.jpg" alt="Product 1">
    <h3>Product 1</h3>
    <p>Price: $10</p>
    <form method="post" action="process.php">
        <input type="hidden" name="productId" value="1">
        <button type="submit" name="checkout">Pay</button>
    </form>
</div>

</html>
