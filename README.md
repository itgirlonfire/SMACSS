index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>SMACSS Example</title>
</head>
<body>
    <header class="layout__header">
        <h1 class="base__title">SMACSS Example</h1>
    </header>
    
    <main class="layout__main">
        <section class="module module--card">
            <h2 class="module__title">Card Title</h2>
            <p class="module__description">This is a description of the card.</p>
            <button class="module__button module__button--primary">Primary Button</button>
            <button class="module__button module__button--secondary">Secondary Button</button>
        </section>

        <section class="module module--card">
            <h2 class="module__title">Another Card Title</h2>
            <p class="module__description">Another description for a different card.</p>
            <button class="module__button module__button--primary">Primary Button</button>
        </section>
    </main>
</body>
</html>

styles.css
/* Base Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #ffeef8; /* Light pink background */
}

.base__title {
    color: #d5006d; /* Dark pink title */
    text-align: center;
    padding: 20px;
}

/* Layout Styles */
.layout__header {
    background-color: #d5006d; /* Dark pink header */
    color: white;
    padding: 15px;
}

.layout__main {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    padding: 20px;
}

/* Module Styles */
.module {
    background-color: white;
    border: 1px solid #ddd;
    border-radius: 4px;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    margin: 10px;
    padding: 20px;
    width: 300px;
}

.module__title {
    font-size: 1.5em;
    margin: 0 0 10px;
    color: #d5006d; /* Dark pink title for modules */
}

.module__description {
    font-size: 1em;
    margin: 0 0 20px;
}

/* Button Styles */
.module__button {
    display: inline-block;
    padding: 10px 15px;
    margin: 5px;
    border: none;
    border-radius: 3px;
    cursor: pointer;
    text-align: center;
}

.module__button--primary {
    background-color: #d5006d; /* Dark pink button */
    color: white;
}

.module__button--secondary {
    background-color: #ffd1e0; /* Light pink button */
    color: #333;
}
