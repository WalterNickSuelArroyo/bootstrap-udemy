# SECCION 3: ELEMENTOS DE BOOTSTRAP

# 15. Tipografia (Parte I)

- clase text-muted: se utiliza para aplicar un estilo visual que hace que el texto aparezca más tenue o desvanecido, lo que es útil para indicar que es un texto secundario o menos importante en comparación con el texto principal.

- clase h1: Aplica los estilos de un encabezado de nivel 1. Tambien se aplica para h2,h3, etc.

- clase display-1: aplica un tamaño de fuente significativamente mayor que los tamaños estándar de los encabezados. Lo mismo ocurre para display-2, display-3, etc.

- clase lead: La clase lead generalmente aplica un tamaño de fuente un poco más grande que el del texto normal, con un mayor espaciado entre líneas (line-height). Esto hace que el texto sea más fácil de leer y que se destaque como una introducción o un resumen.

- clase text-center: se utiliza para centrar el contenido de texto dentro del elemento que la contiene

- clase blockquote: añade estilos adicionales a la etiqueta <blockquote>, tales como márgenes, fuentes específicas, y un formato general que mejora la apariencia visual de la cita.

- blockquote-footer: Esta clase estiliza el pie de página de la cita, a menudo dándole un formato que indica que es un comentario, una fuente, o una atribución relacionada con la cita. Puede ser un texto en cursiva o con un color diferente, lo que ayuda a distinguirlo del contenido principal de la cita.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tipografia</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col">
                <h1>Encabezado H1 <small class="text-muted">Texto Secundario</small></h1>
                <h2>Encabezado H2 <small class="text-muted">Texto Secundario</small></h2>
                <h3>Encabezado H3 <small class="text-muted">Texto Secundario</small></h3>
                <h4>Encabezado H4 <small class="text-muted">Texto Secundario</small></h4>
                <h5>Encabezado H5 <small class="text-muted">Texto Secundario</small></h5>
                <h6>Encabezado H6 <small class="text-muted">Texto Secundario</small></h6>
            </div>
            <div class="col">
                <p class="h1">Encabezado H1 <small class="text-muted">Texto Secundario</small></p>
                <p class="h2">Encabezado H2 <small class="text-muted">Texto Secundario</small></p>
                <p class="h3">Encabezado H3 <small class="text-muted">Texto Secundario</small></p>
                <p class="h4">Encabezado H4 <small class="text-muted">Texto Secundario</small></p>
                <p class="h5">Encabezado H5 <small class="text-muted">Texto Secundario</small></p>
                <p class="h6">Encabezado H6 <small class="text-muted">Texto Secundario</small></p>
            </div>
            <hr>
            <div class="col">
                <h1 class="display-1">Display 1</h1>
                <h2 class="display-2">Display 2</h2>
                <h3 class="display-3">Display 3</h3>
                <h4 class="display-4">Display 4</h4>
                <h5 class="display-5">Display 5</h5>
                <h6 class="display-6">Display 6</h6>
            </div>
            <div class="col">
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. A et accusamus sapiente! Ipsa eum aperiam ipsum laborum</p>
                <p class="lead">Lorem ipsum dolor sit amet consectetur, adipisicing elit. A et accusamus sapiente! Ipsa eum aperiam ipsum laborum</p>
            </div>
            <hr>
            <div class="col">
                <figure class="text-center">
                    <blockquote class="blockquote">
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. At, eum?</p>
                    </blockquote>
                    <figcaption class="blockquote-footer">
                        Lorem <cite title="Titulo de la fuente">ipsum dolor</cite>  sit amet.
                    </figcaption>
                </figure>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

# 16. Tipografia (Parte II)



