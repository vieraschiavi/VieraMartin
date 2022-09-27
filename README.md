
Martin Viera Schiavi, Matias Nuñez Franco

Coderhouse

DataScience Proyect


credit_card_churn.csv: Archivo con las base de datos  (Necesario para la ejecución del código)


#Tema: Abandono de Clientes de tarjetas de Credito
#Introducción
#Las tarjetas de crédito son una buena fuente de ingresos para los bancos debido a los diferentes tipos de comisiones que cobran, como las tasas anuales, las de transferencia de saldo, las de adelanto de efectivo, las de retraso en los pagos y las de transacciones extranjeras, entre otras. Algunas comisiones se cobran a todos los usuarios, independientemente de su uso, mientras que otras se cobran en determinadas circunstancias.

El hecho de que los clientes abandonen los servicios de las tarjetas de crédito supondría una pérdida para el banco, por lo que éste quiere analizar los datos de los clientes e identificar a los que abandonan los servicios de las tarjetas de crédito y las razones para ello, de modo que el banco pueda mejorar en esas áreas.

Un modelo de abandono de clientes es una representación matemática de cómo el abandono afecta a su negocio. Los cálculos de abandono de clientes se construyen a partir de los datos existentes (el número de clientes que abandonaron su servicio durante un periodo de tiempo determinado). Un modelo predictivo de cancelación de clientes extrapola estos datos para mostrar las tasas de cancelación de clientes potenciales en el futuro.

El churn (también conocido como deserción de clientes) es un problema para las empresas de suscripción. Cuando sus ingresos se basan en contratos mensuales o anuales recurrentes, cada cliente que se va hace mella en su flujo de caja. Unas altas tasas de retención son vitales para su supervivencia. ¿Y si le dijéramos que hay una forma de predecir, al menos hasta cierto punto, cómo y cuándo cancelarán sus clientes?

La creación de un modelo de predicción de bajas le ayudará a realizar cambios proactivos en sus esfuerzos de retención que reduzcan las tasas de bajas. Comprender el impacto de la pérdida de clientes en sus objetivos de ingresos actuales y hacer predicciones sobre cómo gestionar esos problemas en el futuro también le ayuda a frenar el flujo de clientes perdidos. Si no toma medidas contra la pérdida de clientes ahora, cualquier crecimiento de la empresa que experimente no será sostenible.

Los perfiles completos de los clientes le ayudan a ver qué tipos de clientes están cancelando sus cuentas. Ahora es el momento de averiguar cómo y por qué se dan de baja. Hágase las siguientes preguntas para saber más sobre los puntos conflictivos de su producto y la experiencia del cliente que hacen que éste decida darse de baja.

¿Qué es la pérdida de clientes?
La pérdida de clientes (o desgaste de clientes) es la tendencia de los clientes a abandonar una marca y dejar de ser clientes de pago de una empresa determinada. El porcentaje de clientes que dejan de utilizar los productos o servicios de una empresa durante un periodo de tiempo determinado se denomina tasa de abandono de clientes (attrition). Una de las formas de calcular la tasa de abandono es dividir el número de clientes perdidos durante un intervalo de tiempo determinado entre el número de clientes adquiridos y, a continuación, multiplicar esa cifra por el 100%. Por ejemplo, si ha conseguido 150 clientes y ha perdido tres el mes pasado, su tasa de abandono mensual es del 2%.

El índice de rotación es un indicador de salud para las empresas cuyos clientes están suscritos y pagan por los servicios de forma recurrente, por lo que un cliente permanece abierto a ofertas más interesantes o ventajosas. Además, cada vez que termina su compromiso actual, los clientes tienen la oportunidad de reconsiderar y elegir no continuar con la empresa. Por supuesto, una parte de la rotación natural es inevitable, y la cifra difiere de un sector a otro. Pero tener una cifra de churn más alta que esa es una señal definitiva de que una empresa está haciendo algo mal".

