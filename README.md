# AREP-LLM

En este laboratorio, exploraremos como trabajar con Python y la API de OpenAI para crear un prompt, para realizar consultas especificas y aprender el uso de la inteligencia artificial. 

## Prerequisitos

* Se debe tener minimo: Python, Pip. Si desea el paso a paso de cada uno de estas instalaciones de manera más visual para mejor comprensión, puede buscar una breve explicacion en Youtube, sin embargo, adjunto los links de las paginas oficiales donde indican paso a paso su respectiva instalación.

    - Python <br>
     <https://www.python.org/downloads/>
    - Pip <br>
     <https://docs.python.org/es/3/installing/index.html>

## Empezando

* Para obtener una copia del proyecto en su maquina local:

    - Se debe ubicar en la carpeta donde desea bajar el proyecto y le da click donde señala la flecha y esribe cmd:

      ![image](https://github.com/XimenaRodriguez20/AREP-Taller2/assets/123812926/52f8f03c-3b3e-48cf-bd2c-f7b029c2d8bb)

    - Después de esto debe escribir el siguiente comando:

        ~~~                  
            git clone https://github.com/XimenaRodriguez20/AREP-LLM.git
        ~~~                                                                   

* Para acceder al repositorio desde consola utilice el siguiente comando:

    ~~~
       cd AREP-Taller6/
    ~~~

* Para poder correr el código abra el IDE de su preferencia, por recomendación utilice Pycharm.
* En la terminal del IDE debera escribir el siguiente comando que es necesario para poder ejecutar el codigo:

    - Para instalar pip utilice:
  
        ~~~                 
            pip install -r 'requirements.txt'
        ~~~  

## Descripción 

### Escriba un programa para enviar mensajes a Chatgpt y recuperar respuestas.
    
  ~~~                 
      LangChain.py
  ~~~ 

En esta clase necesitamos utilizar una llave que se nos genera por parte de la Api de OpenAI y se hace uso de la biblioteca Lang Chain para interactuar con OpenAI y enviar las solicitudes a Chatgpt. 

![image](https://github.com/XimenaRodriguez20/AREP-LLM/assets/123812926/ac5b4ebe-19bc-4570-a0cc-0cd9057e39d9)

### Escriba un RAG simple utilizando una base de datos vectorial en memoria

  ~~~                 
      RAG.py
  ~~~ 

En esta clase necesitamos utilizar una llave que se nos genera por parte de la Api de OpenAI pero en este caso la informacion que se le va a consultar no va a ser de nuestro interes ni directamente proporcionado por nosotros sino que en este caso se alimenta del siguiente repositorio <"https://lilianweng.github.io/posts/2023-06-23-agent/">, por lo cual la pregunta que se hace va referente a los datos que nos brinda este. 

![image](https://github.com/XimenaRodriguez20/AREP-LLM/assets/123812926/19295206-5537-4d6f-8406-36d4770e9143)

### Escriba un RAG simple utilizando Pinecone

  ~~~                 
      Pinecone.py
  ~~~ 

Se crea una cuenta en [Pinecone](https://app.pinecone.io/organizations/-NvDhN1HGcD4EGX_nFND/projects/c88cc521-9391-4782-9b5e-05bc962020ae/indexes), para poder generar La base de datos vectorial que se va a usar para alimentar la IA.

En esta clase necesitamos utilizar una llave que se nos genera por parte de la Api de OpenAI y además debemos de poner la llave que  nos genera Pinecone para hacer uso de la respectiva base de datos.

![image](https://github.com/XimenaRodriguez20/AREP-LLM/assets/123812926/b91175e8-c75b-4a5c-bfd3-86298c0a8e15)

En esta clase se tienen dos funciones muy importantes la primera es:

  - loadText: Aca se indica el archivo(Datos de nuestro interes) que debe leer Pinecone para alimentar la base de datos, para poderla consultar luego. Una ves se ejecuta esta función en Pinecone se crea este Index que es quien divide la información en diferentes partes, estas seran las respuestas que se van a proporcionar al usuario dependiendo la pregunta que haga.
 
    ![image](https://github.com/XimenaRodriguez20/AREP-LLM/assets/123812926/0df96564-ab4d-45df-8ab9-73aaaba921c7)

  - search: Aca directamente se va añadir la pregunta que quiera hacerle a la IA.



## Autor

* **Ximena Rodriguez** 
