https://www.figma.com/file/MnvrTPgZYjfcPCC7nVVHHa/Untitled?node-id=0%3A1


**CONCEPTO BÁSICO DE DISEÑO**

La idea fundamental que manejaba a la hora de diseñar esta web portfolio era que estuviera construida en tres páginas a modo de web empresarial (salvando las distancias). La primera de esas páginas estaría orientada a describirme a mi, mi background, mis habilidades y lenguajes conocidos y simplemente dar unas breves referencias.

El restultado final debería ser algo similar a esto:


![Primera página de la web!](diseño2.jpg "Primera página de la web")

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

Para los conocimientos técnicos y las soft skills creí que lo mejor era un formato visual, sin texto o con texto animado que fuera sencillo y a la vez claro y que posibilitase un rápido entendimiento del usario.