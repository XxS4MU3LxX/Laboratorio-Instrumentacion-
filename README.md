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

. La señal presentó un comportamiento periódico y relativamente estable.

. Se observaron ciclos regulares correspondientes a inhalación y exhalación.

. La amplitud fue constante.

. El conteo manual permitió estimar una frecuencia aproximada de ___ respiraciones por minuto.

𝘿𝙪𝙧𝙖𝙣𝙩𝙚 𝙚𝙡 𝙝𝙖𝙗𝙡𝙖

Mientras el sujeto leía en voz alta:

. La señal mostró mayor irregularidad.

. Se observaron variaciones en la amplitud.

. Se prolongaron las fases de espiración (debido a la fonación).

. La frecuencia respiratoria presentó cambios respecto al estado de reposo.

Esto confirma que el habla modifica el patrón respiratorio al introducir un control voluntario sobre el proceso automático de respiración.

<h1 align="center"><i><b>𝐏𝐚𝐫𝐭𝐞 𝘽 𝐝𝐞𝐥 𝐥𝐚𝐛𝐨𝐫𝐚𝐭𝐨𝐫𝐢𝐨</b></i></h1>

Este proyecto implementa un sistema de adquisición de señal respiratoria utilizando una DAQ, la cual captura el CO2 generada por un sensor MQ135 y envía los datos a MATLAB mediante comunicación serial.

El objetivo del script en MATLAB es:

Capturar la señal durante un tiempo definido.

Visualizarla.

Guardarla en un archivo .mat.

Permitir análisis posterior (filtrado, FFT y cálculo de frecuencia respiratoria)
