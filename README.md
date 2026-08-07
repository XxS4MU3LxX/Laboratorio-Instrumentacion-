## Laboratorio_1_Monitoreo del patrón y frecuencia respiratoria 
# **Integrantes**
>
* María Angélica Vargas Saldaña
* Samuel Esteban Fonseca Luna
* Laura Daniela Triana Molano

<h2 align="center">𝙞𝙣𝙩𝙧𝙤𝙙𝙪𝙘𝙘𝙞ó𝙣</h2>
En este laboratorio se analizó el patrón y la frecuencia respiratoria mediante la adquisición de una señal biológica usando un sensor mq135 y adq. Posteriormente, la señal se procesó en MATLAB para observar su comportamiento en el tiempo y la frecuencia, comparando condiciones de reposo y habla. Esta práctica brinda una base teórica y aplicada sobre el monitoreo respiratorio, permitiendo comprender su relevancia dentro de la instrumentación biomédica y su utilidad en contextos reales de evaluación fisiológica.

<h2 align="center">𝙤𝙗𝙟𝙚𝙩𝙞𝙫𝙤𝙨</h2>

𝙊𝙗𝙟𝙚𝙩𝙞𝙫𝙤 𝙜𝙚𝙣𝙚𝙧𝙖𝙡: 

Evaluar la influencia del habla o verbalización sobre el patrón respiratorio. 

𝙊𝙗𝙟𝙚𝙩𝙞𝙫𝙤𝙨 𝙀𝙨𝙥𝙚𝙘𝙞́𝙛𝙞𝙘𝙤𝙨:

• Reconocer las variables físicas principalmente involucradas en el proceso respiratorio. 

• Desarrollar un sistema que extraiga el patrón respiratorio y la frecuencia respiratoria. 

• Identificar tareas de verbalización a partir del patrón y/o la frecuencia respiratoria. 

<h1 align="center"><i><b>𝐏𝐚𝐫𝐭𝐞 A 𝐝𝐞𝐥 𝐥𝐚𝐛𝐨𝐫𝐚𝐭𝐨𝐫𝐢𝐨</b></i></h1>


<h2 align="center">𝙋𝙧𝙤𝙘𝙚𝙨𝙤 𝙍𝙚𝙨𝙥𝙞𝙧𝙖𝙩𝙤𝙧𝙞𝙤</h2>

La respiración es un proceso vital para el funcionamiento normal en todos los niveles de organización, desde la célula hasta el organismo. El oxígeno, suministrado por la circulación local a nivel tisular, funciona en la membrana interna mitocondrial como mediador esencial para la liberación de energía. En las mitocondrias, los nutrientes digeridos experimentan reacciones metabólicas, llegan a la cadena de transporte de electrones y liberan compuestos de alta energía (p. ej., trifosfato de adenosina). El principal subproducto de este proceso, el dióxido de carbono, se libera en la sangre venosa y regresa a los pulmones. El dióxido de carbono se difunde a través de las paredes alveolares y se disuelve en el aire exhalado. La frecuencia respiratoria (es decir, el número de respiraciones por minuto) está altamente regulada para que las células produzcan la energía óptima en cualquier momento. Un complejo sistema nervioso de tejidos nerviosos regula la tasa de entrada de oxígeno y la tasa de salida de dióxido de carbono, ajustándola en consecuencia en condiciones que alteran las presiones parciales de los gases en la sangre. La respiración involucra el cerebro, el tronco encefálico, los músculos respiratorios, los pulmones, las vías respiratorias y los vasos sanguíneos. Todas estas estructuras tienen una participación estructural, funcional y reguladora en la respiración.
>
>

<img width="1402" height="1122" alt="image" src="https://github.com/user-attachments/assets/f8e681f5-f74f-4a74-875a-af07e903e475" />
>
>


