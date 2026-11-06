HTML
<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Card Designs & Display Properties Showcase</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Card Designs & Display Properties</h1>
        <p>Exploring distinct backgrounds, borders, rounded corners, and display behaviors.</p>
    </header>

    <main class="container">
        <!-- Section 1: 3 Card Designs -->
        <section class="cards-section">
            <h2>Subscription Cards</h2>
            <div class="cards-grid">
                <!-- Card 1: Basic -->
                <div class="card card-basic">
                    <h3>Basic Plan</h3>
                    <p>Essential features for personal use and beginner web development projects.</p>
                    <button class="btn">Choose Basic</button>
                </div>

                <!-- Card 2: Standard -->
                <div class="card card-standard">
                    <h3>Standard Plan</h3>
                    <p>Great for growing projects with expanded toolsets and support.</p>
                    <button class="btn">Choose Standard</button>
                </div>

                <!-- Card 3: Premium -->
                <div class="card card-premium">
                    <h3>Premium Plan</h3>
                    <p>Advanced tools, priority support, and full access to all resources.</p>
                    <button class="btn">Choose Premium</button>
                </div>
            </div>
        </section>

        <!-- Section 2: Display Property Demonstration -->
        <section class="display-section">
            <h2>Display Property Demonstrations</h2>
            <div class="display-demo">
                <h3>1. <code>display: inline</code></h3>
                <p>This paragraph contains <span class="demo-inline">inline elements</span> like this span, which flow naturally within text and ignore width/height properties.</p>

                <h3>2. <code>display: block</code></h3>
                <div class="demo-block">
                    This box is a block-level element. It takes up the full available width and starts on a new line.
                </div>

                <h3>3. <code>display: inline-block</code></h3>
                <div class="demo-inline-block">Box A</div>
                <div class="demo-inline-block">Box B</div>
                <div class="demo-inline-block">Box C</div>
                <p class="demo-caption">These boxes sit side by side like inline elements while respecting custom widths, heights, padding, and margins.</p>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2026 Atim Akhtar. All rights reserved.</p>
    </footer>
</body>
</html>
CSS
/* style.css */
body {
    font-family: Arial, sans-serif;
    background-color: #f8fafc;
    color: #334155;
    margin: 0;
    padding: 0;
    line-height: 1.6;
}

header {
    background-color: #0f172a;
    color: #ffffff;
    text-align: center;
    padding: 2.5rem 1rem;
}

header h1 {
    margin-bottom: 0.5rem;
}

header p {
    color: #94a3b8;
    margin: 0;
}

.container {
    max-width: 900px;
    margin: 2rem auto;
    padding: 0 1rem;
    display: flex;
    flex-direction: column;
    gap: 2.5rem;
}

section {
    background-color: #ffffff;
    border: 1px solid #e2e8f0;
    border-radius: 12px;
    padding: 2rem;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.05);
}

h2 {
    color: #0f172a;
    border-bottom: 2px solid #e2e8f0;
    padding-bottom: 0.5rem;
    margin-top: 0;
    margin-bottom: 1.5rem;
}

/* Cards Grid & Styles */
.cards-grid {
    display: flex;
    gap: 1.5rem;
    flex-wrap: wrap;
    justify-content: center;
}

.card {
    flex: 1;
    min-width: 240px;
    max-width: 280px;
    padding: 1.5rem;
    border-radius: 12px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    transition: transform 0.2s ease;
}

.card:hover {
    transform: translateY(-4px);
}

/* Card 1: Basic */
.card-basic {
    background-color: #ffffff;
    border: 2px solid #cbd5e1;
}

/* Card 2: Standard */
.card-standard {
    background-color: #f0fdf4;
    border: 2px solid #22c55e;
}

/* Card 3: Premium */
.card-premium {
    background-color: #faf5ff;
    border: 2px solid #a855f7;
}

.card h3 {
    margin-top: 0;
    color: #0f172a;
    font-size: 1.25rem;
}

.card p {
    color: #475569;
    font-size: 0.95rem;
    margin-bottom: 1.5rem;
}

.btn {
    background-color: #0f172a;
    color: #ffffff;
    border: none;
    border-radius: 6px;
    padding: 0.6rem 1rem;
    font-weight: bold;
    cursor: pointer;
    transition: background-color 0.2s ease;
}

.btn:hover {
    background-color: #334155;
}

/* Display Property Demonstration Styles */
.display-demo h3 {
    font-size: 1.1rem;
    color: #334155;
    margin-top: 1.2rem;
    margin-bottom: 0.5rem;
}

/* Inline Element Demo */
.demo-inline {
    background-color: #fed7aa;
    color: #9a3412;
    padding: 2px 6px;
    font-weight: bold;
    /* Note: width and height properties are ignored on inline elements */
}

/* Block Element Demo */
.demo-block {
    display: block;
    background-color: #e0f2fe;
    color: #0369a1;
    border: 1px dashed #0284c7;
    padding: 12px;
    border-radius: 6px;
    width: 100%;
}

/* Inline-Block Element Demo */
.demo-inline-block {
    display: inline-block;
    background-color: #f3e8ff;
    color: #6b21a8;
    border: 1px solid #9333ea;
    padding: 10px 20px;
    margin-right: 10px;
    border-radius: 6px;
    width: 100px;
    height: 40px;
    text-align: center;
    line-height: 20px;
    font-weight: bold;
}

.demo-caption {
    font-size: 0.9rem;
    color: #64748b;
    margin-top: 0.8rem;
}

footer {
    text-align: center;
    padding: 1.5rem;
    color: #64748b;
    font-size: 0.875rem;
    border-top: 1px solid #e2e8f0;
    margin-top: 2rem;
}