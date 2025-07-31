| **Repositorio** | Crea un repo en GitHub llamado **python-json-bootcamp** y haz tu primer commit (`README.md`). |

---

### Día 1 · Fundamentos del lenguaje (2–3 h)

1. **Sintaxis mínima**  
   - Sentencias, indentación, comentarios.
2. **Tipos primitivos**  
   - `int`, `float`, `str`, `bool`, `None`.  
   - Conversión entre tipos (`str(42)`, `int("7")`).
3. **Variables y operadores**  
   - Aritméticos, lógicos, comparación.
4. **Control de flujo**  
   - `if/elif/else`, bucle `for`, `while`, `break`, `continue`.  
   - *Mini‑ejercicio*: imprime los números pares del 1 al 20.

---

### Día 2 · Estructuras de datos (2–3 h)

| Estructura | Por qué importa para JSON | Actividad |
|------------|---------------------------|-----------|
| `list`     | JSON **array**            | Crea una lista de tareas y recórrela. |
| `dict`     | JSON **object**           | Construye un diccionario `user = {"id": 1, "name": "Ana"}` y accede a sus claves. |
| `set` / `tuple` | (opcionales) | Entiende sus diferencias; no se serializan directo a JSON pero son útiles internamente. |
- *Mini‑reto*: combina una lista de usuarios con sus correos en un diccionario.

---

### Día 3 · Funciones y módulos (2 h)

1. **Definir funciones** (`def saludo(nombre): ...`).  
2. **Argumentos opcionales** y retorno de valores.  
3. **Importar módulos estándar** (`import math`, `from datetime import datetime`).  
4. **`pip install requests`** para pruebas HTTP del día 6.

*Ejercicio*: crea `utilidades.py` con una función `slug(texto)` y úsala desde un script.

---

### Día 4 · Entrada/Salida de archivos (2 h)

1. Lectura y escritura con `with open("archivo.txt", "r") as f:`.  
2. Concepto de **codificación UTF‑8** (por qué importa en JSON).  
3. *Mini‑proyecto*: guarda la lista de tareas de Día 2 en un `.txt` y vuelve a cargarla.

---

### Día 5 · Manejo de errores (1.5 h)

1. **`try/except`** básicos.  
2. Tipos de excepciones comunes (`ValueError`, `FileNotFoundError`).  
3. *Kata*: convierte una lista de cadenas en enteros; gestiona los valores no numéricos con un `try/except`.

---

### Día 6 · Networking rápido con `requests` (2 h)

1. Instalación (ya hecha).  
2. `response = requests.get("https://jsonplaceholder.typicode.com/todos/1")`.  
3. Atributos clave: `status_code`, `headers`, `json()`.  
4. *Ejercicio*: descarga 5 tareas y muestra sólo las completadas (`completed == True`).

---

### Día 7 · Proyecto “Puente a JSON” (3–4 h)

**Objetivo**: integrar todo lo aprendido en un script que:

1. Reciba por *CLI* (`argparse`) una URL de API pública que devuelva JSON.  
2. Haga la petición con `requests`.  
3. Compruebe el código 200 y maneje errores de red.  
4. Guarde la respuesta en **`data.json`** con `with open(..., "w")`.  
5. Lea nuevamente ese archivo y filtre/regroupe datos con listas y diccionarios.  
6. Imprima un pequeño reporte al usuario.

> **Entrega**: sube el script y un `README.md` con instrucciones de uso a tu repo. ¡Listo para iniciar el curso intensivo de JSON!

---

## Resumen de habilidades cubiertas

| Categoría                  | Competencia mínima alcanzada |
|----------------------------|------------------------------|
| Sintaxis & flujo básico    | ✓ |
| Listas y diccionarios      | ✓ (mapear ↔ JSON) |
| Funciones & módulos        | ✓ |
| Manejo de archivos         | ✓ (lectura/escritura UTF‑8) |
| Entornos y paquetes        | ✓ (`venv`, `pip`) |
| Manejo de errores          | ✓ |
| Peticiones HTTP simples    | ✓ (`requests`) |

Con este **bootcamp de 1 semana** estarás plenamente equipado para abordar el plan intensivo de JSON: podrás serializar, parsear, validar y transformar datos, así como consumir APIs sin obstáculos de sintaxis o entorno. Cuando termines la fase de JSON, ya tendrás bases sólidas para profundizar en Python avanzado (OOP, asíncrono, testing, frameworks web, data science, etc.). ¡Éxitos en tu camino!
