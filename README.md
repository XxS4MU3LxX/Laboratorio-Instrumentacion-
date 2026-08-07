# Laboratorio_1_Monitoreo del patrón y frecuencia respiratoria 

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

<img width="1402" height="1122" alt="image" src="https://github.com/user-attachments/assets/f8e681f5-f74f-4a74-875a-af07e903e475" />

𝙎𝙚𝙣𝙨𝙤𝙧 𝙚𝙨𝙘𝙤𝙜𝙞𝙙𝙤 

(samuel habla sobbre porque fue ese se sensor)

<img width="381" height="492" alt="image" src="https://github.com/user-attachments/assets/b69d795f-27fe-4837-9808-36ea78e3302e" />

𝘾𝙤𝙣𝙨𝙚𝙣𝙩𝙞𝙢𝙞𝙚𝙣𝙩𝙤 𝙞𝙣𝙛𝙤𝙧𝙢𝙖𝙙𝙤 𝙙𝙚𝙡 𝙥𝙖𝙧𝙩𝙞𝙘𝙞𝙥𝙖𝙣𝙩𝙚 

Debido a que la práctica involucró la adquisición de datos fisiológicos mediante el registro de la frecuencia respiratoria utilizando un sensor MQ-135 y una máscara, fue necesario obtener el consentimiento informado del participante. Este documento garantiza que la persona comprendió el objetivo del experimento, el procedimiento a realizar, el uso académico de los datos recolectados y la confidencialidad de la información, asegurando una participación libre y voluntaria de acuerdo con los principios éticos de la investigación.

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/8a69872f-8bd8-4ed0-a155-337248a09a5a" />

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

+ El conteo manual permitió estimar una frecuencia aproximada de ___ respiraciones por minuto.

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
(samuel)

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


<h1 align="center"><i><b>𝐏𝐚𝐫𝐭𝐞 𝘾 𝐝𝐞𝐥 𝐥𝐚𝐛𝐨𝐫𝐚𝐭𝐨𝐫𝐢𝐨</b></i></h1>

𝘾𝙤𝙣𝙘𝙡𝙪𝙨𝙞𝙤𝙣𝙚𝙨
1.Se logró adquirir la señal respiratoria utilizando el sensor MQ-135 y la tarjeta de adquisición de datos NI USB-6002, evidenciando que el montaje permitió registrar las variaciones del aire exhalado.

2.Los patrones respiratorios variaron según la condición evaluada. En estado de relajación se obtuvo una señal periódica y estable, mientras que durante el habla la señal presentó una mayor variabilidad debido a los cambios en el flujo de aire requeridos para la fonación.

3.La frecuencia respiratoria estimada en reposo fue cercana a 10 respiraciones por minuto, valor que se encuentra dentro del rango fisiológico esperado, lo que indica que el sistema fue capaz de identificar adecuadamente los ciclos respiratorios.
