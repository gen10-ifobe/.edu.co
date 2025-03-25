<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inicio de Sesión - Institución Educativa</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
    <link rel="stylesheet" href="styles.css">
    <script>
        function validarLogin(event) {
            event.preventDefault();
            var email = document.getElementById("email").value;
            var password = document.getElementById("password").value;
            
            if (email === "admin@ifobe.edu.com"&& password === "Admin2024@") {
                alert("Inicio de sesión exitoso");
                window.location.href = "home.html";
            } else {
                alert("Credenciales incorrectas");
            }
        }
    </script>
    
</head>

<body class="bg-light d-flex justify-content-center align-items-center vh-100">
       <div class="container-fluid">
        <div class="row vh-100">
            <div class="col-md-6 d-flex justify-content-center align-items-center bg-primary text-white p-5">
                <img src="img/logo.png" alt="Logo Institución" class="img-fluid" style="max-width: 60%;">
            </div>
            <div class="col-md-6 d-flex justify-content-center align-items-center">
                <div class="card shadow-lg p-5 w-75">
                    <div class="card-body">
                        
                        <h3 class="text-center mb-4">Inicio de Sesión</h3>
                        <form onsubmit="validarLogin(event)">
                            <div class="mb-3">
                                <label for="email" class="form-label">Correo Electrónico</label>
                                <input type="email" class="form-control" id="email" placeholder="Ingrese su correo">
                            </div>
                            <div class="mb-3">
                                <label for="password" class="form-label">Contraseña</label>
                                <input type="password" class="form-control" id="password" placeholder="Ingrese su contraseña">
                            </div>
                            <div class="mb-3 form-check">
                                <input type="checkbox" class="form-check-input" id="recordar">
                                <label class="form-check-label" for="recordar">Recordar sesión</label>
                            </div>
                            <button type="submit" class="btn btn-primary w-100">Iniciar Sesión</button>
                        </form>
                        <p class="text-center mt-3"><a href="#">¿Olvidaste tu contraseña?</a></p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
