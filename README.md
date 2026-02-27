# RegistroPHP
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>


<header>
    <img src = "deadpool.png" alt = "Logo">
    <a href = "https://www.google.com" target = "-blank"> Ir a google</a>
</header>

<section class ="hero">
    <h1> Bienvenido a Nuestra Landing Page </h1>
    <p> Completa el formulario para registarte </p>
    <img src =  "loki.png" alt="Imagen Principal">
</section>

<div class = "form-container">
    <h2> Formulario de Registro </h2>
    <form id="registroForm" method="POST" enctype ="multipart/form-data"

</div>

<body>
<div class = "form-container">
        <form id = "registroForm" method ="POST" enctypr="multipart/form-data">
    

     <div class ="form-group">
        <label> Nombre: </label>
        <input type ="text" id = "nombre" required>
    </div>

    <div class ="form-group">
        <label> Apellido: </label>
        <input type ="text" id = "apellido" required>
    </div>

     <div class ="form-group">
        <label> Edad: </label>
        <input type ="number" id = "edad" required>
    </div> 

    <div class ="form-group">
        <label> Correo: </label>
        <input type ="email" id = "correo" required>
    </div>

     <div class ="form-group">
        <label> Género: </label>
        <div class ="radio-group">
            <label><input type ="radio" name = "genero" 
            value=" Masculino" required> Masculino</label>
            <label><input type="radio" name = "genero"
            value ="Femenino"> Femenino </label>
        </div>
    </div>

    <div class ="form-group">
        <label> Estado civil: </label>
        <select id="estadoCivil" required>
            <option value ="">Seleccione</option>
            <option value ="1">Soltero/a</option>
            <option value ="2">Casado/a</option>
            <option value ="3">Divorciado/a</option>
            <option value ="4">Unión Libre</option>
        </select>
    </div>

    <div class ="form-group">
        <label>Subir Archivo:</label>
        <input type ="file" id=" archivo"required>
    </div>

    <button type="submit">  Enviar </button>
    </form>
</div>
</body>

<style>
    * {
        box-sizing: border-box;
    }
 
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        background: #f4f6f9;
    }
 
    header {
        background:forestgreen;
        color: white;
        padding: 15px 40px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        flex-wrap: wrap;
    }
 
    header img {
        height: 50px;
    }
 
    header a {
        color:darkgreen;
        text-decoration: none;
        font-weight: bold;
    }
 
    .hero {
        text-align: center;
        padding: 40px 20px;
    }
 
    .hero img {
        width: 100%;
        max-width: 400px;
        height: auto;
        border-radius: 10px;
    }
 
    .form-container {
        width: 90%;
        max-width: 500px;
        margin: 30px auto;
        background: white;
        padding: 25px;
        border-radius: 10px;
        box-shadow: 0px 4px 12px rgba(0,0,0,0.1);
    }
 
    .form-group {
        margin-bottom: 15px;
    }
 
    input, select {
        width: 100%;
        padding: 10px;
        border-radius: 5px;
        border: 1px solid #ccc;
    }
 
    .radio-group {
        display: flex;
        gap: 15px;
        margin-top: 5px;
        flex-wrap: wrap;
    }
 
    button {
        width: 100%;
        padding: 12px;
        background: #1e2a38;
        color: white;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-size: 16px;
    }
 
    button:hover {
        background: #34495e;
    }
 
    footer {
        text-align: center;
        padding: 15px;
        background: #1e2a38;
        color: white;
        margin-top: 30px;
    }
 
    /*  MEDIA QUERIES */
 
    @media (max-width: 768px) {
        header {
            flex-direction: column;
            text-align: center;
        }
 
        header a {
            margin-top: 10px;
        }
 
        .hero {
            padding: 20px;
        }
    }
 
    @media (max-width: 480px) {
        body {
            font-size: 14px;
        }
 
        .form-container {
            padding: 15px;
        }
 
        button {
            font-size: 14px;
        }
    }
 
</style>
</html>
