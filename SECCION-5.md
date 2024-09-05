# SECCION 5: FORMULARIOS EN BOOTSTRAP

# 29. Estructura basica de los formularios en Bootstrap

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap 5</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col-6">
                <form action="">
                    <div class="mb-3">
                        <label for="correo" class="form-label">Correo Electrónico</label>
                        <input type="text" class="form-control" id="correo" aria-describedby="ayuda-correo">
                        <div id="ayuda-correo" class="form-text">Te enviaremos un mensaje de confirmación</div>
                    </div>

                    <div class="mb-3">
                        <label for="mensaje" class="form-label">Mensaje</label>
                        <textarea class="form-control" name="mensaje" id="mensaje"></textarea>
                    </div>

                    <button type="submit" class="btn btn-primary">Enviar</button>
                    
                </form>
            </div>

            <div class="col-6">
                <form action="">
                    <input type="text" class="form-control form-control-lg mb-3" placeholder="Input Grande">
                    <input type="text" class="form-control form-control-sm mb-3" placeholder="Input Grande">
                    <input type="text" class="form-control mb-3" placeholder="Input Deshabilitado" disabled>
                    <input type="text" class="form-control mb-3" placeholder="Input solo lectura" readonly>
                    <input type="text" class="form-control-plaintext mb-3" placeholder="Input solo lectura" readonly>
                    <input type="file" class="form-control">
                </form>
            </div>
        </div>
    </div>
    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 30. Selectbox

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Select Box</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <select name="pais" id="pais" class="form-select mb-3" aria-label="seleccion de pais mb-3">
                <option value="mexico">México</option>
                <option value="mexico">España</option>
                <option value="mexico">Colombia</option>
            </select>

            <select name="pais" id="pais" class="form-select form-select-lg mb-3" aria-label="seleccion de pais">
                <option value="mexico">México</option>
                <option value="mexico">España</option>
                <option value="mexico">Colombia</option>
            </select>

            <select name="pais" id="pais" class="form-select form-select-sm mb-3" aria-label="seleccion de pais">
                <option value="mexico">México</option>
                <option value="mexico">España</option>
                <option value="mexico">Colombia</option>
            </select>

            <select multiple size="3" name="pais" id="pais" class="form-select mb-3" aria-label="seleccion de pais">
                <option value="mexico">México</option>
                <option value="españa">España</option>
                <option value="colombia">Colombia</option>
                <option value="peru">Perú</option>
                <option value="argentina">Argentina</option>
            </select>

            <select disabled name="pais" id="pais" class="form-select form-select-sm mb-3" aria-label="seleccion de pais">
                <option value="mexico">México</option>
                <option value="mexico">España</option>
                <option value="mexico">Colombia</option>
            </select>
        </div>
    </div>
    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 31. Checkbox y Radio Buttons

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap 5</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <!-- Checkbox -->
            <div class="col-4">
                <div class="form-check">
                    <input type="checkbox" name="checkbox-1" class="form-check-input" id="checkbox-1">
                    <label for="checkbox-1" class="form-check-label"> Checkbox 1</label>
                </div>
                <div class="form-check">
                    <input type="checkbox" name="checkbox-2" class="form-check-input" id="checkbox-2">
                    <label for="checkbox-2" class="form-check-label"> Checkbox 2</label>
                </div>
                <div class="form-check">
                    <input type="checkbox" name="checkbox-3" class="form-check-input" id="checkbox-3">
                    <label for="checkbox-3" class="form-check-label"> Checkbox 3</label>
                </div>
            </div>

            <!-- Radio Buttons -->
            <div class="col-4">
                <div class="form-check">
                    <input type="radio" name="mi-radio-button" class="form-check-input" id="radio-1">
                    <label for="radio-1" class="form-check-label"> Radio 1</label>
                </div>
                <div class="form-check">
                    <input type="radio" name="mi-radio-button" class="form-check-input" id="radio-2">
                    <label for="radio-2" class="form-check-label"> Radio 2</label>
                </div>
                <div class="form-check">
                    <input type="radio" name="mi-radio-button" class="form-check-input" id="radio-3">
                    <label for="radio-3" class="form-check-label"> Radio 3</label>
                </div>
            </div>

            <!-- Switch -->
            <div class="col-4">
                <div class="form-check form-switch">
                    <input type="checkbox" name="switch-1" class="form-check-input" id="switch-1">
                    <label for="switch-1" class="form-check-label"> Switch 1</label>
                </div>
                <div class="form-check form-switch">
                    <input type="checkbox" name="switch-2" class="form-check-input" id="switch-2">
                    <label for="switch-2" class="form-check-label"> Switch 2</label>
                </div>
                <div class="form-check form-switch">
                    <input type="checkbox" name="switch-3" class="form-check-input" id="switch-3">
                    <label for="switch-3" class="form-check-label"> Switch 3</label>
                </div>
            </div>

            <!-- Checkbox inline -->
            <div class="col-12 mt-4">
                <div class="form-check form-check-inline">
                    <input type="checkbox" name="checkbox-inline-1" class="form-check-input" id="checkbox-inline-1">
                    <label for="checkbox-inline-1" class="form-check-label"> Checkbox 1</label>
                </div>
                <div class="form-check form-check-inline">
                    <input type="checkbox" name="checkbox-inline-2" class="form-check-input" id="checkbox-inline-2">
                    <label for="checkbox-inline-2" class="form-check-label"> Checkbox 2</label>
                </div>
                <div class="form-check form-check-inline">
                    <input type="checkbox" name="checkbox-inline-3" class="form-check-input" id="checkbox-inline-3">
                    <label for="checkbox-inline-3" class="form-check-label"> Checkbox 3</label>
                </div>
            </div>

            <!-- Checkbox estilo boton-->
            <div class="col-6 mt-4">
                <input type="checkbox" name="checkbox-button-1" class="btn-check" id="checkbox-button-1">
                <label for="checkbox-button-1" class="btn btn-primary"> Checkbox 1</label>


                <input type="checkbox" name="checkbox-button-2" class="btn-check" id="checkbox-button-2">
                <label for="checkbox-button-2" class="btn btn-primary"> Checkbox 2</label>


                <input type="checkbox" name="checkbox-button-3" class="btn-check" id="checkbox-button-3" disabled>
                <label for="checkbox-button-3" class="btn btn-primary"> Checkbox 3</label>
            </div>

            <!-- Radio estilo boton-->
            <div class="col-6 mt-4">
                <input type="radio" name="radio-button" class="btn-check" id="radio-button-1">
                <label for="radio-button-1" class="btn btn-primary"> Radio 1</label>

                <input type="radio" name="radio-button" class="btn-check" id="radio-button-2">
                <label for="radio-button-2" class="btn btn-primary"> Radio 2</label>

                <input type="radio" name="radio-button" class="btn-check" id="radio-button-3">
                <label for="radio-button-3" class="btn btn-primary"> Radio 3</label>
            </div>
        </div>
    </div>

    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 32. Input de rango

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Range</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col-6">
                <label for="rango" class="form-label">Presupuesto</label>
                <input type="range" class="form-range" name="" id="rango" min="0" max="1000" step="100">
                <div class="d-flex justify-content-between">
                    <p class="form-text">$0</p>
                    <p class="form-text">$1000</p>
                </div>
            </div>
        </div>
    </div>
    
    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 33. Grupo de inputs

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Input Group</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col-6">
                <!-- Input Group -->
                 <div class="input-group mb-3">
                    <input type="text" class="form-control" placeholder="Nombre" aria-label="Nombre">
                    <span class="input-group-text">@gmail.com</span>
                 </div>

                 <!-- Text Area -->
                 <div class="input-group mb-3">
                    <span class="input-group-text">Notas:</span>
                    <textarea class="form-control" id="label-notas" aria-label="Notas"></textarea>                 
                 </div>

                 <!-- Input Group con multiples elementos -->
                 <div class="input-group mb-3">
                    <span class="input-group-text">Nombre</span>
                    <input type="text" class="form-control" aria-label="Nombre">

                    <span class="input-group-text">Apellido</span>
                    <input type="text" class="form-control" aria-label="Apellido">                 
                 </div>

                 <div class="input-group">
                    <label for="pais" class="input-group-text">Pais</label>
                    <select name="" id="pais" class="form-select">
                        <option value="mexico">Mexico</option>
                        <option value="peru">Peru</option>
                        <option value="españa">España</option>
                    </select>
                    <button class="btn btn-primary">Enviar</button>
                 </div>
            </div>
        </div>
    </div>
    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 34. Etiquetas flotantes para formularios

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Floating Label</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col-6">
                <div class="form-floating mb-3">
                    <input type="text" name="nombre" id="nombre" class="form-control" placeholder="Nombre">
                    <label for="nombre">Nombre</label>
                </div>
                
                <div class="form-floating mb-3">
                    <textarea name="notas" id="notas" class="form-control" placeholder="notas"></textarea>
                    <label for="Notas">Notas</label>
                </div>

                <div class="form-floating mb-3">
                    <select name="pais" id="pais" class="form-select">
                        <option selected>Selecciona una opción</option>
                        <option value="mexico">Mexico</option>
                        <option value="peru">Peru</option>
                        <option value="españa">España</option>
                    </select>
                    <label for="pais">Selecciona un pais</label>
                </div>
            </div>
        </div>
    </div>
    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 35. [PRACTICA] Creando un formulario con grid de bootstrap I