𝙎𝙚𝙣𝙨𝙤𝙧 𝙚𝙨𝙘𝙤𝙜𝙞𝙙𝙤 
>
Se seleccionó el sensor MQ-135 debido a que es capaz de detectar las variaciones en la concentración de CO₂ presentes en el aire exhalado, generando una señal analógica que permite identificar los ciclos de inspiración y espiración. A partir de estas variaciones es posible extraer el patrón respiratorio y calcular la frecuencia respiratoria.
>
El monitoreo respiratorio alternativo utilizado era la galga extensiométrica, la cual mide de forma indirecta la respiración a través de la expansión y contracción del tórax  Sin embargo, este método requiere el uso de una banda ajustada al cuerpo y su señal puede verse afectada por movimientos del participante, cambios de postura o desplazamientos de la banda durante la adquisición.
>
En comparacion, el MQ-135 mide directamente los cambios en la composición del aire exhalado dentro de la máscara, lo que permite obtener una señal representativa del proceso respiratorio sin depender de la deformación mecánica del tórax. Además, su integración con la máscara de nebulizacion utilizada en el montaje, presenta un bajo costo y proporciona una salida analógica compatible con el DAQ (NI USB-6002), facilitando el procesamiento de la señal en MATLAB.
>
Aunque el sensor no está diseñado como un sensor médico ni permite cuantificar con precisión la concentración de CO₂, su respuesta es suficiente para detectar los cambios periódicos asociados a la respiración. Por ello, se consideró la opción más adecuada para este laboratorio, ya que permite obtener de forma confiable el patrón respiratorio y analizar las modificaciones producidas durante el habla.
>
>
<img width="381" height="492" alt="image" src="https://github.com/user-attachments/assets/b69d795f-27fe-4837-9808-36ea78e3302e" />


𝘾𝙤𝙣𝙨𝙚𝙣𝙩𝙞𝙢𝙞𝙚𝙣𝙩𝙤 𝙞𝙣𝙛𝙤𝙧𝙢𝙖𝙙𝙤 𝙙𝙚𝙡 𝙥𝙖𝙧𝙩𝙞𝙘𝙞𝙥𝙖𝙣𝙩𝙚 

Debido a que la práctica involucró la adquisición de datos fisiológicos mediante el registro de la frecuencia respiratoria utilizando un sensor MQ-135 y una máscara, fue necesario obtener el consentimiento informado del participante. Este documento garantiza que la persona comprendió el objetivo del experimento, el procedimiento a realizar, el uso académico de los datos recolectados y la confidencialidad de la información, asegurando una participación libre y voluntaria de acuerdo con los principios éticos de la investigación.
>
>
<img width="1130" height="1535" alt="image" src="https://github.com/user-attachments/assets/aa444c3b-a480-4891-9a1a-c57afc1d2bf5" />
>

𝙈𝙤𝙣𝙩𝙖𝙟𝙚 𝙚𝙭𝙥𝙚𝙧𝙞𝙢𝙚𝙣𝙩𝙖𝙡

Para la adquisición de la señal respiratoria se implementó un montaje compuesto por un sensor de gases MQ-135, una máscara de oxígeno, una tarjeta de adquisición de datos National Instruments USB-6002 y un computador para el procesamiento de la información.

El sensor MQ-135 se fijó en la parte inferior de la máscara, de manera que quedara expuesto al aire exhalado por el participante. La salida analógica del sensor se conectó a una entrada analógica (AI0) de la tarjeta NI USB-6002, mientras que la alimentación del sensor se realizó mediante una fuente de 5 V y se compartió la referencia de tierra (GND) con la DAQ para garantizar una medición estable.

La tarjeta de adquisición de datos se conectó al computador mediante un cable USB, permitiendo la captura de la señal analógica generada por el sensor. Inicialmente, el correcto funcionamiento del montaje se verificó mediante el panel de pruebas de NI MAX, observando la variación del voltaje producida por los ciclos de inspiración y espiración. Posteriormente, la adquisición de los datos se realizó desde MATLAB para su visualización y posterior análisis de la frecuencia respiratoria.

<img width="1600" height="1517" alt="image" src="https://github.com/user-attachments/assets/d5235421-b084-4b6c-b285-17cefd69981e" />

𝙎𝙚𝙣̃𝙖𝙡 𝙚𝙣 𝙎𝙚𝙧𝙞𝙖𝙡 𝙋𝙡𝙤𝙩𝙩𝙚𝙧 (𝙍𝙚𝙥𝙤𝙨𝙤-𝙃𝙖𝙗𝙡𝙖)

