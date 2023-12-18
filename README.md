# Curso de Transformaciones y Transiciones en CSS

[Github Pages](https://velasco1704.github.io/curso-transformaciones-transiciones-css/)

## Propiedades para crear animaciones con CSS y propiedades animable

- Transform: La propiedad **transform** en CSS permite aplicar transformaciones 2D o 3D a un elemento. Puedes usarla para rotar, escalar, sesgar, trasladar y aplicar otros efectos visuales a un elemento. Algunos valores comunes para esta propiedad son **rotate()**, **scale()**, **skew()**, **translate(),** entre otros. La propiedad **transform-origin** se utiliza para cambiar la posición de los elementos transformados en relación con su origen. Esto puede afectar cómo se aplican las transformaciones.
- Transition: La propiedad **transition** en CSS permite crear transiciones suaves entre diferentes estados de un elemento. Puedes especificar qué propiedades CSS deben tener una transición, la duración de la transición, la función de temporización y el retraso antes de que comience la transición. Por ejemplo, puedes hacer que un elemento cambie de color durante 2 segundos cuando se le aplica un evento de **hover**. La propiedad **transition** es una propiedad abreviada que combina **transition-property,transition-duration, transition-timing-function y transition-delay**.
- Animation: La propiedad **animation** en CSS permite crear animaciones más complejas y controladas. Puedes definir una serie de fotogramas clave **(@keyframes)** que describen cómo debe cambiar un elemento a lo largo del tiempo. Luego, puedes aplicar esa animación a un elemento utilizando la propiedad **animation**. Puedes especificar la duración, el retraso, la función de temporización y otras opciones para controlar la animación. Por ejemplo, puedes hacer que un elemento se mueva de un lado a otro de la pantalla de forma continua. Estas propiedades son muy útiles para agregar interactividad y efectos visuales a tus elementos HTML utilizando CSS. Puedes experimentar con diferentes valores y combinaciones para lograr los efectos deseados.

## Pseudo-clases y pseudo-elementos en las animaciones

### trigger o disparador

Un disparador o trigger es una funcionalidad que se ejecuta de forma automática cuando se realiza una accion.

### Pseudo-clases en las animaciones

Una pseudo-clases CSS es una palabra clave que se añade a los selectores y que especifica un estado especial del elemento seleccionado. Por ejemplo, :hover aplicará un estilo cuando el usuario haga hover sobre el elemento especificado por el selector.

- :link
- :visited
- :hover
- :not
- :nth-child
- :focus
- :active
- :disabled

### Pseudo-elementos en las animaciones

Al igual que las pseudo-classes, los pseudo-elementos se añaden a los selectores, pero en cambio, no describen un estado especial sino que, permiten añadir estilos a una parte concreta del documento. Por ejemplo, el pseudoelemento ::first-line selecciona solo la primera línea del elemento especificado por el selector.

- ::after
- ::before

## Timing functions, planos y ejes

Las funciones de temporización (timing functions) en CSS se utilizan para controlar cómo se realiza una transición o animación a lo largo del tiempo. Estas funciones definen la aceleración o desaceleración de una propiedad a medida que cambia de un estado a otro. Algunos ejemplos de funciones de temporización comunes son **ease, linear, ease-in, ease-out y ease-in-out**. Estas funciones se pueden aplicar a las propiedades **transition-timing-function y animation-timing-function** para controlar la velocidad y la suavidad de las transiciones y animaciones.

Los planos y ejes se refieren a la representación espacial de los elementos en una escena. En CSS, los planos y ejes se utilizan en combinación con las transformaciones 2D y 3D para controlar la posición y orientación de los elementos. Los planos se refieren a las dimensiones en las que se mueven los elementos, como el plano XY o el plano XZ. Los ejes, por otro lado, se refieren a las direcciones en las que se mueven los elementos, como el eje X, el eje Y y el eje Z. Al utilizar transformaciones 2D o 3D, puedes especificar los planos y ejes en los que deseas que se realicen las transformaciones, lo que te permite controlar la posición, rotación y escala de los elementos en una escena.

## Transform Translate

**Transform translate** es una combinación de dos propiedades CSS que se utilizan para modificar la posición y la apariencia de un elemento en una página web.

La propiedad **transform** se utiliza para aplicar transformaciones 2D o 3D a un elemento, como rotación, escala, sesgado y traslación. La transformación de traslación se utiliza para mover un elemento a lo largo de los ejes X, Y y Z.

Por otro lado, la propiedad **translate** se utiliza junto con la propiedad **transform** para especificar la cantidad de traslación que se debe aplicar a un elemento. La función translate() toma dos o tres valores, que representan las distancias de traslación en los ejes X, Y y Z. Si se especifica solo un valor, se asume que es la distancia de traslación en el eje X.

```css
.elemento {
  transform: translate(100px, 50px);
}
```

## Transform rotate

La propiedad CSS **transform rotate** se utiliza para aplicar una rotación a un elemento en una página web. Permite girar un elemento en sentido horario o antihorario alrededor de un punto de referencia. Se especifica el ángulo de rotación en grados, donde un valor positivo indica una rotación en sentido horario y un valor negativo indica una rotación en sentido antihorario. Por ejemplo, **transform: rotate(45deg)** giraría el elemento 45 grados en sentido horario.

```css
.rotar {
  transform: rotate(30deg);
}
```

## Transform scale

La propiedad CSS **transform scale** se utiliza para aplicar una escala a un elemento en una página web. Permite aumentar o disminuir el tamaño de un elemento en relación con su tamaño original. Se especifica el factor de escala como un número decimal o porcentaje, donde un valor mayor que 1 aumenta el tamaño y un valor menor que 1 lo reduce. Por ejemplo, **transform: scale(1.5)** aumentaría el tamaño del elemento en un 50%.w

```css
.escalar {
  transform: scale(1.5);
}
```

## Transform skew

La propiedad CSS **transform skew** se utiliza para aplicar un sesgado a un elemento en una página web. Permite inclinar o deformar un elemento en los ejes X e Y. Se especifica el ángulo de sesgado en grados, donde un valor positivo inclina hacia la derecha y un valor negativo inclina hacia la izquierda. Por ejemplo, **transform: skew(30deg, -10deg)** sesgaría el elemento 30 grados hacia la derecha en el eje X y 10 grados hacia la izquierda en el eje Y.

```css
.sesgar {
  transform: skew(30deg, -10deg);
}
```

## Transform matrix

La propiedad CSS **transform matrix** se utiliza para aplicar una transformación 2D arbitraria a un elemento en una página web. Permite combinar múltiples transformaciones, como rotación, escala, sesgado y traslación, en una sola matriz de transformación. Se especifican los valores de la matriz en una función **matrix()**, que consta de 6 valores numéricos separados por comas. Cada valor de la matriz representa una transformación específica. Esta propiedad es más compleja de utilizar que las anteriores, ya que requiere conocimientos matemáticos y una comprensión más profunda de las transformaciones 2D.

```css
.matriz {
  transform: matrix(1, 0.5, -0.5, 1, 100, 50);
}
```

Es importante tener en cuenta que todas estas propiedades de transformación **(rotate, scale, skew y matrix)** afectan la apariencia visual de un elemento, pero no cambian su posición real en el flujo del documento.

## Transform origin

La propiedad CSS **transform-origin** se utiliza para establecer el punto de origen de una transformación aplicada a un elemento en una página web. Define el punto de referencia alrededor del cual se realiza la transformación, como la rotación, escala o sesgado.

```css
.transformar {
  transform-origin: top left;
}
```

En este ejemplo, se establece el punto de origen de la transformación en la esquina superior izquierda del elemento. Esto significa que cualquier transformación aplicada, como una rotación, se realizará alrededor de ese punto de origen.

Es importante tener en cuenta que el valor por defecto de **transform-origin** es **center**, lo que significa que la transformación se aplicará alrededor del centro del elemento.

## Transform style

La propiedad CSS **transform-style** establece cómo se renderizan los elementos hijos de un elemento 3D cuando se aplica una transformación 3D a este último. Los valores que puede tomar son **flat** (plano) y **preserve-3d** (preservar 3D).

```css
.padre {
  transform-style: preserve-3d;
}
```

Con el valor **preserve-3d**, los elementos hijos seguirán las transformaciones 3D aplicadas al elemento padre y se renderizarán en 3D. Con el valor **flat**, los elementos hijos ignorarán las transformaciones 3D y siempre se renderizarán de forma plana.

## Transform perspective

La propiedad CSS **transform-perspective** define la perspectiva 3D de un elemento. Establece la distancia entre el usuario y el plano de proyección, lo que determina qué tan aplastados o alargados se verán los elementos 3D.

```css
.elemento {
  transform: perspective(500px);
}
```

Cuanto mayor sea el valor, más plano se verá el elemento. Un valor pequeño lo hará parecer más alargado.

## Backface visibility

La propiedad CSS **backface-visibility** se utiliza para controlar la visibilidad de la cara posterior de un elemento cuando se aplica una transformación 3D, como una rotación, a dicho elemento.

```css
.rotar {
  transform: rotateY(180deg);
  backface-visibility: hidden;
}
```

En este ejemplo, se aplica una rotación de 180 grados al elemento en el eje Y, lo que lo girará completamente. La propiedad **backface-visibility** se establece en **hidden**, lo que significa que la cara posterior del elemento no será visible durante la rotación.

Es importante tener en cuenta que la propiedad **backface-visibility** solo tiene efecto en elementos que tienen una transformación 3D aplicada. Si no se aplica ninguna transformación 3D, esta propiedad no tendrá ningún efecto visible.

## Efecto Parallax

[Parallax Example](https://velasco1704.github.io/parallax-effect/)

El efecto parallax es una técnica utilizada en diseño y desarrollo web para crear una sensación de profundidad y movimiento en una página. Se logra al mover diferentes elementos de la página a diferentes velocidades mientras el usuario se desplaza por ella. Esto crea una ilusión de profundidad y añade un aspecto dinámico a la experiencia de navegación.

### Cómo funciona el efecto parallax

El efecto parallax se basa en la idea de que los objetos cercanos al observador se mueven más rápido que los objetos más alejados. En el contexto del diseño web, esto se logra al dividir la página en capas o secciones y moverlas a diferentes velocidades mientras el usuario se desplaza hacia abajo.

Cuando el usuario se desplaza, las capas más cercanas al frente se mueven más rápido que las capas más alejadas, creando una sensación de profundidad y movimiento. Esto se logra mediante el uso de propiedades CSS como **background-position, transform y transition**, así como también mediante el uso de JavaScript para controlar el comportamiento del efecto.

### Aplicación del efecto parallax

El efecto parallax se puede aplicar de diferentes maneras en el diseño web. Algunos ejemplos comunes incluyen:

- **Fondos de pantalla**: Se puede aplicar el efecto parallax a los fondos de pantalla de una página web para crear una sensación de profundidad y movimiento.

- **Imágenes y videos**: El efecto parallax también se puede aplicar a imágenes y videos para crear una experiencia visual más dinámica.

- **Secciones desplazables**: Algunas páginas web utilizan el efecto parallax en secciones específicas, como encabezados o secciones de presentación, para captar la atención del usuario y crear un efecto visual impactante.

## Transition timing function

Las funciones de temporización, también conocidas como timing functions en inglés, son utilizadas en animaciones y transiciones en el desarrollo web para controlar la velocidad y el ritmo de cambio de una propiedad CSS a lo largo del tiempo. Estas funciones permiten crear efectos de aceleración, desaceleración y cambios de velocidad en las animaciones, lo que añade dinamismo y fluidez a la experiencia del usuario.

### Funcionamiento de las funciones de temporización

Las funciones de temporización se aplican a las transiciones y animaciones CSS utilizando la propiedad transition-timing-function o animation-timing-function. Estas funciones definen cómo cambia una propiedad CSS a medida que avanza en el tiempo.

Existen diferentes tipos de funciones de temporización, cada una con su propio comportamiento:

- **Linear**: Esta función de temporización produce un cambio constante y uniforme a lo largo del tiempo. No hay aceleración ni desaceleración, lo que resulta en una animación lineal y constante.

- **Ease**: Esta función de temporización produce una aceleración gradual al principio y una desaceleración gradual al final de la animación. Es la función de temporización predeterminada en muchas animaciones y transiciones.

- **Ease-in**: Esta función de temporización produce una aceleración gradual al principio de la animación, lo que significa que la animación comienza lentamente y luego se acelera.

- **Ease-out**: Esta función de temporización produce una desaceleración gradual al final de la animación, lo que significa que la animación comienza rápidamente y luego se desacelera.

- **Ease-in-out**: Esta función de temporización combina las características de las funciones Ease-in y Ease-out. La animación comienza lentamente, se acelera en el medio y luego se desacelera al final.

Además de estas funciones de temporización básicas, también es posible crear funciones de temporización personalizadas utilizando la función cubic-bezier(). Esta función permite definir puntos de control para crear curvas de aceleración y desaceleración más complejas.

## Finalize este curso en 4h
