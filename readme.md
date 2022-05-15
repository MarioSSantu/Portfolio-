https://www.figma.com/file/MnvrTPgZYjfcPCC7nVVHHa/Untitled?node-id=0%3A1


**CONCEPTO BÁSICO DE DISEÑO**

La idea fundamental que manejaba a la hora de diseñar esta web portfolio era que estuviera construida en tres páginas a modo de web empresarial (salvando las distancias). La primera de esas páginas estaría orientada a describirme a mi, mi background, mis habilidades y lenguajes conocidos y simplemente dar unas breves referencias.

El restultado final debería ser algo similar a esto:


![Primera página de la web!](/Portfolio-\diseño2.jpg "Primera página de la web")

Para ello y en toda la página decidí utilizar secciones en flex que incluirían o bien pequeños contenedores con información/imagenes que se podrían articular solos o en flex/grid como por ejemplo: 

```HTML
{

 <div class="contenedor_seccion">
          <h2 class="titulo_texto">Mi formación</h2>
          <div class="formacion">
              <div class="formacion_apartado">
                  <a href="https://www.uniovi.es/ " target="_blank"><img src="Imagenes\historia.jpg"></a>
                  <p>Grado en Historia <br>por la Universidad de Oviedo<br> 2012-2018</p>
              </div>
              <div class="formacion_apartado">
                  <a href="https://www.uniovi.es/" target="_blank"><img src="Imagenes\master.buena.jpg"></a>
                  <p>Master en historia y análisis sociocultural<br> por la Universidad de Oviedo<br> 2018-2019</p>
              </div>
              <div class="formacion_apartado">
                  <a href="https://afa-formacion.com/" target="_blank"><img src="Imagenes\web.jpg" ></a>
                  <p>CFSG Desarrollo App Web <br> por AFA Formación (Oviedo)<br> 2021-2023.</p>
              </div>
          </div>


}
```

```CSS

{

.contenedor_seccion{
      display: flex;
      padding-top: 30px;
      justify-content: center;
      align-items: center;
      padding-bottom: 30px;
      flex-direction: column;
     width: 100%;
     background-color: aquamarine;
  }
  .formacion{
    padding-top: 30px;
    display: flex;
    justify-content: space-between;
    max-width: 100%;
    max-height: 300px;
    text-align: center;
    font-size: 18px;
      background-color: aquamarine;
  }
  

}

```

**Habilidades** 

Para los conocimientos técnicos y las soft skills creí que lo mejor era un formato visual, sin texto o con texto animado que fuera sencillo y a la vez claro y que posibilitase un rápido entendimiento del usario. Opte por hacer cuadriculas con grid y pequeñas animaciones en la parte de las soft-kills.

```html
{
 <div class="contenedor_seccion">
          <h2 class="titulo_texto">Mis competencias técnicas</h2>
          <div class="lenguajes_conocidos">
              <div class="lenguaje">
                  <a href="https://www.java.com/es/" target="_blank"><img src="Imagenes\java.jpg"  ></a>
              </div>
              <div class="lenguaje">
                  <a href="https://www.javascript.com/" target="_blank"><img src="Imagenes\js.jpg"></a>
              </div>
              <div class="lenguaje">
                  <a href="https://www.mysql.com/" target="_blank"><img src="Imagenes\MySQL.jpg"></a>
              </div>
              <div class="lenguaje">
                  <a href="https://lenguajecss.com/" target="_blank"><img src="Imagenes\css.jpg"></a>
              </div>
              <div class="lenguaje">
                  <a href="https://developer.mozilla.org/es/docs/Web/HTML" target="_blank"><img src="Imagenes\html.jpg"></a>
              </div>
              <div class="lenguaje">
                  <a href="https://es.wikipedia.org/wiki/C_Sharp" target="_blank"><img src="Imagenes\Csharp_Logo.jpg"></a>
              </div>
          </div>
      </div>


}
```

```css
{

 .lenguajes_conocidos{
     display: grid;
      grid-template-columns: repeat(3,1fr);
      grid-template-rows: repeat(2, 1fr);
      padding: 30px;
      background-color: aquamarine;
  }
  .lenguaje{
    margin: 30px;

  }

  .softskills{
    display: grid;
      grid-template-columns: repeat(2,1fr);
      grid-template-rows: repeat(2, 1fr);
      padding: 30px;
      background-color: aquamarine;
  }

  .skill{

    margin: 30px;

     #escritura1{
    display: block;
    font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    font-size: 30px;
    white-space: nowrap;
    border-right: 4px solid;
    width: 30ch;

    animation: maquina_escribir 2s steps(30), cursor .5s infinite step-end alternate ;
    overflow: hidden;
}

@keyframes maquina_escribir{
    from{
        width: 0;
    }




  }


}

```

