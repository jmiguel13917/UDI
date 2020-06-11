<!DOCTYPE html>
<html>

<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <style>
        body {
            background-image: url('https://www.xtrafondos.com/wallpapers/espacio-interestelar-universo-2900.jpg');
            background-repeat: repeat-y;
        }
        .header img {
            float: left;
            width: 100px;
            height: 100px;
            background-color: transparent;
        }

        .header h1 {
            position: relative;
            top: 18px;
            left: 10px;
        }
        .mynav ul {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            list-style-type: none;
            padding: 0;
        }

        .mynav li:not(:last-child) {
            margin-right: 20px;
        }

        .mynav a {
            display: block;
            font-size: 20px;
            color: black;
            text-decoration: none;
            padding: 7px 15px;
        }

        .target {
            position: absolute;
            border-bottom: 4px solid transparent;
            z-index: -1;
            transform: translateX(-60px);
        }

        .mynav a, .target {
            transition: all .35s ease-in-out;
        }

        footer {
            position: fixed;
            left: 0;
            bottom: 0;
            width: 100%;
            height: 50px;
            background-color: darkslategrey;
            color: white;
            text-align: right;
        }

        * {
            box-sizing: border-box
        }

        body, html {
            height: 100%;
            margin: 0;
            color: white;
            font-size: 20px;
            font-family: Arial;
        }

        .tablink {
            background-color: #555;
            color: white;
            float: left;
            border: none;
            outline: none;
            cursor: pointer;
            padding: 14px 16px;
            font-size: 17px;
            width: 25%;
        }

         .tablink:hover {
            background-color: #777;
            }

        .tabcontent {
            color: white;
            display: none;
            padding: 100px 20px;
            height: 100%;
        }

        {
            box-sizing: border-box;
        }

        input[type=text], select, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            margin-top: 6px;
            margin-bottom: 16px;
            resize: vertical;
        }

        input[type=tel] {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            margin-top: 6px;
            margin-bottom: 16px;
            resize: vertical;
        }

        input[type=email] {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
            margin-top: 6px;
            margin-bottom: 16px;
            resize: vertical;
        }

        input[type=submit] {
            background-color: #4CAF50;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

            input[type=submit]:hover {
                background-color: #45a049;
            }

        .container {
            border-radius: 5px;
            background-color: #f2f2f2;
            padding: 20px;
            color: black;
            width: 50%;
            align-content: center;
            margin: 50px auto;
            float: none;
        }
        .banner {
            width: 100%;
            height: 20vh;
        }
         .banner img {
             height: 132px;
             width: 232px;
             background-color: transparent;
            }
        .parent {
            display: flex;
            flex-wrap: wrap;
        }

        .child {
            flex: 1 0 21%;
            margin: 5px;
            height: auto;
            background-color: palegreen;
        }
    </style>
</head>

<link rel="icon"
      type="image/png"
      href="https://www.iebschool.com/frontend/assets/img/icons/RSC1.png">

<div class="header">
    <img src="https://www.iebschool.com/frontend/assets/img/icons/RSC1.png" alt="logo"/>
    <center><h1>Actividad Final</h1></center>
</div>

<ul>
    <center>
        <script>
            var meses = new Array("Enero", "Febrero", "Marzo", "Abril", "Mayo", "Junio", "Julio", "Agosto", "Septiembre", "Octubre", "Noviembre", "Diciembre");
            var diasSemana = new Array("Domingo", "Lunes", "Martes", "Miércoles", "Jueves", "Viernes", "Sábado");
            var f = new Date();
            document.write(diasSemana[f.getDay()] + ", " + f.getDate() + " de " + meses[f.getMonth()] + " de " + f.getFullYear());
        </script>
    </center>
</ul>
<body>

    <button class="tablink" onclick="openPage('Inicio', this, 'lightseagreen')" id="defaultOpen">Inicio</button>
    <button class="tablink" onclick="openPage('QuienesSomos', this, 'plum')">Quienes Somos</button>
    <button class="tablink" onclick="openPage('Productos', this, 'palegreen')">Productos</button>
    <button class="tablink" onclick="openPage('Contactenos', this, 'deepskyblue')">Contactenos</button>


    <div id="Inicio" class="tabcontent">
        <h3>Inicio</h3>
        <p>
            Hola! , bienvenidos a mi sitio.
            Está concebido este sitio, para que nos sirva de orientación e  información con respecto a todo lo que son las nuevas tecnologías, Mi intención, con la creación de este sitio, es la de tener una herramienta al alcance de la mano que nos sirva de apoyo a la hora de realizar cualquier actividad, hay muchos productos tambien que al entusiasta de la tecnologia de manera muy motivadora le va a encantar.
            Espero hacer de este sitio un recurso fácil, efectivo y  claro, para que los entusiastas se vayan animando a hacer de los recursos tecnologicos en casa u oficina, una herramienta de trabajo sencilla y de uso diario, para de ese modo, convertir a nuestro entorno al Siglo XXI.
        </p>
        <center>
            <div class="banner" onclick="openPage('QuienesSomos')">
                <img src="https://www.thebizfest.com/public/template/img/quienes-somos.png">
            </div>
            <div class="banner" onclick="openPage('Productos')">
                <img src="https://images.vexels.com/media/users/3/200097/isolated/lists/942820836246f08c2d6be20a45a84139-icono-de-carrito-de-compras-carrito-de-compras.png">
            </div>
        </center>
    </div>

    <div id="QuienesSomos" class="tabcontent">
        <center>
            <h2>Quienes Somos</h2>
            <p>Somos JOYASA, una compańía dedicada a brindar productos y servicios que estén a la vanguardia de las últimas tendencias que el mercado demanda. Reunimos nuestros esfuerzos y trabajamos profesionalmente colaborando en un círculo multidisciplinario, el cual permite un compromiso del personal y las altas gerencias para: Asegurar el desempeńo de requisitos aplicables y normativas que regulan nuestro campo de acción. Satisfacer los requerimientos de nuestros clientes, basándonos en la ética de ofrecerles soluciones integrales de productos y servicios de la más alta calidad. Desarrollar continuamente la competencia de nuestro personal, valorizando y reconociéndolo en las tareas que desempeñan, siendo profesionales al guiarnos bajo una cultura institucional que funge como estándar. Mejorar nuestros procesos internos a fin de prevalecer como diferenciadores en calidad, precio e innovación.</p>

            <h2>Mision</h2>
            <p>Conectar a las personas de manera segura, con excelencia operativa y un toque personal</p>

            <h2>Vision</h2>
            <p>Ser líder en el mercado nacional en los segmentos de tecnologia para los sectores privados y empresariales.</p>
            <br />
            <p> Nuestro CEO</p>
            <img src="https://cdn.pixabay.com/photo/2020/06/06/05/23/yo-5265272_960_720.jpg" width="214"
                 height="285">
        </center>
    </div>

    <div id="Productos" class="tabcontent">
        <div class="parent">
            <div class="child">
                <img src="https://www.yoytec.com/images/klip/klip_kss-710_tn.gif"
                <br />
                <h3>Bocinas</h3>
                <p>Alambricas y Bluetooth</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/kingston/kingston_kvr1333d3s9_8g_tn.gif"
                <br />
                <h3>Memoria RAM</h3>
                <p>Memorias RAM DDR3 y DDR4</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/logitech/logitech_981-000014_tn.gif"
                <br />
                <h3>Audifonos</h3>
                <p>Alambricos y Bluetooth</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/nexxt/nexxt_aw250nxt05_tn.gif"
                <br />
                <h3>Herramientas</h3>
                <p>Ponchadoras y Herramientas</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/generic/generic_crw-inwb_tn.gif"
                <br />
                <h3>Lectoras</h3>
                <p>Lectoras USB,SD,MicroSD</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/generic/generic_hdmi-hdmi-15f-2_tn.gif"
                <br />
                <h3>Cables</h3>
                <p>Cables USB y Serial</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/canon/canon_pg-145xl_tn.gif"
                <br />
                <h3>Tintas Canon</h3>
                <p>Tintas para Impresoras Canon</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/arcticsilver/arctic_silver_5_tn.gif"
                <br />
                <h3>Pasta Térmica</h3>
                <p>Pastas térmicas para procesadores y tarjetas de video</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/logitech/logitech_910-001354_tn.gif"
                <br />
                <h3>Punteros</h3>
                <p>Punteros laser para sus presentaciones</p>
            </div>
            <div class="child">
                <img src="https://www.yoytec.com/images/epson/BotellaTintaMagentaEpson664_tn.gif"
                <br />
                <h3>Tintas Epson</h3>
                <p>Tintas para impresoras Epson</p>
            </div>
            
            <h1> Quieres saber más sobre los productos, envíanos un mensaje en el area de contáctenos !</h1>
            <br />
        </div>

        </div>
        <div id="Contactenos" class="tabcontent">
            <center>
                <h1>Datos de la Empresa</h1>
                <h2>Ubicación</h2>
                <p> Nos encontramos ubicados en Plaza Burunga, Arraijan, Panamá</p>
                <p>Nuestra dirección de correo electrónico es <a href="mailto:jbuitrago_e3@udi.edu.pa">JoYaSa Panamá</a></p>
                <p>Nuestros teléfonos de contacto son el 845-5214 y el 852-7845</p>
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15765.158974606808!2d-79.66762183453378!3d8.945426042079841!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8faca3e6cdb42621%3A0x85461a86ec6d8a03!2sPlaza%20Burunga!5e0!3m2!1ses!2spa!4v1591418225962!5m2!1ses!2spa" width="600" height="450" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
            </center>

            <center><h3>Formulario de Contacto</h3></center>

            <div class="container">

                <form name="form1" action="javascript: enviar()">

                    <label for="fname">Nombre</label>
                    <input type="text" id="fname" name="Nombre" placeholder="Su nombre..">

                    <label for="lname">Apellido</label>
                    <input type="text" id="lname" name="Apellido" placeholder="Su Apellido..">

                    <label for="tel">Teléfono</label>
                    <input type="tel" id="tel" name="tel" placeholder="Su numero de telefono...">

                    <label for="email">Email</label>
                    <input type="email" id="email" name="email" placeholder="Su E-Mail...">

                    <label for="mensaje">Mensaje</label>
                    <textarea id="mensaje" name="mensaje" placeholder="Escribanos sus comentarios..." style="height:80px"></textarea>

                    <center><input type="submit" value="Enviar"></center>

                </form>
            </div>

            <br>

            </br>

        </div>
        <script>
            function openPage(pageName, elmnt, color) {
                var i, tabcontent, tablinks;
                tabcontent = document.getElementsByClassName("tabcontent");
                for (i = 0; i < tabcontent.length; i++) {
                    tabcontent[i].style.display = "none";
                }
                tablinks = document.getElementsByClassName("tablink");
                for (i = 0; i < tablinks.length; i++) {
                    tablinks[i].style.backgroundColor = "";
                }
                document.getElementById(pageName).style.display = "block";
                elmnt.style.backgroundColor = color;
            }

            document.getElementById("defaultOpen").click();

            function enviar() {
                alert('Formulario Enviado');
                var nom = document.form1.fname.value; var ape = document.form1.lname.value; var tel = document.form1.tel.value;
                alert('Ingreso el nombre:'+" " + nom +" " + ape +" y numero de contacto: " + tel);
            }

            function preguntar(event) {
                var opcion = confirm("Formulario Enviado");
                if (!opcion) {
                    event.preventDefault();
                }

                }
        </script>
        }

    </script>

    <footer id="footer">
        <p class="copyright">&copy; Jose Miguel Buitrago 2016. Sitio Web con los derechos reservados. </p>
    </footer>

</body>
</html>

