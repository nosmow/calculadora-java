<h1 align="center" id="title">Calculadora.exe</h1>

<p align="center"><img src="https://socialify.git.ci/nosmow/calculadora-java/image?font=Inter&forks=1&issues=1&language=1&name=1&owner=1&pattern=Solid&stargazers=1&theme=Auto" alt="project-image"></p>

<p id="description">Este proyecto se desarrolló utilizando el lenguaje Java y consiste en una aplicación de escritorio diseñada para simular las operaciones fundamentales de una calculadora. Además, ofrece la flexibilidad de alternar entre los modos Claro  y Oscuro, proporcionando una experiencia visual adaptada a las preferencias del usuario.</p>

## Tabla de Contenido

- [Demo](#demo)
- [Características](#caracteristicas)
- [Instalación](#instalacion)
- [Proceso de desarrollo](#proceso-de-desarrollo)
  - [Construido con](#construido-con)
  - [Estructura](#estructura)
  - [Documentación](#documentacion)
- [Recursos utilizados](#recursos-utilizados)
- [Licencia](#licencia)
- [Autor](#autor)

## Demo

<img height="400px" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExenMxNWg5cXo3YzgyZzRqZGc2Z2o3emlvcXV4aXF0ZDBkanVqZHVhaSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/5vAAapQSGOeqWKdJjy/giphy.gif"/>


## Caracteristicas

Estas son algunas de las características del proyecto:

*   Permite realizar las operaciones básicas de una calculadora
*   Puedes elegir entre modo Claro u Oscuro
*   La interfaz está diseñada para que sea amigable a la vista del usuario


## Instalacion:

1. Descargue la ultima versión de [Java JDK](https://www.oracle.com/java/technologies/downloads/)
2. Descargue el IDE [Apache NetBeans](https://netbeans.apache.org/download/index.html)
3. Clone el repositoria mediante el siguiente enlace: https://github.com/nosmow/Calculadora_Java.git
4. Abra el proyecto en el IDE Apache NetBeans
5. Compile y ejecute la aplicación, listo.

## Proceso de desarrollo
### Construido con

Tecnologías usadas en el proyecto:

*   Java 19.0.2
*   Apache NetBeans IDE 18
*   Windows 11 22H2

### Estructura

``` Java
// Este metodo se encarga de añadir el numero seleccionado a la pantalla 
//de la calculadora, Si ha ejecutado alguna operacion como suma 
//el resultado en pantalla se borra y se empieza a mostrar los nuevos 
//números que este seleccionando

public void AnadirNumero(JLabel jlbl, double numero) {       
        try {
            if(jlbl.getText().startsWith("0") && 
               !jlbl.getText().startsWith("0.") ||          
                this.limpiar == true) {
                
                //limpia la pantalla
                jlbl.setText("");
                limpiar = false;
            }
            
            // Añade el numero a la pantalla
            jlbl.setText(jlbl.getText() + this.ValidarDecimales(numero));
            
        } catch (ArithmeticException e) {
            e.getMessage();
            limpiar = true;
        }
    }
```

### Documentacion

*   Clic para acceder al [javadoc](https://github.com/nosmow/Calculadora_Java/tree/main/dist/javadoc)

## Recursos utilizados

* [Wenhui Yu](https://dribbble.com/shots/3756276-Daily-UI-004-Calculator/attachments/10002349?mode=media) - Diseño base de la calculadora.
* [Photopea](https://www.photopea.com/) - Mejor alternativa gratuita a Photoshop
* [FiveCodMover](https://mega.nz/file/guhw1IRD#LFa8hjhACXqsgoJRdlwux-KaOu6Hc0_wlJwkL4R4kd4) - Librería de Java creada por FiveCod SoftWare

## Licencia:

> Este proyecto está licenciado bajo la licencia Creative Commons

## Autor

Hecho con 💙 por [Nosmow](https://www.linkedin.com/in/nosmow)
