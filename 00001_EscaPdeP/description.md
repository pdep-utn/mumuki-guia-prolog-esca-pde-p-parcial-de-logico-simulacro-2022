<div align="center">
<img src="https://raw.githubusercontent.com/MumukiProject/mumuki-guia-gobstones-pruebas-contenido-mumuki/master/assets/escapdep_1598124676430.png" alt="escapdep_1598124676430.png" width="auto" height="auto">
</div>

_¿Te quedaste sin ideas para hacer en la cuarentena?_ 💤 _Te traemos la salida, o mejor dicho, ¡el escape! Sabemos que quizás no es una novedad_ 😅_, pero te damos la bienvenida a ¡EscaPdeP!_ :woman_running::computer::man_running:_. Un sitio que reúne las mejores salas de escape que existen en la web._

En nuestra base de conocimientos contamos con los siguientes datos de las personas que se crearon una cuenta en nuestra página:

```prolog
%persona(Apodo, Edad, Peculiaridades).
persona(ale, 15, [claustrofobia, cuentasRapidas, amorPorLosPerros]).
persona(agus, 25, [lecturaVeloz, ojoObservador, minuciosidad]).
persona(fran, 30, [fanDeLosComics]).
persona(rolo, 12, []).
```

Hay varias empresas metidas en este rubro y cada una tiene distintas salas:

```prolog
%esSalaDe(NombreSala, Empresa).
esSalaDe(elPayasoExorcista, salSiPuedes).
esSalaDe(socorro, salSiPuedes).
esSalaDe(linternas, elLaberintoso).
esSalaDe(guerrasEstelares, escapepepe).
esSalaDe(fundacionDelMulo, escapepepe).
```

Las salas no son todas iguales. Contamos con las siguientes experiencias:

```prolog
%terrorifica(CantidadDeSustos, EdadMinima).
%familiar(Tematica, CantidadDeHabitaciones).
%enigmatica(Candados).

%sala(Nombre, Experiencia).
sala(elPayasoExorcista, terrorifica(100, 18)).
sala(socorro, terrorifica(20, 12)).
sala(linternas, familiar(comics, 5)).
sala(guerrasEstelares, familiar(futurista, 7)).
sala(fundacionDelMulo, enigmatica([combinacionAlfanumerica, deLlave, deBoton])).
```

Hacé los siguientes predicados teniendo en cuenta que deben ser **totalmente inversibles**.

1. **_nivelDeDificultadDeLaSala/2_**: para cada **sala** nos dice su **dificultad**. Para las salas de experiencia terrorífica el nivel de dificultad es la cantidad de sustos menos la edad mínima para ingresar. Para las de experiencia familiar es 15 si es de una temática futurista y para cualquier otra temática es la cantidad de habitaciones. El de las enigmáticas es la cantidad de candados que tenga.

2. _**puedeSalir/2**_: una **persona** puede salir de una **sala** si la dificultad de la sala es 1 o si tiene más de 13 años y la dificultad es menor a 5. En ambos casos la persona no debe ser claustrofóbica.

3. _**tieneSuerte/2**_: una **persona** tiene suerte en una **sala** si puede salir de ella aún sin tener ninguna peculiaridad.

4. _**esMacabra/1**_: una **empresa** es macabra si todas sus salas son de experiencia terrorífica.

5. _**empresaCopada/1**_: una **empresa** es copada si no es macabra y el promedio de dificultad de sus salas es menor a 4.

6. ¡Cada vez hay más salas y empresas! Conozcámoslas para agregarlas a nuestro sistema:
  * La empresa supercelula es dueña de salas de escape familiares ambientadas en videojuegos. La sala estrellasDePelea cuenta con 7 habitaciones pero lamentablemente no sabemos la cantidad que tiene su nueva sala choqueDeLaRealeza.
  * La empresa SKPista (fanática de un famoso escritor) es la dueña de una única sala terrorífica para mayores de 21 llamada miseriaDeLaNoche que nos asegura 150 sustos.
  * La nueva empresa que se suma a esta gran familia es Vertigo, pero aún no cuenta con salas.

**También podés ver el examen desde [acá](https://docs.google.com/document/d/1toV71CIEeJSfQeK9JDcpgR-FK41C0RDH5zEtQGjkQQk/edit?usp=sharing).**



