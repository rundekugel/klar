# Klar — Reflexiones hacia una lengua mundial

**Versión:** 1.0 · **Fecha:** 06-08-2026
*Libro 1 de una serie planeada: (1) Por qué, (2) Borrador/Especificación, (3) Diccionarios, (4) Experimentos. Este documento explica las razones detrás de las reglas del documento de diseño — para los detalles, véase allí.*

## Historial de cambios

| Versión | Fecha | Cambio |
|---|---|---|
| 1.0 | 06-08-2026 | Primera versión: motivación, contexto histórico, filosofía de diseño, contexto científico (con contraposiciones), preguntas abiertas para el debate |

---

## 1. ¿Por qué otra lengua planificada?

Quien diseña hoy una lengua planificada debe enfrentar un hecho incómodo: ya existen más de 900 intentos documentados de construir una lengua mejor (Okrent 2009). Casi todos han fracasado, medidos según su propia pretensión: convertirse en una lengua vehicular internacional. Tras casi 140 años, el esperanto es la única con una comunidad de hablantes significativa y hablantes nativos reales.

„Klar" no pretende romper este patrón. Su valor está en otro lugar: en el **método** con el que se construye la lengua, y en la pregunta de si con ello se puede aprender algo — sobre el lenguaje, sobre la adquisición del lenguaje, sobre los límites de lo que el diseño puede lograr en absoluto.

## 2. Qué se ha intentado históricamente — y por qué fracasó casi siempre

Se distinguen tres grandes olas de lenguas planificadas (Okrent 2009):

- **Lenguas filosóficas** (s. XVII, p. ej. John Wilkins) querían clasificar el mundo mismo de forma lógica y derivar la lengua directamente de ahí — impresionante como experimento mental, en la práctica de una complejidad inutilizable.
- **Auxlangs esquemáticas** (Volapük 1879, esperanto 1887, ido, interlingua) buscaban una lengua vehicular neutral y fácil de aprender para el intercambio internacional. El esperanto fue el más exitoso de estos intentos — pero su éxito no se debe a una superioridad gramatical. El Volapük tuvo en su momento más seguidores y no se hundió por la lengua en sí, sino por una disputa sobre la autoridad para reformarla.
- **Lenguas lógicas** (Loglan, después Lojban) buscaban una univocidad radical siguiendo el modelo de la lógica formal — con el resultado de que son lingüísticamente muy interesantes, pero demasiado difíciles de aprender para la mayoría de las personas.

„Klar" intenta tomar algo de las tres tradiciones sin repetir la trampa particular de cada una: la regularidad de las auxlangs, la univocidad de las lenguas lógicas — pero limitada a lo que un niño puede aprender de forma incidental (véase el documento de diseño, principios 1–4).

## 3. La verdadera decisión de diseño: método en lugar de intuición

La mayoría de las lenguas planificadas históricas surgieron de la pluma de una sola persona, a menudo en un tiempo relativamente corto, y solo después fueron puestas a prueba en la realidad (si es que llegaron a serlo). „Klar" invierte deliberadamente ese orden — cada regla se comprobó contra frases de ejemplo reales antes de considerarse „terminada" (documento de diseño, sección 1a), y un script de validación automatizado impide que las palabras nuevas violen sin ser detectadas la fonotáctica propia o la ausencia de colisiones (sección 7.1).

Esto no es un dogma de diseño lingüístico, sino simplemente el traslado de un método de la ingeniería de software (pruebas iterativas, comprobación automática de regresiones) a un campo que tradicionalmente se ha tratado de forma más intuitiva. Si esto conduce finalmente a una lengua *mejor* está por ver — lo único seguro es que conduce a una más *trazable*: cada regla se puede remontar a un caso de prueba concreto, no solo al gusto personal.

## 4. Contexto científico — y las contraposiciones

Para que este proyecto no se quede en pura especulación, algunas decisiones de diseño se apoyan en investigación existente. Es importante aportar también la crítica a estas teorías — nada de esto está exento de controversia:

**Hipótesis del bioprograma (Bickerton 1981, *Roots of Language*).** Las lenguas criollas, que surgen de un input pidgin fuertemente simplificado, muestran en todo el mundo rasgos gramaticales llamativamente similares (orden SVO fijo, marcación preverbal de tiempo/modo). La tesis de Bickerton: los niños completan la estructura faltante a partir de un „bioprograma" innato. „Klar" comparte algunos de estos rasgos (documento de diseño, 1b) — no porque consideremos probada la hipótesis, sino porque la coincidencia es al menos un indicio. **Contraposición:** Michel DeGraff ha criticado duramente esta forma de „excepcionalismo criollo" (DeGraff 1999, 2005) — en su opinión, las lenguas criollas no se diferencian gramaticalmente de forma fundamental de otras lenguas surgidas naturalmente, y la supuesta similitud sería en parte ideología colonial y no un hallazgo neutral. Este debate sigue sin resolverse.