# 36. [PRACTICA] Creando un formulario con grid de bootstrap II

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formularios con Grid</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col">
                <form action="">
                    <div class="row">
                        <div class="col-12 col-md-6 mb-3">
                            <label for="nombre" class="form-label">Nombre</label>
                            <input id="nombre" type="text" class="form-control" placeholder="Walter Suel">
                        </div>
                        <div class="col-12 col-md-6 mb-3">
                            <label for="correo" class="form-label">Correo</label>
                            <input id="correo" type="email" class="form-control" placeholder="correo@correo.com">
                        </div>
                    </div>

                    <div class="row">
                        <div class="col-12 col-md-6 mb-3">
                            <label for="mensaje" class="form-label">Mensaje</label>
                            <textarea name="mensaje" id="mensaje" class="form-control"></textarea>
                        </div>

                        <div class="col-12 col-md-6 mb-3">
                            <div class="row">
                                <div class="col-12 col-sm-6 mb-3">
                                    <label class="form-label">Estado Civil</label>
                                    <div class="form-check">
                                        <input class="form-check-input" type="radio" name="estado-civil" id="soltero">
                                        <label for="soltero" class="form-check-label">Soltero</label>
                                    </div>

                                    <div class="form-check">
                                        <input class="form-check-input" type="radio" name="estado-civil" id="casado">
                                        <label for="casado" class="form-check-label">Casado</label>
                                    </div>

                                </div>
                                <div class="col-12 col-sm-6 mb-3">
                                    <label class="form-label">Pais</label>
                                    <select name="pais" id="pais" class="form-select">
                                        <option selected>Selecciona una opción</option>
                                        <option value="mexico">Mexico</option>
                                        <option value="peru">Peru</option>
                                        <option value="españa">España</option>
                                    </select>
                                </div>
                            </div>
                        </div>
                    </div>

                    <div class="row">
                        <div class="col-12 d-flex justify-content-center">
                            <div>
                                <div class="form-check mb-3">
                                    <input type="checkbox" name="terminos" id="terminos" class="form-check-input">
                                    <label for="terminos" class="form-check-label">Acepto los terminos y condiciones</label>
                                </div>
                                <button type="submit" class="col-12 btn btn-primary">Enviar</button>
                            </div>
                        </div>
                    </div>
                </form>
            </div>
        </div>
    </div>
    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 37. Clases para validacion de formularios

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Clases para Validación</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-5">
            <div class="col-6">
                <form action="">
                    <label for="nombre" class="form-label">Nombre</label>
                    <input type="text" class="form-control is-valid" placeholder="nombre" id="nombre">
                    <div class="valid-feedback">Correcto!</div>
                </form>
            </div>

            <div class="col-6">
                <form action="">
                    <label for="correo" class="form-label">Correo</label>
                    <input type="text" class="form-control is-invalid" placeholder="correo@correo.com" id="correo">
                    <div class="invalid-feedback">Por favor, introduzca un correo valido</div>
                </form>
            </div>
        </div>
    </div>
    
    <script src="../js/bootstrap.bundle.min.js"></script>
</body>

</html>
```
