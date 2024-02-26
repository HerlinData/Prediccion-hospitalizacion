# Diccionario de datos

Un destacado centro hospitalario busca obtener información sobre las características más relevantes de los pacientes que han sido diagnosticados con cierto tipo de enfermedad y que han requerido hospitalización. Esta categorización se ha establecido de la siguiente manera:

- Caso: Se refiere a aquel paciente que ha sido sometido a una biopsia prostática y que, en un periodo máximo de 30 días después del procedimiento, ha experimentado fiebre, infección urinaria o sepsis, lo que conduce a la atención médica ya sea de forma ambulatoria u hospitalaria.

- Contro l: Se refiere al paciente que ha sido sometido a una biopsia prostática y que no ha presentado complicaciones infecciosas en el periodo de 30 días posterior al procedimiento.

La biopsia prostática es un procedimiento diagnóstico que implica la extracción de una pequeña muestra de tejido prostático mediante una técnica de pinchazo. Posteriormente, esta muestra se analiza para detectar enfermedades como el cáncer.

Se dispone de una base de datos que contiene información sobre pacientes, así como los resultados de diversos exámenes diagnósticos, abarcando tanto a aquellos que han sido hospitalizados como a los que no. En esta recopilación, se destacan cuatro grupos de variables: Antecedentes del paciente, Morbilidad asociada al paciente, Antecedentes relacionados con la toma de la biopsia y Complicaciones infecciosas.


## Antecedentes del paciente

* **EDAD**: Dato cuantitativo continuo entero, que representa la edad del paciente.

## Morbilidad asociada al paciente

* **DIABETES**: Dato cualitativo categórico nominal, refiere a la **presencia**/**no presencia** de dicha en enfermedad en el paciente
* **HOSPITALIZACIÓN ULTIMO MES**: Dato cualitativo categórico nominal, refiere a la **hospitalización**/**no hospitalización** un mes previo al procedimiento
* **CUP**: Dato cualitativo categórico nominal, indica el uso de cateter urinario al momento de la biopsia.
* **ENF. CRONICA PULMONAR OBSTRUCTIVA**: Dato cualitativo categórico nominal, refiere si el paciente tiene una enfermedad CRONICA PULMONAR OBSTRUCTIVA previamente.
* **VOLUMEN PROSTATICO**: Dato cualitativo categórico nominal, indica si el volumna prostático es mayor a **40 cm³**.

Próstata: El volumen normal es de aproximadamente **20 cm³**. El crecimiento del tamaño de la próstata es lento y prácticamente inexistente hasta los 30 años. Después de esa edad, se espera un **crecimiento medio anual del tamaño de la próstata en torno al 1,6%** del volumen prostático cada año hasta la quinta década de la vida, en la que puede aumentar a un ritmo medio de **0,4 cm³** por año hasta el fallecimiento del paciente. Esto significa que la próstata es un órgano en continuo crecimiento y, por tanto, su tamaño normal aumentará de forma progresiva. Cuando el volumen prostático es mayor a **40 cm³**, puede causar síntomas y problemas urinarios debido a la compresión de la uretra.

Un **catéter urinario** es un tubo delgado que se pone en la vejiga para drenar la orina.

Una **enfermedad pulmonar obstructiva crónica** (EPOC) es una enfermedad pulmonar común que reduce el flujo de aire y causa problemas.respiratorios.

## Antecedentes relacionados con la toma de la biopsia

* **PSA**: Es la concentración de PSA en sangre. Es una variable cuantitativa continua.
* **BIOPSIAS PREVIAS**: Indica si el paciente ha tenido biopsias previas. Dato cualitativo categórico nominal.
* **ANTIBIOTICO UTILIAZADO EN LA PROFILAXIS**: Indica el tipo de antibiótico utilizado en la profilaxis. Es una variable categórica nominal.
    
    Tipos de antibióticos:
    * *FLUOROQUINOLONA_AMINOGLICOSIDO*
    * *CEFALOSPORINA_AMINOGLUCOCIDO*
    * *OROQUINOLONAS*
    * *OTROS*
* **NUMERO DE MUESTRAS TOMADAS**: Indica el número de muestras tomadas en la biopsia. En un número cuantitativo discreta (entero).
* **BIOPSIA**: Es el resultado de la biopsia. Es una variable categórica nominal.
    
    Se presentan como:
    * *NEG*: resultado negativo para cancer prostático.
    * *ADENOCARCINOMA GLEASON 6*: es un cáncer de grado bajo.
    * *ADENOCARCINOMA GLEASON 7*: es un cáncer de grado medio.
    * *ADENOCARCINOMA GLEASON 8*: es un cáncer de grado alto
    * *ADENOCARCINOMA GLEASON 9*: es un cáncer de grado alto
    * *ADENOCARCINOMA GLEASON 10*: es un cáncer de grado alto
    * *PROSTATITIS*: significa inflamación de la próstata.
    * *HIPERPLASIA PROSTATICA*: significa es un agrandamiento no canceroso de la glándula prostática.
    * *CARCINOMA INDIFERENCIADO DE CELULAS CLARAS*: es una tumoración altamente agresiva y los pacientes fallecen en el primer año después del diagnóstico a pesar del ensayo de la radioterapia.

