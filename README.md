PROYECTO-SHOP

La pagina esta dividida por 7 carpetas de las cuales vamos a utilizar 3

css: en la cual se almacenan todos los archivos css encargados de darle formato forma y color a la pagina

images: en esta se almacenan todas las imágenes utilizadas en la pagina ( estan oresdenas por numeros; tablet1.1 tablet1.2)

phones: en esta se almacenan todos los html utilizados en la pagina 

las paginas estan divididas d manera horizontal por medio de seccion con las clases conten content

en la carpeta phones hay dos tipos de html, los que dirigen a un producto en especifico y los que mandan al catalogo 

los archivos iphone portial-1 tablet-1 y mouse-1 dirigen a un producto en especifico con sus detalles 

los archivos accesorios catalogo portatiles y tablest dirigen al stock general de dicha categoría

el index es el unico archivo html que no esta suelto.

 la barra superior que tiene las opciones de ( catalogo quienes somos y contáctenos ) usa un float:left para permitir que esta baje junto con la pagina sin generar inconvenientes.

```
.navbar {
    display: flex;
    justify-content: space-between;
    list-style: none;
    background: #121212;
    color: white;
    position: fixed;
    height: 30px;
    width: 100%;
    align-items: center;
}

.navbar-menu{
    background-color:#121212;
    overflow: hidden;
    width: 80%;
    height: 100%;
    justify-content: space-between;
}

.navbar-menu a{
    float: left;
    display: flex;
    color: #f9f9f9;
    text-align: center;
    text-decoration: none;
    align-items: center;
    font: 16px;
    height: 100%;
    width: 25%;
}

.navbar-menu a:hover {
    background-color: #313131;
}

.navbar-menu .icon {
    display: none;
}

```

codigo de la barra.

```
.phones{
  background: #F6F6F6;
  margin-top: 25px;
  height: 31rem;
  width: 91%;/**/
}
.produto-phone{
    display: flex;
    flex-direction: column;
    justify-content: center;
    width:45%;/**/
    margin-left: 2%;
}
.phone{
    display: flex;
    justify-content:flex-start;
    height:10rem;
    width: relative;
    margin-left: 20px;
}
.phone-clone1{
  height:15rem;
  width: relative;
  margin-left: -190px;
  margin-top: 118px
}
.phone-clone2{
  height:15rem;
  width: relative;
  margin-left: -190px;
  margin-top: -40px;

}
.phone-clone3{
  height:15rem;
  width: relative;
  margin-top: -200px;
}
.telefonos-aparecer{
    border:none;
    cursor: pointer; 
}
.contenedor-imagen {
    display: flex;
    position: relative;
    justify-content: flex-start;
    gap:28px
}
.imagen-original,
.imagen-duplicada {
    cursor: pointer;
    transition: transform 0.3s ease;  
    opacity: 0.5; 
    filter: blur(1px);
}
.imagen-duplicada {
    position: absolute;
    top: 0;
    opacity: 0;
    margin-left: 150px;
}
.contenedor-imagen:hover .imagen-original {
    transform: scale(1);
    opacity: 1;
    filter: blur(0px);
}
.contenedor-imagen:hover .imagen-duplicada {
    opacity: 1;
    left: calc(100% + 10px); /* Ajusta la distancia entre las imágenes según tus preferencias */
    transform: scale(2);
    filter: blur(0px);
    width: auto;
   
   
}
  /* Estilos para el checkbox (oculto) */

input[type="checkbox"] {
    display: none;
}
.caracteristicas-phone{
  display: flex;
  flex-direction:column;
  align-content: flex-start;
  margin-left: 0;
}
.contorno{
  border: #121212 1px solid;
  border-radius: 7px;
  height: 100px;
}
```

con este código se  ajusta la apracion y desaparicion de imágenes en el catalogo 