```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tipografia 2</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col-6">
                <p>Lorem <mark>ipsum dolor</mark> sit amet.</p>
                <p><del>Lorem ipsum dolor sit amet.</del></p>
                <p><s>Lorem ipsum dolor sit amet.</s></p>
                <p><ins>Lorem ipsum dolor sit amet.</ins></p>
                <p><u>Lorem ipsum dolor sit amet.</u></p>
                <p><strong>Lorem ipsum dolor sit amet.</strong></p>
                <p><em>Lorem ipsum dolor sit amet.</em></p>
            </div>
            <div class="col-6">
                <p class="fw-bold">Texto en negritas</p>
                <p class="fw-normal">Texto normal</p>
                <p class="fw-light">Texto light</p>
                <p class="fst-italic">Texto italic</p>
                <p class="fst-normal">Texto con font style normal</p>

                <p class="text-decoration-underline">Texto subrayado</p>
                <p class="text-decoration-line-through">Texto tachado</p>
                <a href="#" class="text-decoration-none">Enlace sin subrayado</a>
            </div>
            <div class="col-12">
                <hr>
                <p class="text-start">Texto alineado a la izquierda</p>
                <p class="text-center">Texto alineado al centro</p>
                <p class="text-end">Texto alineado a la derecha</p>
            </div>
            <hr>
            <div class="col-12">
                <p class="text-start text-sm-end">Alineado a la derecha en dispositivos pequeños en adelante</p>
                <p class="text-start text-md-end">Alineado a la derecha en dispositivos medianos en adelante</p>
                <p class="text-start text-lg-end">Alineado a la derecha en dispositivos largos en adelante</p>
                <p class="text-start text-xl-end">Alineado a la derecha en dispositivos extralargos en adelante</p>
            </div>
            <hr>
            <div class="col-12">
                <p class="text-lowercase">Minusculas - Lorem ipsum dolor sit.</p>
                <p class="text-uppercase">MAYUSCULAS - Lorem ipsum dolor sit.</p>
                <p class="text-capitalize">Letras Capitales - Lorem ipsum dolor sit.</p>
            </div>
            <div class="col-12">
                <p class="fs-1">Font Size 1</p>
                <p class="fs-2">Font Size 2</p>
                <p class="fs-3">Font Size 3</p>
                <p class="fs-4">Font Size 4</p>
                <p class="fs-5">Font Size 5</p>
                <p class="fs-6">Font Size 6</p>
            </div>
            <hr>
            <div class="col-6">
                <p class="text-primary">.text-primary</p>
                <p class="text-secondary">.text-secondary</p>
                <p class="text-success">.text-success</p>
                <p class="text-danger">.text-danger</p>
                <p class="text-dark">.text-dark</p>
                <p class="text-body">.text-body</p>
                <p class="text-muted">.text-muted</p>
            </div>
            <div class="col-6">
                <p class="text-warning  bg-dark">.text-warning</p>
                <p class="text-info  bg-dark">.text-info</p>
                <p class="text-light  bg-dark">.text-light</p>
                <p class="text-white  bg-dark">.text-white</p>


                <p class="text-black-50">.text-black-50</p>
                <p class="text-white-50 bg-dark">.text-black-50</p>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 17. Imagenes

- clase img-fluid: se aplica a las imágenes para hacerlas responsivas, es decir, para que se ajusten automáticamente al tamaño de su contenedor mientras mantienen sus proporciones originales.

- clase img-thumbnail: se aplica a imágenes para darles un estilo específico que imita la apariencia de una miniatura o "thumbnail". Esta clase añade un borde y un ligero padding (espaciado interno) alrededor de la imagen, haciendo que la imagen parezca estar dentro de un marco.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Imagenes</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col-6">
                <img class="img-fluid" src="./img-2/carousel1.jpg" alt="">
            </div>
            <hr>
            <div class="col-12">
                <img class="img-fluid float-start img-thumbnail" src="./img-2/bg.jpg" width="400" alt="">
                <img class="img-fluid float-end img-thumbnail" src="./img-2/bg2.jpg" width="400" alt="">
            </div>
            <hr>
            <div class="row">
                <div class="col-12">
                    <figure class="figure">
                        <img class="img-fluid rounded" src="img-2/bg3.jpg" width="400" alt="">
                        <figcaption class="figure-caption">
                            <p class="text-center">Lorem ipsum dolor sit amet.</p>
                        </figcaption>
                    </figure>
                </div>
            </div>
        </div>

    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

# 18. Tablas

- clase table-responsive: se aplica a un contenedor alrededor de una tabla para hacerla responsiva. Esto significa que la tabla podrá adaptarse y manejar mejor el desbordamiento de contenido en pantallas pequeñas, como en dispositivos móviles.

- clase table-striped: se aplica a una tabla para darle un estilo visual en el cual las filas alternan colores de fondo, creando un efecto de "rayado" o "zebra". Este estilo es especialmente útil para mejorar la legibilidad de las tablas al hacer que sea más fácil seguir la línea de datos de una fila a otra.

- clase table-hover: se utiliza para aplicar un efecto de resaltado a las filas de una tabla cuando el cursor del ratón pasa sobre ellas. 

- clase table-sm: se utiliza para hacer que una tabla tenga un diseño más compacto. Esto reduce el tamaño de las celdas y el espaciado entre ellas, lo que resulta en una tabla más pequeña y más condensada.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tablas</title>
    <link rel="stylesheet" href="css/bootstrap.min.css">
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="col">
                <div class="table-responsive">
                    <table class="table table-striped table-hover table-sm">
                        <caption>Lista de amigos</caption>
                        <thead>
                            <tr class="table-dark">
                                <th>Nombre</th>
                                <th>Edad</th>
                                <th>Pais</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>Carlos</td>
                                <td>25</td>
                                <td>Mexico</td>
                            </tr>
                            <tr>
                                <td>Alejandro</td>
                                <td class="table-active">34</td>
                                <td>España</td>
                            </tr>
                            <tr>
                                <td>Cesar</td>
                                <td>30</td>
                                <td>Colombia</td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
    <script src="js/bootstrap.bundle.min.js"></script>
</body>

</html>
```

