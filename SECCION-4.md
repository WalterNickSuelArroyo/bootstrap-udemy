# SECCION 4: COMPONENTES DE BOOTSTRAP

# 19. Acordeon (Accordion)

- data-bs-toggle="collapse": Es un atributo de datos usado por Bootstrap para indicar que el botón debe controlar un componente de colapso. Permite que el botón despliegue o colapse un elemento relacionado.

- data-bs-target="#elemento-1": Especifica el identificador del elemento que debe ser colapsado o desplegado cuando se haga clic en el botón. El valor debe coincidir con el id del elemento objetivo.

- aria-expanded="true": Atributo de accesibilidad que indica si el contenido relacionado está expandido (true) o colapsado (false). Ayuda a los lectores de pantalla a entender el estado del acordeón.

- aria-controls="elemento-1": Atributo de accesibilidad que especifica el id del elemento que el botón controla, proporcionando una referencia para los lectores de pantalla.

- accordion-collapse: Clase de Bootstrap que aplica estilos específicos a los elementos de acordeón.

- collapse: Clase que oculta el contenido inicialmente. Se utiliza para indicar que el contenido es colapsable.

- show: Clase que hace que el contenido sea visible cuando se aplica. Combinada con collapse, indica que este contenido está

- aria-label="encabezado-1": Atributo de accesibilidad que proporciona una etiqueta accesible para los usuarios de tecnologías asistivas. Describe el propósito del div en términos de accesibilidad.

- data-bs-parent="#temario": Especifica el id del contenedor padre que agrupa los elementos del acordeón. Esto asegura que solo un elemento del acordeón esté expandido a la vez.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Acordeon</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-4">
            <div class="col">
                <div class="accordion" id="temario">
                    <!-- Elemento #1 -->
                     <div class="accordion-item" >
                        <h2 class="accordion-header" id="encabezado-1">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#elemento-1" aria-expanded="true" aria-controls="elemento-1">
                                Capitulo #1
                            </button>
                        </h2>
                        <div id="elemento-1" class="accordion-collapse collapse show" aria-label="encabezado-1" data-bs-parent="#temario">
                            <div class="accordion-body">
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed ea doloremque suscipit ipsam eligendi necessitatibus ducimus earum in, modi optio repellendus repudiandae saepe, voluptatem, illum assumenda eos aliquid. Voluptates, fugiat.</p>
                            </div>
                        </div>
                     </div>
                     <!-- Elemento #2 -->
                     <div class="accordion-item" >
                        <h2 class="accordion-header" id="encabezado-2">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#elemento-2" aria-expanded="true" aria-controls="elemento-2">
                                Capitulo #2
                            </button>
                        </h2>
                        <div id="elemento-2" class="accordion-collapse collapse" aria-label="encabezado-2" data-bs-parent="#temario">
                            <div class="accordion-body">
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed ea doloremque suscipit ipsam eligendi necessitatibus ducimus earum in, modi optio repellendus repudiandae saepe, voluptatem, illum assumenda eos aliquid. Voluptates, fugiat.</p>
                            </div>
                        </div>
                     </div>
                     <!-- Elemento #3 -->
                     <div class="accordion-item" >
                        <h2 class="accordion-header" id="encabezado-3">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#elemento-3" aria-expanded="true" aria-controls="elemento-3">
                                Capitulo #3
                            </button>
                        </h2>
                        <div id="elemento-3" class="accordion-collapse collapse" aria-label="encabezado-3" data-bs-parent="#temario">
                            <div class="accordion-body">
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed ea doloremque suscipit ipsam eligendi necessitatibus ducimus earum in, modi optio repellendus repudiandae saepe, voluptatem, illum assumenda eos aliquid. Voluptates, fugiat.</p>
                            </div>
                        </div>
                     </div>
                </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 20. Alertas

- alert-dismissible: Añade estilos y funcionalidad para que la alerta sea cerrable, proporcionando un botón de cierre (X) para ocultar la alerta.

- fade: Clase que aplica una transición suave para la aparición y desaparición de la alerta.

- show: Clase que hace que la alerta sea visible. En combinación con fade, asegura que la alerta se muestre con una animación de desvanecimiento.

- btn-close: Clase de Bootstrap que aplica el estilo específico para un botón de cierre. Esto típicamente incluye un icono de "X" y estilos visuales para que el botón se vea como un botón de cierre en alertas, modales, y otros componentes.

