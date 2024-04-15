# Sistema Electoral para la Cámara Baja en América Latina y sus Reformas

Bienvenidos/as al repositorio GitHub de la base de datos "Sistema Electoral para la Cámara Alta en América Latina y sus Reformas", mantenida por integrantes del Observatorio de Reformas Políticas en América Latina.

## Contenidos

-   [Resumen](#resumen)
-   [Descripción](#descripción)
-   [Citado](#citado)

## Resumen

La base de datos contiene información sobre las reformas electorales a la normativa que regula el sistema electoral de las cámaras altas nacionales de diez países de América Latina. En la base de datos hay información sobre las modificaciones en el principio de representación que sigue la Cámara Alta (principio de representación), la fórmula electoral que se aplica (fórmula electoral) y en caso de ser mixta, se especifica la segunda fórmula electoral aplicada (y, de ser el caso, la tercera), el número de miembros que se establece para la Cámara (miembros cámara), el número de distritos electorales (distritos electorales) y su tamaño, la estructura del voto que establece la reforma electoral para la cámara alta (estructura de voto), los años de mandato de cada funcionario (mandato), si hay existencia de barreras legales (barrera legal), si se permite la reelección legislativa (reelección legislativa) y, por último, si existe el mecanismo de revocatoria de mandato (revocatoria legislativa).

La revisión de la normatividad se realizó a partir del año de la transición a la democracia de cada país, con base en lo planteado por Alcántara; Páramo; Freidenberg y Déniz (2006). En el caso de los países con procesos de cambio político graduales, se utiliza como base el año de inicio de la tercera ola de la democracia en América Latina (Huntington, 1991).

Integrantes del Observatorio de Reformas Políticas en América Latina recopilaron y codificaron la información. Las personas responsables de la recopilación de los datos son Flavia Freidenberg (Instituto de Investigaciones Jurídicas); Karolina Monika Gilas (Facultad de Ciencias Políticas y Sociales, UNAM) y María José Lorenzo Montalvo (Facultad de Ciencias Políticas y Sociales, UNAM), mientras que las personas responsables de la codificación de los datos son Karolina Gilas (Facultad de Ciencias Políticas y Sociales, UNAM) y María José Lorenzo Montalvo (Facultad de Ciencias Políticas y Sociales, UNAM)

## Descripción

El directorio `./Data/` contiene el archivo `./Data/DD_SECA` en el cual se encuentra toda la información relevante respecto a la base de datos del sistema electoral de la Cámara Alta y sus reformas. En específico, la base de datos se compone de las siguientes variables:

-   `país`: nombre del país en el cual se llevó a cabo la reforma al régimen electoral de la cámara baja en América Latina.

-   `cowcode`: código del país de acuerdo con la codificación de “Correlates of War”
https://correlatesofwar.org/data-sets/cow-country-codes.

-   `siglas_pais`: siglas del país de acuerdo con el código de tres letras ISO (por ejemplo: ARG, MEX, SAL) disponible en: http://utils.mucattu.com/iso_3166-1.html 

-   `consec_reforma_pais`: registra el número consecutivo de las reformas al régimen electoral de la cámara baja en cada país de América Latina. Ejemplo: Peru_1 Peru_2, Peru_3, Peru_4.

-   `año`: año calendario al que corresponde la reforma al régimen electoral de la cámara baja en cada país de América Latina entre 1949-2023.

-   `principio_representacion`: indica el principio de representación política que rige la elección de los miembros de la cámara baja nacional del poder legislativo nacional en cada país. Sus valores son [1]: Mayoritario [2]: Proporcional; [3]: Mixto; [4]: Mayoritario con representación de la minoría.

-   `form_elec_01`: indica la fórmula electoral que se aplica para la ocupación de escaños. Sus valores son [1]: Cifra repartidora; [2]: D’Hondt; [3]: Cociente o residuo electoral; [4]: Hare y restos mayores; [5] Hare modificada;[6]: Imperiali corregido; [7]: Factor ponderado; [8]: Webster; [9]: Hagenbanch-Bischoff; [10]: Sistema proporcional integral; [11]: Mayoría absoluta; [12]: Mayoría relativa; [13]: Mayoría; [99]: No aplica

-   `form_elec_02`: en caso de que el sistema de elección sea mixto, indica la segunda fórmula electoral que se aplica para la ocupación de escaños. Sus valores son [1]: Cifra repartidora; [2]: D ́Hondt; [3]: Cociente o residuo electoral; [4]: Hare y restos mayores; [5] Hare modificada; [6]: Imperiali corregido; [7]: Factor ponderado; [8]: Webster; [9]: Hagenbanch-Bischoff; [10]: Sistema proporcional integral; [11]: Mayoría absoluta; [12]: Mayoría relativa; [13]: Mayoría; [99]: No aplica

-   `m_camara`: indica el número de escaños que la reforma electoral establece para la cámara alta del poder legislativo nacional.

-   `distr_elec`: indica el número de distritos electorales que eligen a representantes.

-   `elecc_distr__01`: indica el tamaño de distritos en los que se divide el territorio para la elección de la cámara alta. Sus valores son [1]: Uninominal; [2]: Binomial; [3]: Trinomial; [4]: Cuatrinominal; [5]: Pentanominal; [6]: Nacional; [7]: Especial; [99]: No aplica

-   `elecc_distr__02`: en caso de que haya más de un tipo de elección, indica el tamaño de distritos en los que se divide el territorio para la elección de la cámara alta bajo la segunda fórmula electoral. Sus valores son [1]: Uninominal; [2]: Binomial; [3]: Trinomial; [4]: Cuatrinominal; [5]: Pentanominal; [6]: Nacional; [7]: Especial; [99]: No aplica

-   `elecc_distr__03`: en caso de que se aplique más de dos fórmulas electorales, indica el tamaño de distritos en los que se divide el territorio para la elección de la cámara alta bajo la tercera fórmula electoral. Sus valores son [5]: Pentanominal y [99]: No aplica.

-   `estr_voto_01`: indica el tipo de la estructura del voto que establece la reforma electoral dentro de la cámara alta. Sus valores son [1]: Candidatura uninominal; [2]: Lista cerrada y bloqueada; [3]: Lista cerrada y no bloqueada; [4]: Lista cerrada, no bloqueada y voto preferencial doble; [5]: Lista cerrada, no bloqueada y voto preferencial y opcional; [6]: Lista abierta; [7]: Lista abierta y voto preferente; [8]: Lista única vinculada a candidatura presidencial; [9]: Voto preferente; [10]: Doble voto simultáneo; [11]: Doble voto preferencial opcional; [12]: Voto por un candidato en listas de partido; [13]: Mixto.

-   `estr_voto_02`: en caso de haber una estructura mixta, se indica el segundo tipo de estructura del voto que establece la reforma electoral dentro de la cámara alta. Sus valores son [1]: Candidatura uninominal; [2]: Lista cerrada y bloqueada; [3]: Lista cerrada y no bloqueada; [4]: Lista cerrada, no bloqueada y voto preferencial doble; [5]: Lista cerrada, no bloqueada y voto preferencial y opcional; [6]: Lista abierta; [7]: Lista abierta y voto preferente; [8]: Lista única vinculada a candidatura presidencial; [9]: Voto preferente; [10]: Doble voto simultáneo; [11]: Doble voto preferencial opcional; [12]: Voto por un candidato en listas de partido; [13]: Mixto.

-   `mandato`: duración de años de mandato que ejercen los funcionarios fijada por la reforma.

-   `barrera_legal`: indica si la reforma electoral plantea la existencia o inexistencia de barreras legales para el acceso de los partidos políticos al reparto de escaños de la cámara alta del poder legislativo nacional. Sus valores son [0]: No específica; [1]: Si específica.

-   `reelección_legis`: indica si hay o no reelección y la manera en que la reforma electoral regula la reelección de los miembros de la cámara alta. Sus valores son  [1]: No reelección; [2]: No reelección inmediata; [3]: Reelección inmediata; [4]: Reelección inmediata e indefinida; [5]: Reelección inmediata por dos períodos;

-   `revoca_legis`: indica si la reforma electoral considera la existencia o inexistencia de la revocación legislativa para los miembros de la cámara alta del poder ejecutivo nacional. Sus valores son No [0]: la normativa no considera la existe de revocación legislativa; Sí [1]: la normativa considera la existe de revocación legislativa.


## Citado

``` r
Freidenberg, Flavia. Dir., 2023, “Sistema electoral para la Cámara Alta en América Latina y sus reformas”, Observatorio de Reformas Políticas en América Latina (1978-2023). Ciudad de México: Instituto de Investigaciones Jurídicas (IIJ-UNAM) y Washington, D.C.: Secretaría para el Fortalecimiento de la Democracia de la Organización de los Estados Americanos (SFD/OEA), V2. DOI: https://doi.org/10.5281/zenodo.8263240
```