**PSA** El PSA es una proteína producida por células normales y malignas de la próstata. La prueba del PSA mide su concentración en la sangre, expresada generalmente en nanogramos por mililitro (ng/ml). Anteriormente, se consideraba que concentraciones de PSA de 4,0 ng/ml o menos eran normales, pero no hay una norma fija. Concentraciones entre 4 ng/ml y 10 ng/ml no siempre indican cáncer, aunque a mayor concentración, aumenta la probabilidad de cáncer.

La concentración del PSA puede variar debido a factores como la edad, tamaño de la próstata, inflamación, biopsias, eyaculación, ejercicio vigoroso y medicamentos como finasterida y dutasterida. Medicamentos para la hiperplasia prostática benigna disminuyen el PSA.

Resultados positivos falsos son comunes, generando ansiedad y llevando a procedimientos innecesarios como biopsias. Solo alrededor del 25 % de las biopsias realizadas debido a concentraciones elevadas de PSA confirman cáncer de próstata, con posibles efectos secundarios como infecciones, dolor y sangrado.

## Complicaciones infecciosas

* **NUMERO DE DIAS POST BIOPSIA EN QUE SE PRESENTA LA COMPLICACIÓN INFECCIOSA**: indica el tiempo al cual se presenta la complicación infecciosa con un máximo de 30 días. En una variable cuantitativa discreta (entero).
* **FIEBRE**: indica si el paciente presenta fiebre. cualitativo categórico nominal.
* **ITU**: indica si el paciente presenta infección de tracto urinario. cualitativo categórico nominal.
* **TIPO DE CULTIVO**: indica el tipo de cultivo solicitado. Es una variable categórica nominal. 
    
    Entre los Tipos de Cultivos aparecen:
    * *Hemocultivo*: es un examen de laboratorio que permite verificar si hay bacterias u otros organismos en la muestra de sangre del paciente.
    * *Urocultivo*: examen que permite determinar la presencia de una infección urinaria.
    * *Hemocultivo y urocultivo*: cuando se piden ambos estudios.
    * *No*: cuando no se pide ninguno.
* **AGENTE AISLADO**: indica el tipo de agente aislado en el cultivo. Es una variable categórica nominal.
    
    Se indican:
    * *E. Coli*: es una de las bacterias más comúnmente implicadas en el desarrollo de infecciones prostática.
    * *Pseudomonas aeruginosa*: son patógenos oportunistas que con frecuencia causan infecciones intrahospitalarias.
    * *No*: que no se ha aislado agente. 
* **PATRON DE RESISTENCIA**: indica si presenta algún patrón de resistencia a los antibióticos. Es una variable categórica nominal.
    
    Se presentan como:
    * *AMPI*: significa resistencia a la ampicilina.
    * *CIPRO*: significa resistencia a ciprofloxacino.
    * *GENTA*: significa resistencia a gentamicina.
    * *SULFA*: significa resistencia a sulfametoxazol/trimetoprima.
    * *CEFADROXILO*: significa resistencia a cefadroxilo.
    * *CEFUROXIMO*: significa resistencia a cefuroxima.
    * *CEFEPIME*: significa resistencia cefepima.
    * *CEFOTAXIMA*: significa resistencia cefotaxima.
    * *MULTI SENSIBLE*: se refiere un paciente que experimenta resistencia a gran variedad de antibióticos.

* **HOSPITALIZACION**: indica si el paciente fue hospitalizado luego del procedimiento. Es una variable categórica nominal.
* **DIAS HOSPITALIZACION MQ**: indica los días de hospitalización médico quirúrgico. En una variable cuantitativa entera.
* **DIAS HOSPITALIZACIÓN UPC**: indica los días de hospitalización en estado crítico. En una variable cuantitativa entera.

Luego de realizar el ETL se cambiaron los nombres de las columnas de la siguiente manera:

   * EDAD: edad,
   * DIABETES: diabetes,
   * HOSPITALIZACIÓN ULTIMO MES: hosp_ult_mes,
   * PSA: psa,
   * BIOPSIAS PREVIAS: biop_prev,
   * VOLUMEN PROSTATICO: vol_prostatico,
   * ANTIBIOTICO UTILIAZADO EN LA PROFILAXIS: antib_en_profilaxis,
   * NUMERO DE MUESTRAS TOMADAS: n_muestras,
   * CUP: cup,
   * ENF. CRONICA PULMONAR OBSTRUCTIVA: e_cpo,
   * BIOPSIA: biopsia,
   * NUMERO DE DIAS POST BIOPSIA EN QUE SE PRESENTA LA COMPLICACIÓN INFECCIOSA: n_dias_con_infecc,
   * FIEBRE: fiebre,
   * ITU: itu,
   * TIPO DE CULTIVO: tipo_cultivo,
   * AGENTE AISLADO: agente_aislado,
   * PATRON DE RESISTENCIA: patron_resistencia,
   * HOSPITALIZACION: hospitalizacion,
   * DIAS HOSPITALIZACION MQ: dias_hosp_mq,
   * DIAS HOSPITALIZACIÓN UPC: dias_hosp_upc