- data-bs-dismiss="alert": Atributo de datos que indica que al hacer clic en el botón, se debe cerrar el elemento de alerta (alert). 

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alertas</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col">
                <div class="alert alert-primary alert-dismissible fade show mt-3" role="alert" aria-label="Close">
                    <strong>Aviso</strong> A simple primary alert—check it out! <a href="#" class="alert-link">Lorem,
                        ipsum.</a>
                    <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
                </div>
                <div class="alert alert-secondary mt-3" role="alert">
                    <strong>Aviso</strong> A simple primary alert—check it out! <a href="#" class="alert-link">Lorem,
                        ipsum.</a>
                </div>
                <div class="alert alert-danger mt-3" role="alert">
                    <strong>Aviso</strong> A simple primary alert—check it out! <a href="#" class="alert-link">Lorem,
                        ipsum.</a>
                </div>
                <div class="alert alert-warning mt-3" role="alert">
                    <strong>Aviso</strong> A simple primary alert—check it out! <a href="#" class="alert-link">Lorem,
                        ipsum.</a>
                </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 21. Insignias (Badges)

- class="badge": Clase de Bootstrap que aplica el estilo de una "badge" (etiqueta), que se usa para mostrar información adicional o resaltada.

- rounded-pill: Clase que aplica bordes redondeados con una forma de píldora a la "badge". Hace que la etiqueta tenga un borde curvado y una forma más suave en los extremos.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Insignias / Badges</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col">
                <h1>Encabezado H1 <span class="badge bg-primary">Etiqueta</span></h1>
                <h2>Encabezado H2 <span class="badge bg-primary">Etiqueta</span></h2>
                <h3>Encabezado H3 <span class="badge bg-primary">Etiqueta</span></h3>
                <h4>Encabezado H4 <span class="badge bg-primary">Etiqueta</span></h4>
                <h5>Encabezado H5 <span class="badge bg-primary">Etiqueta</span></h5>
                <h6>Encabezado H6 <span class="badge bg-primary">Etiqueta</span></h6>
            </div>
            <div class="col">
                <h3>Encabezado H3 <span class="badge bg-primary">Etiqueta</span></h3>
                <h3>Encabezado H3 <span class="badge bg-secondary">Etiqueta</span></h3>
                <h3>Encabezado H3 <span class="badge bg-success">Etiqueta</span></h3>
                <h3>Encabezado H3 <span class="badge rounded-pill bg-info">Etiqueta</span></h3>
                <h3>Encabezado H3 <span class="badge rounded-pill bg-warning">Etiqueta</span></h3>
                <h3>Encabezado H3 <span class="badge rounded-pill bg-danger">Etiqueta</span></h3>
            </div>
            <div class="col-12">
                <span class="badge bg-primary">Primary</span>
                <span class="badge bg-secondary">Primary</span>
                <span class="badge bg-success">Primary</span>
                <span class="badge bg-info">Primary</span>
                <span class="badge bg-warning">Primary</span>
                <span class="badge bg-danger">Primary</span>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 22. Migas de pan (Breadcrumbs)

- aria-label="breadcrumb": Atributo de accesibilidad que proporciona una etiqueta accesible para el componente de migas de pan. Ayuda a los usuarios de tecnologías asistivas a entender que este elemento es una navegación de tipo breadcrumb

- class="breadcrumb": Clase de Bootstrap que aplica el estilo específico para una lista de migas de pan. Esto proporciona un diseño adecuado para mostrar la ruta de navegación.

- class="breadcrumb-item": Clase de Bootstrap que aplica el estilo para los elementos individuales del breadcrumb. Esto asegura que cada ítem tenga el formato adecuado.

- class="breadcrumb-item active": Clase adicional que indica que este ítem es el elemento activo (actual) en la navegación. Se muestra sin enlace y destaca que es la página en la que el usuario se encuentra actualmente.

- aria-current="page": Atributo de accesibilidad que indica que este elemento es la página actual en la navegación.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Breadcrumbs / Migas de pan</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col mt-3">
                <nav aria-label="breadcrumb">
                    <ol class="breadcrumb">
                        <li class="breadcrumb-item"><a href="#">Home</a></li>
                        <li class="breadcrumb-item active" aria-current="page">Library</li>
                    </ol>
                </nav>
            </div>
        </div>
    </div>

    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 23. Botones

- clase d-grid: Clase de Bootstrap que convierte al div en un contenedor con un sistema de cuadrícula CSS. Esto significa que los elementos hijos (en este caso, los botones) se dispondrán en un diseño basado en la cuadrícula.

- clase gap: Clase que aplica un espacio (gap) entre los elementos de la cuadrícula. 

