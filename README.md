# Visor-de-Im-genes
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> 
<html>

<head>
  

<script type="text/javascript">
window.onload = function() { //tras cargar la página ...
visor1=document.getElementById("visor"); //referencia al visor
mititulo=document.getElementById("titulo"); //referencia al pie de foto
}
function mifoto(num) { //cambiar la imagen
         f="foto"+num+".jpg"; //ruta de la nueva imagen
         document.images["fotoVisor"].src=f; //cambiar imagen
         t=document.images["fotos"+num].alt; //texto de pie de foto
         mititulo.innerHTML=t; //cambiar pie de foto
         }
</script>
</head>
<body>
<div id="cabecera">
<h1>Visor de imágenes</h1>
</div>
<div id="menu">
<img src='foto1.jpg' alt='1. Cloro - Bleach.' name='fotos1' onclick="mifoto(1)"/>
<img src='foto2.jpg' alt='2. Desinfectante - Multi-Purpose Cleaner.' name='fotos2' onclick="mifoto(2)"/>
<img src='foto3.jpg' alt='3. Detergente - Detergent.' name='fotos3' onclick="mifoto(3)"/>
<img src='foto4.jpg' alt='4. Desengrasante - Degreaser.' name='fotos4' onclick="mifoto(4)"/>
<img src='foto5.jpg' alt='5. Lava platos - Dishwashing Liquid.' name='fotos5' onclick="mifoto(5)"/>
<img src='foto6.jpg' alt='6. Polvo limpiador - Cleaner.' name='fotos6' onclick="mifoto(6)"/>
</div>
<div id="principal">
<div id="visor">
  <img src='foto1.jpg' alt='1. Cloro - Bleach.' name='fotoVisor'/>
   <div id="titulo">1. Cloro - Bleach.</div>
   </div>
</div>
</body>
</html>
