# Creating a basic HTML and CSS structure for the website "Only for Students"
# Save the files into a zip file for download

# File structure:
# /only_for_students/
#   index.html
#   style.css

import zipfile

# HTML content
html_content = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Only for Students</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>Only for Students</h1>
            <p>Simplify homework and note sharing</p>
        </div>
    </header>
    <main>
        <section class="about">
            <h2>About Us</h2>
            <p>Welcome to Only for Students, a platform where students can share homework and notes to help each other succeed. Explore resources by subject and grade level.</p>
        </section>
        <section class="features">
            <h2>Features</h2>
            <ul>
                <li>Upload and download notes</li>
                <li>Organized by subject and grade</li>
                <li>Secure student-only access</li>
            </ul>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Only for Students. All rights reserved.</p>
    </footer>
</body>
</html>
"""

# CSS content
css_content = """
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header {
    background: #4CAF50;
    color: white;
    padding: 20px 0;
    text-align: center;
}

header .container h1 {
    margin: 0;
    font-size: 2.5em;
}

header .container p {
    margin: 5px 0 0;
    font-size: 1.2em;
}

main {
    padding: 20px;
}

.about, .features {
    margin-bottom: 20px;
}

.features ul {
    list-style: none;
    padding: 0;
}

.features li {
    background: #f9f9f9;
    border: 1px solid #ddd;
    margin: 5px 0;
    padding: 10px;
}

footer {
    background: #333;
    color: white;
    text-align: center;
    padding: 10px 0;
    margin-top: 20px;
}
"""

# Creating the zip file with HTML and CSS
zip_path = "/mnt/data/only_for_students.zip"

with zipfile.ZipFile(zip_path, "w") as z:
    z.writestr("index.html", html_content)
    z.writestr("style.css", css_content)

zip_path

<!---
Jeetrawal12345/Jeetrawal12345 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
