<html>
<head>
<title>Practical 10 - Frames and Iframe | CS25044</title>

<style>

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #f0f0f0;
}

h1 {
    text-align: center;
    background: black;
    color: white;
    padding: 15px;
    margin: 0;
}

.container {
    display: flex;
    flex-direction: column;
    gap: 20px;
    padding: 20px;
}

.section {
    background: white;
    border-radius: 10px;
    padding: 15px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

.section h2 {
    margin: 0 0 10px 0;
    font-size: 16px;
    color: #333;
}

iframe {
    width: 100%;
    height: 400px;
    border: 2px solid black;
    border-radius: 8px;
}

.frames-row {
    display: flex;
    gap: 20px;
}

.frames-row iframe {
    flex: 1;
    height: 300px;
}

@media (max-width: 600px) {
    .frames-row {
        flex-direction: column;
    }
}

</style>

</head>
<body>

<h1>Practical 10 - HTML Iframe & Embedding | CS25044</h1>

<div class="container">

    <div class="section">
        <h2>Embedded Map - Nagpur, Maharashtra</h2>
        <iframe
            src="https://maps.google.com/maps?q=21.150273,79.1042573&z=15&output=embed"
            allowfullscreen=""
            loading="lazy">
        </iframe>
    </div>

    <div class="section">
        <h2>Embedded External Pages</h2>
        <div class="frames-row">
            <iframe src="https://www.wikipedia.org"></iframe>
            <iframe src="https://example.com"></iframe>
        </div>
    </div>

</div>

</body>
</html>