- clase d-flex: aplica el sistema de diseño Flexbox al contenedor div. Esto permite que los elementos hijos dentro del div se alineen y distribuyan utilizando las propiedades de Flexbox, como dirección, alineación, distribución del espacio, etc.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap 5</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col-12 mt-3">
                <button type="button" class="btn btn-primary">Primary</button>
                <button type="button" class="btn btn-link">Enlace</button>
            </div>
            <div class="col-12 mt-3">
                <button type="button" class="btn btn-outline-primary">Primary</button>
                <button type="button" class="btn btn-outline-danger">Enlace</button>
            </div>
            <div class="col-12 mt-3">
                <button type="button" class="btn disabled btn-primary">Primary</button>
                <button type="button" class="btn disabled btn-danger">Enlace</button>
            </div>
            <div class="col-12 mt-3">
                <a href="#" class="btn btn-primary">Enlace</a>
                <button type="button" class="btn btn-primary">Boton</button>
                <input type="button" class="btn btn-primary" value="Boton Input">
                <input type="submit" class="btn btn-primary" value="submit">
            </div>
            <div class="col-12 mt-3">
                <button type="button" class="btn btn-lg btn-primary">Boton Grande</button>
                <button type="button" class="btn btn-lg btn-secondary">Boton Secundario Grande</button>

                <button type="button" class="btn btn-sm btn-primary">Boton Pequeño</button>
                <button type="button" class="btn btn-sm btn-secondary">Boton Secundario Pequeño</button>
            </div>
            <div class="col-12 mt-3">
                <div class="d-grid gap-2 col-12">
                    <button type="button" class="btn btn-primary">Primario</button>
                    <button type="button" class="btn btn-secondary">Secundario</button>
                </div>
            </div>
            <div class="col-12 mt-3">
                <div class="d-flex gap-2 justify-content-between">
                    <button type="button" class="btn btn-primary">Primario</button>
                    <button type="button" class="btn btn-secondary">Secundario</button>
                </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 24. Grupos de Botones







