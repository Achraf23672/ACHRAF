<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Delicious Kitchen</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
</head>
<body>
    <header>
        <div class="container">
            <h1><i class="fas fa-utensils"></i> Delicious Kitchen</h1>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#recipes">Recipes</a></li>
                    <li><a href="#upload">Upload Recipe</a></li>
                    <li><a href="#about">About</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <section id="home" class="hero">
            <h2>Discover & Share Amazing Recipes</h2>
            <p>Join our community of food lovers and explore thousands of delicious recipes from around the world.</p>
            <a href="#recipes" class="btn">Browse Recipes</a>
        </section>

        <section id="recipes">
            <h2>Featured Recipes</h2>
            <div class="recipe-grid" id="recipe-container">
                <!-- Recipes will be loaded here dynamically -->
            </div>
        </section>

        <section id="upload" class="upload-form">
            <h2>Share Your Recipe</h2>
            <form id="recipe-form">
                <div class="form-group">
                    <label for="recipe-name">Recipe Name</label>
                    <input type="text" id="recipe-name" required>
                </div>
                <div class="form-group">
                    <label for="recipe-image">Image URL</label>
                    <input type="url" id="recipe-image" placeholder="https://example.com/image.jpg">
                </div>
                <div class="form-group">
                    <label for="recipe-category">Category</label>
                    <select id="recipe-category" required>
                        <option value="">Select a category</option>
                        <option value="breakfast">Breakfast</option>
                        <option value="lunch">Lunch</option>
                        <option value="dinner">Dinner</option>
                        <option value="dessert">Dessert</option>
                        <option value="snack">Snack</option>
                    </select>
                </div>
                <div class="form-group">
                    <label for="recipe-time">Prep Time (minutes)</label>
                    <input type="number" id="recipe-time" required>
                </div>
                <div class="form-group">
                    <label for="recipe-ingredients">Ingredients (one per line)</label>
                    <textarea id="recipe-ingredients" rows="5" required></textarea>
                </div>
                <div class="form-group">
                    <label for="recipe-instructions">Instructions</label>
                    <textarea id="recipe-instructions" rows="8" required></textarea>
                </div>
                <button type="submit" class="btn">Upload Recipe</button>
            </form>
        </section>

        <section id="about">
            <h2>About Delicious Kitchen</h2>
            <p>We're a community of food enthusiasts dedicated to sharing and discovering the best recipes from around the world. Whether you're a professional chef or a home cook, you'll find inspiration in our collection.</p>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2023 Delicious Kitchen. All rights reserved.</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-pinterest"></i></a>
            </div>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>