tratando que el diseño de la página fuera lo más responsive posible y, obviamente, media queries en todas las páginas de la web.

```css
{

@media only screen and (max-width: 900px) {

    .formacion{
      flex-direction: column;
      max-height: 100%;
      max-width: 100%;
    }

    .lenguajes_conocidos{
      grid-template-columns: repeat(2,1fr);
      grid-template-rows: repeat(3, 1fr);
    }

    .softskills{
      display: grid;
        grid-template-columns: repeat(1,1fr);
        grid-template-rows: repeat(4, 1fr);
    }
    
  }

 @media only screen and (max-width: 600px) {


    .lenguajes_conocidos{
      grid-template-columns: repeat(1,1fr);
      grid-template-rows: repeat(6, 1fr);
    }

    .softskills{
      font-size: 20px;
    }
    
  }



}
```

**TRABAJOS** 

Para la parte de trabajos creí que lo más conveniente era darle uniformidad a la web así que propuse el mismo encabezado con una imagen para luego subdivir la página en dos bloques, esos bloques estarían destinados a pequeños proyectos de apredizaje en el caso del primero y, en el caso del segundo, a los proyectos más grandes, como este mismo.


![Primera página de la web!](/Portfolio-\diseño1.jpg "Segunda página de la web")


```html
{
 <h2 class="titulo_texto">Pequeños trabajos de formación</h2>
        <div class="trabajos">
            <div class="pequeños_trabajos">
                <img src="Imagenes\javabasesdedatos.jpg">
                <p>Conexiones SQL <br> con Java</p>
            </div>
            <div class="pequeños_trabajos">
              <img src="Imagenes\cssyhtmlanimaciones.jpg">
                <p>CSS Y HTML <br>para hacer transiciones</p>
            </div>
            <div class="pequeños_trabajos">
                <img src="Imagenes\procedimientosbasesdedatos.jpg" >
                <p>Procedimientos y funciones <br> SQL sobre base de datos</p>
            </div>
        </div>
    </div>
    <div class="contenedor_seccion">
      <h2>PROYECTOS MAYORES</h2>
      
      <div class="info_imagenes">
        <h3>Calculadora usando JS, CSS y HTML</h3>
      </div>
      <div class="imagenes_grandes">
          
        <a href="https://github.com/fabiovigo/Calculadora.git" target="_blank"><img src="Imagenes\calculadora.jpg"></a>
        <a href="https://github.com/fabiovigo/Calculadora.git" target="_blank"><img src="Imagenes\codigocalculadora.jpg"></a>

      </div>

}
```

Para organizar estos bloques de nuevo utilizamos grid sobre todo y también algo de flex en los algunos casos.

```css
{

.trabajos{
  padding-top: 30px;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  max-width: 100%;
  text-align: center;
  font-size: 18px;
  background-color: rgb(2, 192, 128);
}


.pequeños_trabajos{
display: flex;
flex-direction: column-reverse;
justify-content: center;
align-items: center;
background-color: rgb(2, 192, 128);
}



.imagenes_grandes{
  padding-top: 30px;
  padding-bottom: 30px;
  display: flex;
  justify-content: space-between;
 
}



}
```

La idea fundamental radicaba en que hubiera un desarrollo incremental a lo largo de la página de la complejidad de los trabajos mostrados para que, el el futuro, estos puedan ser sustitudos por otros de mayor complejidad que puedan seguir este patrón.

**CONTACTO*

La página de contacto tenía que ser la más simple de todas, sobre el diseño original, que se presentaba así:

![Primera página de la web!](/Portfolio-\diseño3.jpg "Primera página de la web")

Se decidió incluir de nuevo un encabezado de imagen bajo los links al resto de páginas por uniformidad con el resto de la web.

Esta página además, debía destacar por su simpleza, así que obtamos por incluir simplemente tres tarjetas con links incluidos y unos iconos descriptivos ordenadas por flex.

```html
{

    <div class="contenedor_principal">
        <div class="metodos_contacto">
            <div class="metodo">
                <a href="mailto:msshm@hotmail.es" target="_blank"><img src="Imagenes\mail.jpg"></a>
            </div>
            <div class="metodo">
                <a href="tel:+34674237775" target="_blank"><img src="Imagenes\tlf.jpg"></a>

             </div>
            <div class="metodo">
                <a href="https://github.com/MarioSSantu" target="_blank"><img src="Imagenes\github.jpg"></a>
            </div>

        </div>
    </div>



}
```