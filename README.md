# 🦷 LUC-IA — Asistente Inteligente en Odontología

LUC-IA es una aplicación web desarrollada con **Streamlit** que actúa como un **asistente de inteligencia artificial especializado en odontología**.  
Permite consultar información clínica y técnica a partir de una base documental en PDF, utilizando **búsqueda semántica y modelos generativos** para ofrecer respuestas precisas y contextualizadas, acompañadas de referencias.

---

## 🚀 Funcionalidades principales

- 📄 **Carga y procesamiento automático de documentos PDF**
- 🧠 **Indexación semántica** mediante embeddings y FAISS
- 🔍 **Búsqueda por similitud** para recuperar información relevante
- 🤖 **Generación de respuestas en lenguaje natural** usando modelos de OpenAI
- 📚 **Trazabilidad y referencias**: cada respuesta incluye los fragmentos utilizados
- 🎨 **Interfaz personalizada** con estilos CSS avanzados en Streamlit
- 🧭 **Sidebar interactivo** con secciones informativas integradas

---

## 🧠 Arquitectura del sistema

1. **Carga de documentos**
   - Lectura de PDFs desde una carpeta local (`documentacion_odontologia`)
   - Extracción de texto con `PyPDF2`

2. **Procesamiento**
   - División del texto en *chunks* con solapamiento
   - Generación de embeddings usando `OpenAIEmbeddings`

3. **Indexación**
   - Almacenamiento vectorial con **FAISS**

4. **Consulta**
   - Búsqueda semántica (`similarity_search_with_score`)
   - Construcción de prompt contextualizado

5. **Generación**
   - Respuesta generada por un modelo LLM de OpenAI
   - Inclusión de referencias relevantes

---

## 🛠️ Tecnologías utilizadas

- **Python**
- **Streamlit**
- **LangChain**
- **OpenAI API**
- **FAISS**
- **PyPDF2**
- **dotenv**
- **HTML & CSS personalizado**

---

## 📁 Estructura del proyecto


