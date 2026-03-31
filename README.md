```css id="redoval7"
* {
    box-sizing: border-box;
    font-family: 'Segoe UI', 'Poppins', system-ui, sans-serif;
}

body {
    background: linear-gradient(135deg, #fff1f1, #ffe5e5);
    margin: 0;
    padding: 20px;
    color: #2d1f1f;
}

.container {
    max-width: 1200px;
    margin: auto;
    background: #ffffffcc;
    backdrop-filter: blur(10px);
    border-radius: 30px;
    overflow: hidden;
    box-shadow: 0 10px 40px rgba(150,0,0,0.1);
}

/* HEADER */
.header {
    background: linear-gradient(135deg, #ff4d4d, #b30000);
    padding: 25px;
    text-align: center;
    color: white;
}

.header h1 {
    margin: 0;
    font-weight: 600;
}

/* LAYOUT */
.main-content {
    display: flex;
    flex-wrap: wrap;
    gap: 25px;
    padding: 25px;
}

.form-panel, .list-panel {
    flex: 1;
    min-width: 300px;
}

/* INPUTS */
input, textarea {
    width: 100%;
    padding: 12px;
    margin: 10px 0;
    border-radius: 14px;
    border: 1px solid #f0b3b3;
    background: #fff7f7;
    transition: 0.3s;
}

input:focus, textarea:focus {
    outline: none;
    border-color: #ff4d4d;
    background: white;
}

/* BUTTONS (OVAL STYLE) */
button {
    padding: 10px 18px;
    border: none;
    border-radius: 999px; /* FULL OVAL */
    cursor: pointer;
    background: linear-gradient(135deg, #ff4d4d, #cc0000);
    color: white;
    margin: 5px 5px 5px 0;
    transition: 0.3s;
    font-weight: 500;
}

button:hover {
    transform: translateY(-2px) scale(1.03);
    box-shadow: 0 6px 18px rgba(200,0,0,0.25);
}

/* RECIPE CARD */
.recipe-card {
    background: white;
    padding: 15px;
    border-radius: 20px;
    margin-bottom: 15px;
    box-shadow: 0 5px 20px rgba(150,0,0,0.08);
    transition: 0.3s;
}

.recipe-card:hover {
    transform: translateY(-4px);
}

.recipe-card h3 {
    margin: 0 0 5px;
}

.recipe-card small {
    color: #aa6666;
}

/* MODAL */
.modal {
    display: none;
    position: fixed;
    top:0; left:0;
    width:100%; height:100%;
    background: rgba(80,0,0,0.5);
    justify-content: center;
    align-items: center;
}

.modal-content {
    background: white;
    padding: 25px;
    border-radius: 25px;
    max-width: 500px;
    width: 90%;
    box-shadow: 0 10px 30px rgba(100,0,0,0.3);
    animation: fadeIn 0.3s ease;
}

@keyframes fadeIn {
    from {opacity: 0; transform: scale(0.9);}
    to {opacity: 1; transform: scale(1);}
}

/* EMPTY TEXT */
#recipeList p {
    text-align: center;
    color: #cc8888;
}
```