Hay muchas cosas que las marcas pueden hacer mal, desde una incorporación complicada en la que no se da a los clientes información fácil de entender sobre el uso del producto y sus capacidades, hasta una mala comunicación, por ejemplo, la falta de comentarios o el retraso en las respuestas a las consultas. Otra situación: Los clientes veteranos pueden sentirse poco apreciados porque no reciben tantas bonificaciones como los nuevos.

#Objetivo

Explorar y visualizar el conjunto de datos.
Construir un modelo de clasificación para predecir si el cliente va a abandonar o no.
Optimizar el modelo utilizando las técnicas adecuadas
Generar un conjunto de ideas y recomendaciones que ayuden al banco   

#Problema
¿Tienen los ingresos algún efecto sobre el abandono?
¿Tiene el sexo alguna relación con el abandono?
¿Cuáles son los signos de desgaste?


#Problemática
Indicación de la fuente del dataset y los criterios de selección (Data Acquisition)

Dataset https://www.kaggle.com/code/xavier14/predicting-churn-with-tree-based-models

Criterios de selección: Para el presente trabajo se realizó una búsqueda de los dataset que realmente fuera de nuestro interés.
Consideramos importante que los datos se adecuaran a los requerimientos en cuanto a calidad y cantidad para un mejor análisis, entre ellas que tenga una cantidad suficiente de variables numéricas y también categóricas, que no tenga o bien tenga una cantidad reducida de datos nulos.

Nuestro dataset contiene el abandono de los clientes de las tarjetas de credito segun distintas variables.

Variables
CLIENTNUM = Client number. Unique identifier for the customer holding the account

Attrition_Flag = Internal event (customer activity) variable - if the account is closed then 1 else 0

Customer_Age = Demographic variable - Customer's Age in Years

Gender = Demographic variable - M=Male, F=Female

Dependent_count = Demographic variable - Number of dependents

Education_Level = Demographic variable - Educational Qualification of the account holder (example: high school, college graduate, etc.)

Marital_Status = Demographic variable - Married, Single, Divorced, Unknown

Income_Category = Demographic variable - Annual Income Category of the account holder (<  40K, 40K - 60K,  60K− 80K,  80K− 120K, $120K >)

Card_Category = Product Variable - Type of Card (Blue, Silver, Gold, Platinum)

Months_on_book = Period of relationship with bank

Total_Relationship_Count = Total no. of products held by the customer

Months_Inactive_12_mon = No. of months inactive in the last 12 months

Contacts_Count_12_mon = No. of Contacts in the last 12 months

Credit_Limit = Credit Limit on the Credit Card

Total_Revolving_Bal = Total Revolving Balance on the Credit Card

Avg_Open_To_Buy = Open to Buy Credit Line (Average of last 12 months)

Total_Amt_Chng_Q4_Q1 = Change in Transaction Amount (Q4 over Q1)

Total_Trans_Amt = Total Transaction Amount (Last 12 months)

Total_Trans_Ct = Total Transaction Count (Last 12 months)

Total_Ct_Chng_Q4_Q1 = Change in Transaction Count (Q4 over Q1)

Avg_Utilization_Ratio = Average Card Utilization Ratio

#¿Qué es un saldo renovable(Revolving Balance)?

Si no pagamos el saldo de la cuenta de crédito renovable en su totalidad cada mes, la parte no pagada se traslada al mes siguiente. A eso se le llama saldo renovable

¿Qué es el saldo medio abierto para comprar( Average Open to buy)?

El "Open to Buy" significa la cantidad que le queda a su tarjeta de crédito por utilizar. Esta columna representa la media de este valor en los últimos 12 meses.

¿Qué es el Ratio de utilización media (Average utilization Ratio)?

El Avg_Utilization_Ratio representa cuánto del crédito disponible gastó el cliente. Esto es útil para calcular la puntuación de crédito.

Relación entre Avg_Open_To_Buy, Credit_Limit y Avg_Utilization_Ratio:

( Avg_Open_To_Buy / Credit_Limit ) + Avg_Utilization_Ratio = 1
