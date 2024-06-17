# marketplace-ml
**Analítica de Descuentos y predicción de Precios en el Market Place de MELI**

El repositorio contiene 4 Notebooks:

1. data_collection.ipynb : consumo de las APIs de MELI para extraer información y contrucción de los Datasets base.
2. EDA_Discounts.ipynb: análisis de descuentos.
3. price_prediction.ipynb : modelamiento para predicción del precio.
4. mvp_llm.ipynb : modelo LLM para aprender de la relación de productos y precios. Ej: ¿Cuál es el precio de audifonos? -> Repuesta 20 Usd. Este modelo surge como respuesta a la alta variabilidad de los productos en el Marketplace, ya que como se evidenció en el Modelamiento predictivo, predecir el precio de un producto con variables parametrizables de la plataforma de MELI es complejo (ej: condition, accpets_mercado_pago, listing_type_id, category_id), el precio depende de propiedades intrínsecas de los items y un modelo LLM puede capturar estas relaciones. Posibilidad de mejora: utilizar el modelamiento predictivo del paso 4 para entrenar el modelo LLM y delimitar los precios por categorías.

Adicionalmente se comparte el archivo requirements.txt con las dependencias necesarias para la ejecución del proyecto y un jamboard con el análisis de: el negocio de MELI, los múltiples endpoints de la API pública, las variables más relevantes, y la construcción del DataSet.