**Código de frecuencia (Ohala 1983, 1984).** Un tono de voz agudo se asocia interlingüísticamente con pequeñez, ausencia de amenaza y cortesía; un tono grave, con dominancia — derivado de la correlación entre el tamaño corporal y el tono de voz en muchas especies animales. En esto se apoya la regla de entonación de la sección 5.7 del borrador. El modelo de Ohala es influyente, pero también aquí hay crítica sobre su alcance empírico (p. ej. Grawunder & Winter, que cuestionan algunas de las correlaciones propuestas).

**Efecto propedéutico del esperanto.** Varios estudios independientes (entre otros Szerdahelyi en Hungría en los años 1960; el proyecto *Springboard to Languages* de la Universidad de Manchester, aprox. 2005–2011) encontraron indicios de que aprender esperanto primero acelera la adquisición posterior de otras lenguas extranjeras — presumiblemente porque su gramática regular desarrolla tempranamente una conciencia metalingüística. Si esto se confirma, sería un argumento a favor de que una lengua *aún* más regular y deliberadamente pensada para niños, como „Klar", podría tener un efecto similar o mayor — por ahora pura especulación, sin comprobar.

## 5. Preguntas abiertas para el debate

Estos puntos se dejan deliberadamente sin resolver — deben invitar a la contradicción y a la experimentación propia, no a la aceptación silenciosa:

1. **¿Puede la calidad del diseño generar difusión por sí sola?** La evidencia histórica habla en contra (esperanto vs. efectos de red, véase documento de diseño, capítulo 8). ¿Tiene sentido entonces „construir una lengua mejor" como objetivo del proyecto — o solo se justifica como ganancia de conocimiento, independientemente de su difusión?
2. **¿Doble negación como redundancia o como lastre?** Las lenguas criollas la usan a menudo; „Klar" por ahora no. ¿Sería una mejora real de la robustez frente a errores, o solo una complicación innecesaria que contradice el propio principio de minimalismo (punto abierto, documento de diseño, capítulo 9)?
3. **¿Cuánto de la semejanza criolla es casualidad?** Ante la crítica de DeGraff: ¿son los paralelismos estructurales entre „Klar" y las lenguas criollas un indicio de preferencias infantiles de aprendizaje — o simplemente lo que ocurre cuando *cualquiera* simplifica radicalmente, independientemente de la cognición?
4. **¿Justifica la „robustez de canal" (susurro, limitaciones articulatorias) un nicho lingüístico propio?** Ninguna gran auxlang lo ha perseguido deliberadamente hasta ahora. ¿Es una laguna real — o un problema de nicho que no justifica el esfuerzo de una lengua entera?
5. **¿Qué significaría siquiera que „Klar" „funcione"?** El esperanto mide el éxito por el número de hablantes. Si la difusión explícitamente no es el objetivo (véase el punto 1) — ¿en qué se mediría entonces el éxito de este experimento?

## 6. Invitación

En su forma actual, „Klar" es una herramienta para reflexionar sobre el lenguaje, no en primer lugar un medio de comunicación. Su valor surge de la experimentación — formar frases con las que la gramática roza, escribir poemas en los que la acentuación tropieza, inventar palabras que el script de validación rechaza. Cada quiebre encontrado es más interesante que cualquier regla confirmada.

---

## Referencias

- Bickerton, Derek (1981). *Roots of Language*. Ann Arbor: Karoma Press.
- DeGraff, Michel (1999, 2005). Crítica al „excepcionalismo criollo" — entre otros en: *Language Creation and Language Change: Creolization, Diachrony, and Development* (ed. DeGraff), MIT Press.
- Ohala, John J. (1983). Cross-language use of pitch: An ethological view. *Phonetica* 40, 1–18.
- Ohala, John J. (1984). An ethological perspective on common cross-language utilization of F0 of voice. *Phonetica* 41, 1–16.
- Okrent, Arika (2009). *In the Land of Invented Languages*. Nueva York: Spiegel & Grau.
- Roehr-Brackin, K. / Tellier, A. et al. Resultados del proyecto *Springboard to Languages*, Universidad de Manchester (aprox. 2005–2012).
- Szerdahelyi, István (años 1960). Estudio comparativo húngaro sobre el efecto propedéutico del esperanto, Universidad de Budapest.

*Nota: Estos datos provienen de la investigación realizada durante esta conversación y deberían verificarse contra las fuentes originales antes de una publicación real (número exacto de páginas, posibles ediciones posteriores).*