𝙀𝙣 𝙧𝙚𝙥𝙤𝙨𝙤

Durante la respiración normal en reposo:

+ La señal presentó un comportamiento periódico y relativamente estable.

+ Se observaron ciclos regulares correspondientes a inhalación y exhalación.

+ La amplitud fue constante.

+ El conteo manual permitió estimar una frecuencia aproximada de 12 respiraciones por minuto.

𝘿𝙪𝙧𝙖𝙣𝙩𝙚 𝙚𝙡 𝙝𝙖𝙗𝙡𝙖

Mientras el sujeto leía en voz alta:

+ La señal mostró mayor irregularidad.

+ Se observaron variaciones en la amplitud.

+ Se prolongaron las fases de espiración (debido a la fonación).

+ La frecuencia respiratoria presentó cambios respecto al estado de reposo.

Esto confirma que el habla modifica el patrón respiratorio al introducir un control voluntario sobre el proceso automático de respiración.

<h1 align="center"><i><b>𝐏𝐚𝐫𝐭𝐞 𝘽 𝐝𝐞𝐥 𝐥𝐚𝐛𝐨𝐫𝐚𝐭𝐨𝐫𝐢𝐨</b></i></h1>

Este proyecto implementa un sistema de adquisición de señal respiratoria utilizando una DAQ, la cual captura el CO2 generada por un sensor MQ135 y envía los datos a MATLAB mediante comunicación serial.

El objetivo del script en MATLAB es:

+ Capturar la señal durante un tiempo definido.

+ Visualizarla.

+ Guardarla en un archivo .mat.

+ Permitir análisis posterior (filtrado, FFT y cálculo de frecuencia respiratoria)

𝙀𝙡 𝙛𝙡𝙪𝙟𝙤 𝙙𝙚𝙡 𝙨𝙞𝙨𝙩𝙚𝙢𝙖 𝙚𝙨:

Mascara →  Sensor MQ135  →  jumpers  →  DAQ  → MATLAB → Archivo .mat

La DAQ digitaliza la señal analógica del sensor MQ135. MATLAB recibe esos valores, los grafica y los almacena.

𝙀𝙭𝙥𝙡𝙞𝙘𝙖𝙘𝙞𝙤́𝙣 𝙙𝙚𝙡 𝙘𝙤𝙙𝙞𝙜𝙤
El propósito de este programa, creado en MATLAB, es obtener y examinar las señales respiratorias mediante un sensor que está conectado a una tarjeta de adquisición de datos NI USB-6002. Se efectúan dos mediciones: una cuando la persona está relajada y otra durante el habla de esta. Las señales se procesan más tarde con el fin de calcular la frecuencia respiratoria a través de dos técnicas: análisis espectral utilizando la Transformada Rápida de Fourier (FFT) y detección de picos.
>
Inicialización del sistema y la configuración de la adquisición de datos.
>
```
clc; clear; close all;
dq = daq("ni");
addinput(dq, "Dev1", "ai0", "Voltage");
dq.Rate = 100; 
tiempo_medicion = 30;
```
>
El programa muestra un mensaje para preparar al sujeto, espera tres segundos y registra la señal respiratoria durante 30 segundos, posteriormente se repite el mismo procedimiento, pero esta vez el sujeto realiza una actividad de habla durante la adquisición.
>
```
% MEDICIÓN EN RELAJACIÓN
disp("Preparar sujeto en reposo")
pause(3)
disp("Adquisición en RELAJACIÓN")
datos_relajacion = read(dq, seconds(tiempo_medicion));

% MEDICIÓN EN HABLA
disp("Preparar sujeto para HABLA")
pause(3)
disp("Adquisición en HABLA")
datos_habla = read(dq, seconds(tiempo_medicion));
```
Los datos obtenidos se separan en:
>
> Tiempo (Time): eje temporal de la adquisición.
> Voltaje (Dev1_ai0): amplitud de la señal respiratoria registrada.
>
Se generan dos conjuntos de datos:
>
Relajación.
Habla.
>
```

% EXTRACCIÓN DE SEÑALES
t_r = datos_relajacion.Time;
x_r = datos_relajacion.Dev1_ai0;
t_h = datos_habla.Time;
x_h = datos_habla.Dev1_ai0;
```
>
Visualización de las señales
>
>Se construyen dos gráficos para hacer una comparación visual de las dos condiciones.
>
Cada gráfico muestra:
>
> Eje X: tiempo (en segundos).
> Eje Y: voltaje que se ha medido.
> Cuadrícula para simplificar la interpretación.