```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grupos de botones</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col">
                <div class="btn-group" role="group" aria-label="Basic example">
                    <button type="button" class="btn btn-primary active">Left</button>
                    <button type="button" class="btn btn-primary">Middle</button>
                    <button type="button" class="btn btn-primary">Right</button>
                </div>
            </div>
            <div class="col-12">
                <hr class="mt-3">
                <div class="btn-group" role="group" aria-label="Basic example">
                    <button type="button" class="btn btn-outline-primary active">Left</button>
                    <button type="button" class="btn btn-outline-primary">Middle</button>
                    <button type="button" class="btn btn-outline-primary">Right</button>
                </div>
            </div>
            <div class="col-12">
                <hr class="mt-3">
                <div class="btn-group btn-group-lg" role="group" aria-label="Basic example">
                    <button type="button" class="btn btn-outline-primary active">Left</button>
                    <button type="button" class="btn btn-outline-primary">Middle</button>
                    <button type="button" class="btn btn-outline-primary">Right</button>
                </div>
            </div>
            <div class="col-12">
                <hr class="mt-3">
                <div class="btn-group btn-group-lg" role="group" aria-label="Basic example">
                    <input type="checkbox" name="checkbox-1" id="checkbox-1" class="btn-check">
                    <label for="checkbox-1" class="btn btn-primary">Checkbox1</label>

                    <input type="checkbox" name="checkbox-2" id="checkbox-2" class="btn-check">
                    <label for="checkbox-2" class="btn btn-primary">Checkbox2</label>

                    <input type="checkbox" name="checkbox-3" id="checkbox-3" class="btn-check">
                    <label for="checkbox-3" class="btn btn-primary">Checkbox3</label>
                </div>
            </div>
            <div class="col-12">
                <hr class="mt-3">
                <div class="btn-group btn-group-lg" role="group" aria-label="Basic example">
                    <input type="radio" name="radio" id="radio-1" class="btn-check">
                    <label for="radio-1" class="btn btn-primary">Radio1</label>

                    <input type="radio" name="radio" id="radio-2" class="btn-check">
                    <label for="radio-2" class="btn btn-primary">Radio2</label>

                    <input type="radio" name="radio" id="radio-3" class="btn-check">
                    <label for="radio-3" class="btn btn-primary">Radio3</label>
                </div>
            </div>

            <!-- Toolbar -->
            <div class="col-12">
                <hr class="mt-3">
                <div class="btn-toolbar" role="toolbar" aria-label="Barra de herramientas">
                    <div class="btn-group me-2" role="group" aria-label="Basic example">
                        <button type="button" class="btn btn-primary active">Nuevo</button>
                        <button type="button" class="btn btn-primary">Editar</button>
                        <button type="button" class="btn btn-primary">Guardar</button>
                    </div>
                    <div class="btn-group" role="group" aria-label="Basic example">
                        <button type="button" class="btn btn-info active">Alinear Izquierda</button>
                        <button type="button" class="btn btn-info">Alinear Centro</button>
                        <button type="button" class="btn btn-info">Alinear Derecha</button>
                    </div>
                </div>
            <div class="col-12">
                <hr class="mt-3">
                <div class="btn-group-vertical" role="group" aria-label="Basic example">
                    <button type="button" class="btn btn-primary active">Left</button>
                    <button type="button" class="btn btn-primary">Middle</button>
                    <button type="button" class="btn btn-primary">Right</button>
                </div>
            </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 25. Cards (Parte I)

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bootstrap 5</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col">
                <div class="card">
                    <div class="card-body">
                        <h1>Encabezado</h1>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Obcaecati corrupti sit quam
                            suscipit. Reiciendis quidem consequatur suscipit aperiam quasi quo, cum facilis,
                            voluptatibus vitae tenetur explicabo velit eum laborum distinctio!</p>
                    </div>

                </div>
            </div>
        </div>
        <div class="row mt-3">
            <div class="col-4">
                <div class="card">
                    <img class="card-img-top" src="img-2/bg.jpg" alt="">
                    <div class="card-body">
                        <h5 class="card-title">Titulo</h5>
                        <h6 class="card-subtitle text-muted mb-2">Subtitulo</h6>
                        <p class="card-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Mollitia aliquid deserunt, cumque fugiat tempora dolorem placeat atque at sapiente.</p>
                        <a href="#" class="btn btn-outline-primary">Boton</a>
                    </div>
                </div>
            </div>
            <div class="col-4">
                <div class="card">
                    <div class="card-body">
                        <h5 class="card-title">Titulo</h5>
                        <h6 class="card-subtitle text-muted mb-2">Subtitulo</h6>
                        <p class="card-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Mollitia aliquid deserunt, cumque fugiat tempora dolorem placeat atque at sapiente.</p>
                        <a href="#" class="btn btn-outline-primary">Boton</a>
                    </div>
                    <img class="card-img-bottom" src="img-2/bg.jpg" alt="">
                </div>
            </div>
            <div class="col-4">
                <div class="card">
                    <img class="card-img-top" src="img-2/bg.jpg" alt="">
                    <ul class="list-group list-group-flush">
                        <li class="list-group-item">Elemento #1</li>
                        <li class="list-group-item">Elemento #2</li>
                        <li class="list-group-item">Elemento #3</li>
                    </ul>
                    <div class="card-body">
                        <p class="card-text">Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                        <a href="#" class="btn btn-outline-primary">Boton</a>
                    </div>
                </div>
            </div>

        </div>
        <div class="row mt-3">
            <div class="col-6">
                <div class="card">
                    <div class="card-header">Encabezado</div>
                    <div class="card-body">
                        <h5 class="card-title">Titulo</h5>
                        <p class="card-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aperiam quod iste est reiciendis aut reprehenderit.</p>
                    </div>
                    <div class="card-footer">Footer</div>
                </div>
            </div>
            <div class="col-6">
                <div class="card text-center">
                    <div class="card-header">Cita</div>
                    <div class="card-body">
                        <blockquote class="blockquote mb-0">
                            <p>
                                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Animi, eveniet!
                            </p>
                            <footer class="blockquote-footer">Lorem, ipsum dolor.</footer>
                        </blockquote>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 26.Cards (Parte II)

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cards 2</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col-12 mt-5">
                <div class="card">
                    <div class="card-header">
                        <ul class="nav nav-tabs card-header-tabs">
                            <li class="nav-item">
                                <a href="#" class="nav-link active">Enlace #1</a>
                            </li>
                            <li class="nav-item">
                                <a href="#" class="nav-link">Enlace #2</a>
                            </li>
                            <li class="nav-item">
                                <a href="#" class="nav-link">Enlace #3</a>
                            </li>
                        </ul>
                    </div>
                    <div class="card-body">
                        <h5 class="card-title">Titulo</h5>
                        <p>Lorem ipsum dolor sit amet.</p>
                        <button type="button" class="btn btn-primary">Boton</button>
                    </div>
                </div>
            </div>
            <div class="col-12 mt-5">
                <div class="card">
                    <div class="card-header">
                        <ul class="nav nav-pills card-header-pills">
                            <li class="nav-item">
                                <a href="#" class="nav-link active">Enlace #1</a>
                            </li>
                            <li class="nav-item">
                                <a href="#" class="nav-link">Enlace #2</a>
                            </li>
                            <li class="nav-item">
                                <a href="#" class="nav-link">Enlace #3</a>
                            </li>
                        </ul>
                    </div>
                    <div class="card-body">
                        <h5 class="card-title">Titulo</h5>
                        <p>Lorem ipsum dolor sit amet.</p>
                        <button type="button" class="btn btn-primary">Boton</button>
                    </div>
                </div>
            </div>
            <div class="col-4 my-5">
                <div class="card bg-primary text-white">
                    <div class="card-header">Encabezado</div>
                    <div class="card-body">
                        <h5 class="card-title">Titulo</h5>
                        <p>Lorem ipsum dolor sit amet.</p>
                    </div>
                </div>
            </div>
            <div class="col-4 my-5">
                <div class="card border-primary">
                    <div class="card-header">Encabezado</div>
                    <div class="card-body">
                        <h5 class="card-title">Titulo</h5>
                        <p>Lorem ipsum dolor sit amet.</p>
                    </div>
                </div>
            </div>
            <div class="col-12 mb-5">
                <div class="card-group">
                    <div class="card">
                        <div class="card-header">Encabezado</div>
                        <div class="card-body">
                            <h5 class="card-title">Titulo</h5>
                            <p>Lorem ipsum dolor sit amet.</p>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-header">Encabezado</div>
                        <div class="card-body">
                            <h5 class="card-title">Titulo</h5>
                            <p>Lorem ipsum dolor sit amet.</p>
                        </div>
                    </div>
                    <div class="card">
                        <div class="card-header">Encabezado</div>
                        <div class="card-body">
                            <h5 class="card-title">Titulo</h5>
                            <p>Lorem ipsum dolor sit amet.</p>
                        </div>
                    </div>
                </div>
                
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 27. Carrusel(Slideshow)

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carousel / Slideshow</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-5">
            <div class="col">
                <div class="carousel slide carousel-fade" id="mi-carousel" data-bs-ride="carousel">
                    <div class="carousel-inner">
                        <div class="carousel-item active">
                            <img class="img-fluid" src="img-2/carousel1.jpg" alt="">
                        </div>
                        <div class="carousel-item" data-bs-interval="1000">
                            <div class="carousel-caption">
                                <h5>Titulo de mi articulo</h5>
                                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit, quam.</p>
                            </div>
                            <img class="img-fluid" src="img-2/carousel2.jpg" alt="">
                        </div>
                        <div class="carousel-item">
                            <img class="img-fluid" src="img-2/carousel3.jpg" alt="">
                        </div>
                    </div>

                    <!-- Controles -->
                     <button class="carousel-control-prev" type="button" data-bs-target="#mi-carousel" data-bs-slide="prev">
                        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Anterior</span>
                     </button>
                     
                     <button class="carousel-control-next" type="button" data-bs-target="#mi-carousel" data-bs-slide="next">
                        <span class="carousel-control-next-icon" aria-hidden="true"></span>
                        <span class="visually-hidden">Anterior</span>
                     </button>

                     <!-- Indicadores -->
                      <div class="carousel-indicators">
                        <button type="button" class="active" data-bs-target="#mi-carousel" data-bs-slide-to="0" aria-label="Slide 1"></button>
                        <button type="button" class="" data-bs-target="#mi-carousel" data-bs-slide-to="1" aria-label="Slide 2"></button>
                        <button type="button" class="" data-bs-target="#mi-carousel" data-bs-slide-to="2" aria-label="Slide 3"></button>
                      </div>
                </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 28. Collapse

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Collapse</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row mt-3">
            <div class="col-6">
                <a href="#contenido-1" type="button" class="btn btn-primary" data-bs-toggle="collapse" aria-expanded="false" aria-controls="contenido-1">Informacion</a>
                <div class="collapse mt-3" id="contenido-1">
                    <div class="card">
                        <div class="card-body">
                            <h2 class="card-title">Titulo</h2>
                            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti porro magni blanditiis commodi cumque!</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-6">
                <button type="button" class="btn btn-primary" data-bs-toggle="collapse" data-bs-target="#contenido-2" aria-expanded="false" aria-controls="contenido-2">Informacion</button>
                <div class="collapse mt-3" id="contenido-2">
                    <div class="card">
                        <div class="card-body">
                            <h2 class="card-title">Titulo</h2>
                            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti porro magni blanditiis commodi cumque!</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```