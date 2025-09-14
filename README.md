# 00054621_practica3_secci-n1
Laboratorio no.3 Programación Web

¿Porqué cambia el posicionamiento de las cajas internas al div principal?, ¿Qué pasa si me solicitan hacer
un cambio en el orden de los elementos pero sin tocar los archivos html y js, será que puedo lograrlo a traves de CSS?.
R// es debido a que usamos flexbox column en CSS, si es posible lograrlo a traves de CSS, se puede alterando el CSS con flex ya sea row o row-reverse y column o column-reverse.

¿Qué hacen estás propiedades?
R// .box es un contenedor flex en fila que envuelve sus hijos si no caben. Cada div dentro ocupa 33% de ancho, con estilos visuales, pero el primero ocupa 64%, logrando un diseño donde el primer bloque es más grande y los demás más pequeños.

.box{
    display: flex;
    background-color: var(--pink);
    flex-direction: row;
    flex-wrap: wrap;
}

.box div{
    flex-grow: 4;
    margin: 10px 5px;
    border-radius: 8px;
    padding: 5px;
    background-color: var(--blue);
    width: 33%;
}

/*agregamos*/
.box div:first-child{
    width: 64%;
}

¿Puedo diseñar toda mi web usando GRID? Porqué se
dan estos cambios entre tan pocas líneas de diseño CSS.
R// Sí, yo puedo diseñar toda mi web con Grid. La razón de que logre tantos cambios en tan pocas líneas es que Grid me permite definir el esqueleto de la página de forma declarativa y flexible, ahorrando muchísimo código en comparación con los métodos antiguos.