Esta comparación posibilita la observación de las diferencias en el patrón respiratorio entre el habla y el estado de relajación.
>
```
% GRÁFICAS
figure
subplot(2,1,1)
plot(t_r, x_r)
title('Señal Respiratoria - Relajación')
xlabel('Tiempo (s)')
ylabel('Voltaje (V)')
grid on

subplot(2,1,2)
plot(t_h, x_h)
title('Señal Respiratoria - Habla')
xlabel('Tiempo (s)')
ylabel('Voltaje (V)')
grid on
```
>
La función **findpeaks** identifica los máximos locales de la señal, cada pico representa aproximadamente un ciclo respiratorio. Posteriormente se calcula la frecuencia.
>
```
FRECUENCIA RESPIRATORIA (TIEMPO - PICOS)
[pks_r, locs_r] = findpeaks(x_r, t_r);
[pks_h, locs_h] = findpeaks(x_h, t_h);
dur_r = max(t_r) - min(t_r);
dur_h = max(t_h) - min(t_h);
frec_r = length(pks_r) / dur_r; % Hz
frec_h = length(pks_h) / dur_h;
rpm_r = frec_r * 60;
rpm_h = frec_h * 60;
```
>
Para complementar el análisis temporal se emplea la Transformada Rápida de Fourier, donde la FFT transforma la señal del dominio del tiempo al dominio de la frecuencia.
>

```
% FRECUENCIA DOMINANTE (FFT)
fs = dq.Rate;
%  RELAJACIÓN 
N_r = length(x_r);
Y_r = fft(x_r);
f_r = (0:N_r-1)*(fs/N_r);
mag_r = abs(Y_r);
half_r = 1:floor(N_r/2);
[~, idx_r] = max(mag_r(half_r));
f_dom_r = f_r(idx_r);

%  HABLA 
N_h = length(x_h);
Y_h = fft(x_h);
f_h = (0:N_h-1)*(fs/N_h);
mag_h = abs(Y_h);
half_h = 1:floor(N_h/2);
[~, idx_h] = max(mag_h(half_h));
f_dom_h = f_h(idx_h);
```
**Resultados**
>
El programa muestra en pantalla:
>
>Con el propósito de relajarse:
>
-Frecuencia respiratoria determinada a través de los picos.
-Frecuencia predominante lograda a través de la FFT.
>
> Para hablar:
>
-Frecuencia de la respiración por picos.
-Frecuencia predominante por medio de la FFT.

Esto posibilita la comparación de ambos métodos estimativos.
>
```
% RESULTADOS
disp("========== RESULTADOS ==========")
fprintf("\n--- RELAJACIÓN ---\n")
fprintf("Frecuencia (picos): %.2f rpm\n", rpm_r)
fprintf("Frecuencia dominante: %.3f Hz (%.2f rpm)\n", f_dom_r, f_dom_r*60)
fprintf("\n--- HABLA ---\n")
fprintf("Frecuencia (picos): %.2f rpm\n", rpm_h)
fprintf("Frecuencia dominante: %.3f Hz (%.2f rpm)\n", f_dom_h, f_dom_h*60)
```
> Se generan dos gráficos del espectro (relajación y habla)
```
% ESPECTRO FRECUENCIAL
figure;
plot(f_r(half_r), mag_r(half_r))
title('Espectro - Relajación')
xlabel('Frecuencia (Hz)')
ylabel('Magnitud')
grid on
figure;
plot(f_h(half_h), mag_h(half_h))
title('Espectro - Habla')
xlabel('Frecuencia (Hz)')
ylabel('Magnitud')
grid on
```
GUARDADO DE DATOS
Se almacena toda la información en un archivo MATLAB (.mat) y exporta cada adquisición en formato CSV, permitiendo su análisis posterior en otras herramientas como Excel o Python.
```
save("Respiracion_MQ135_NI6002.mat","datos_relajacion","datos_habla","rpm_r","rpm_h","f_dom_r","f_dom_h")
writetable(datos_relajacion, "Relajacion.csv")
writetable(datos_habla, "Habla.csv")
```


