## Assignment 7.2 — Pricing Cards & Centered Login Form

### `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pricing and Login</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Our Pricing Plans</h1>

    <div class="pricing-container">
        <div class="card">
            <h2>Basic</h2>
            <h3>₹199/month</h3>
            <p>Basic features</p>
            <p>Email support</p>
            <button>Choose Basic</button>
        </div>

        <div class="card">
            <h2>Pro</h2>
            <h3>₹499/month</h3>
            <p>All basic features</p>
            <p>Priority support</p>
            <button>Choose Pro</button>
        </div>

        <div class="card">
            <h2>Premium</h2>
            <h3>₹999/month</h3>
            <p>All Pro features</p>
            <p>24/7 support</p>
            <button>Choose Premium</button>
        </div>
    </div>

    <div class="login-container">
        <form class="login-form">
            <h2>Login</h2>
            <input type="email" placeholder="Email" required>
            <input type="password" placeholder="Password" required>
            <button type="submit">Sign In</button>
        </form>
    </div>
</body>
</html>
```

### `style.css`

```css
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f0f4f8;
    text-align: center;
}

.pricing-container {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
}

.card {
    background: white;
    padding: 25px;
    width: 250px;
    border-radius: 12px;
    box-shadow: 0 4px 10px #ccc;
}

button {
    background: navy;
    color: white;
    border: none;
    padding: 10px 15px;
    border-radius: 5px;
    cursor: pointer;
}

.login-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 350px;
    padding: 20px;
}

.login-form {
    display: flex;
    flex-direction: column;
    gap: 15px;
    width: 300px;
    max-width: 100%;
    padding: 25px;
    background: white;
    border-radius: 12px;
    box-shadow: 0 4px 10px #ccc;
}

input {
    padding: 10px;
    border: 1px solid #aaa;
    border-radius: 5px;
}

@media (max-width: 600px) {
    .pricing-container {
        flex-direction: column;
        align-items: center;
    }
}
```

**Submission:** Save both files in the same folder and open `index.html` using Live Server. The pricing cards use Flexbox, and the login form is centered using `justify-content`, `align-items`, and `flex-direction`.