# CSS Layouts and Responsive Design

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Responsive website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>My small piece of Work</h1>
        <p>This is the website I'm currently working on right now</p>
        <img scr="C:\Users\caiphus Laka\New folder\cinema.jpg">
    </div>
    <nav class="navbar">
        <ul class="nav-links">
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
    <main class="container">
        <div class="grid-item">
            <p>Nothing in the world can take the place of persistence. Talent will not; nothing is more common than unsuccessful men with talent. Genius will not; unrewarded genius is almost a proverb. Education will not; the world is full of educated derelicts. The slogan 'Press On' has solved and always will solve the problems of the human race.</p>
            </div>
        <div class="grid-item">
            <p>Success is peace of mind, which is a direct result of self-satisfaction in knowing you made the effort to become the best of which you are capable</p>
            </div>
        <div class="grid-item">
            <p>If you are working on something that you really care about, you don't have to be pushed. The vision pulls you</p>
        </div>
    </main>
</body>
</html>

style.css

.container {
    width: 80%;
    height:500px;
    margin: 0;
    background-color: orange;
}

img {
    width: 100%;
    height: auto;
}
body {
    font-family: Arial, sans-serif;
}

.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #333;
    padding: 10px 20px;
    color: white;
}

.content {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 20px;
    padding: 20px;
}

.grid-item {
    background-color: #f0f0f0;
    padding: 20px;
    border: 1px solid #ddd;
    text-align: center;
}

/* Media Queries */
@media only screen (max-width: 600px) {
    body {
        background-color: orange;
    }

    .container{
        width: 100%;
        background-color: crimson;
    }
    .content {
        grid-template-columns: repeat(1, 1fr);
    }
}

@media (min-width: 350px) and (max-width: 500px) {
    .content {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (min-width: 350px) {
    .content {
        grid-template-columns: repeat(3, 1fr);
    }
}

.container {
    display: flex;
    justify-content: center;

    align-items: center;
    padding: 30px;
    height: 85px;
    background-color: antiquewhite;
}

.items{
    background-color: black;
    padding: 20px;
    margin: 10px;
    flex: 1;
}