<h2 align="center">𝘼𝙣𝙖𝙡𝙞𝙨𝙞𝙨 𝙙𝙚 𝙧𝙚𝙨𝙪𝙡𝙩𝙖𝙙𝙤𝙨</h2>

<img width="1385" height="912" alt="Figure_14" src="https://github.com/user-attachments/assets/fcab9d21-e951-458f-8c18-8df53d52b9de" />

𝙎𝙚𝙣̃𝙖𝙡 𝙧𝙚𝙨𝙥𝙞𝙧𝙖𝙩𝙤𝙧𝙞𝙖 𝙚𝙣 𝙧𝙚𝙡𝙖𝙟𝙖𝙘𝙞𝙤́𝙣

La señal presenta un comportamiento periódico, con aproximadamente cinco ciclos respiratorios en 30 segundos, lo que corresponde a una frecuencia cercana a 12 respiraciones por minuto. Este valor se encuentra dentro del rango esperado para una persona en estado de reposo, lo que indica que el sistema permitió registrar adecuadamente el patrón respiratorio.

𝙎𝙚𝙣̃𝙖𝙡 𝙧𝙚𝙨𝙥𝙞𝙧𝙖𝙩𝙤𝙧𝙞𝙖 𝙙𝙪𝙧𝙖𝙣𝙩𝙚 𝙚𝙡 𝙝𝙖𝙗𝙡𝙖

Durante el habla, la frecuencia respiratoria deja de ser constante y los ciclos presentan una duración variable. Esto se debe a que la respiración se adapta a las necesidades de la fonación, generando pausas y espiraciones prolongadas que modifican el patrón respiratorio. Como resultado, la frecuencia es menos uniforme y la señal presenta una menor periodicidad.

<h2 align="center">𝙋𝙧𝙚𝙜𝙪𝙣𝙩𝙖𝙨</h2>

+ ¿Son los patrones respiratorios y frecuencias respiratorias iguales o diferentes en cada caso? ¿A qué se debe esto?
  
> **Los patrones y las frecuencias respiratorias fueron diferentes en cada caso.** En la condición de relajación se observó un patrón respiratorio regular y periódico, con una frecuencia aproximada de **12 respiraciones por minuto**. En cambio, durante el habla la señal presentó una menor periodicidad y una frecuencia variable, debido a las pausas y modificaciones del flujo de aire necesarias para la producción de la voz. Estas diferencias se deben a que, en reposo, la respiración mantiene un ritmo estable, mientras que durante el habla el sistema respiratorio ajusta continuamente la inspiración y la espiración para permitir la fonación, alterando tanto el patrón como la frecuencia respiratoria.
+ ¿Cuáles serían las ventajas y desventajas de emplear múltiples sensores para el monitoreo del proceso respiratorio? ¿Cuáles podrían ser las razones?
  
> 
**VENTAJAS**
> 
>El empleo de diversos sensores posibilita mejorar la **exactitud** y fiabilidad de las mediciones al fusionar distintas variables fisiológicas. Por ejemplo, el empleo simultáneo de una galva de presión para identificar el movimiento del tórax y un sensor de gases (MQ135) para medir el c02 exhalado en cada respiración, posibilita verificar la respiración desde dos perspectivas diferentes, lo cual brinda una mayor seguridad respecto a la medición precisa de la actividad respiratoria.
>
>Otro beneficio significativo es que la información adquirida es más completa y puede compararse entre los distintos sensores. Un solo sensor brinda datos restringidos, pero la combinación de diversas señales permite que se detecten sucesos como patrones respiratorios irregulares o la apnea del sueño, puesto que estos pueden ser identificados con más exactitud cuando se correlaciona la información que llega de distintos orígenes.
>
>Además el uso de múltiples sensores, además, fortalece el sistema. Si uno de los sensores tiene un error o reporta información incorrecta, los demás siguen tomando mediciones, lo que asegura la continuidad del monitoreo y previene que se pierda información.

**DESVENTAJAS**
>
>El uso de múltiples sensores también presenta algunas desventajas.En primer lugar, incrementa el costo total del sistema debido a la incorporación de más componentes electrónicos. Asimismo, aumenta la complejidad del diseño, ya que es necesario sincronizar las señales provenientes de cada sensor y procesarlas de manera conjunta, lo que requiere algoritmos más elaborados y una mayor cantidad de líneas de programación.
>
>Otra desventaja es el aumento en el consumo de energía, ya que cada sensor demanda alimentación eléctrica para su funcionamiento. Este aspecto resulta especialmente crítico en sistemas portátiles o alimentados por baterías, donde la autonomía es un factor importante.
>
>Además, el procesamiento de múltiples señales implica una mayor carga computacional, debido a la necesidad de implementar algoritmos más complejos para el análisis, filtrado y fusión de los datos. Finalmente, pueden presentarse inconsistencias entre las mediciones de los distintos sensores, ya que cada uno posee características, niveles de sensibilidad y errores propios. Por esta razón, es indispensable realizar un proceso de calibración individual para garantizar que las mediciones sean precisas y consistentes.



<h1 align="center"><i><b>𝐏𝐚𝐫𝐭𝐞 𝘾 𝐝𝐞𝐥 𝐥𝐚𝐛𝐨𝐫𝐚𝐭𝐨𝐫𝐢𝐨</b></i></h1>

𝘾𝙤𝙣𝙘𝙡𝙪𝙨𝙞𝙤𝙣𝙚𝙨

𝟭. Se logró adquirir la señal respiratoria utilizando el sensor MQ-135 y la tarjeta de adquisición de datos NI USB-6002, evidenciando que el montaje permitió registrar las variaciones del aire exhalado.

𝟮. Los patrones respiratorios variaron según la condición evaluada. En estado de relajación se obtuvo una señal periódica y estable, mientras que durante el habla la señal presentó una mayor variabilidad debido a los cambios en el flujo de aire requeridos para la fonación.

𝟯. La frecuencia respiratoria estimada en reposo fue cercana a 10 respiraciones por minuto, valor que se encuentra dentro del rango fisiológico esperado, lo que indica que el sistema fue capaz de identificar adecuadamente los ciclos respiratorios.

𝘽𝙞𝙗𝙡𝙞𝙤𝙜𝙧𝙖𝙛𝙞𝙖

+ Biomedical Engineering Fundamentals | Joseph D. Bronzino | Taylor & Fr. (2006, April 14). Taylor & Francis. https://www.taylorfrancis.com/books/edit/10.1201/9781420003857/biomedical-engineering-fundamentals-joseph-bronzino
+ Fieselmann, J. F., Hendryx, M. S., Helms, C. M., & Wakefield, D. S. (1993). Respiratory rate predicts cardiopulmonary arrest for internal medicine inpatients. Journal of General Internal Medicine, 8(7), 354–360. https://doi.org/10.1007/bf02600071
+ Subbe, C. P., Davies, R. G., Williams, E., Rutherford, P., & Gemmell, L. (2003). Effect of introducing the Modified Early Warning score on clinical outcomes, cardio‐pulmonary arrests and intensive care utilisation in acute medical admissions*. Anaesthesia, 58(8), 797–802. https://doi.org/10.1046/j.1365-2044.2003.03258.x
+ Goldhill, D. R., McNarry, A. F., Mandersloot, G., & McGinley, A. (2005). A physiologically‐based early warning score for ward patients: the association between score and outcome*. Anaesthesia, 60(6), 547–553. https://doi.org/10.1111/j.1365-2044.2005.04186.x
+ Chourpiliadis, C., & Bhardwaj, A. (2022, September 12). Physiology, respiratory rate. https://www.ncbi.nlm.nih.gov/books/NBK537306/
+ Cretikos, M., Chen, J., Hillman, K., Bellomo, R., Finfer, S., & Flabouris, A. (2007). The objective medical emergency team activation criteria: A case–control study. Resuscitation, 73(1), 62–72. https://doi.org/10.1016/j.resuscitation.2006.08.020
