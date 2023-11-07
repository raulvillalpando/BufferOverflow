# BufferOverflow
Investigue 5 ejemplos de BufferOverflow en internet y explique como derivaron en fallas de seguridad.

### Ejemplos de BufferOverflow:

- **Ejemplo 1:**

  En este ejemplo el error radica en que el arreglo "buffer" espera recibir cinco caracteres, realiza una copia de lo
  que recibe sin verificar cuantos caracteres son, por lo que en caso de que reciba mas de cinco se causa un buffer
  overflow.
  
  ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/image_2023-11-06_202557125.png)

- **Ejemplo 2:**
  sample text
  ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/image_2023-11-06_210557868.png)

- **Ejemplo 3:**
 sample text
 ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/image_2023-11-06_210959371.png)

 - **Ejemplo 4:**
 sample text
 ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/image_2023-11-06_211429596.png)

 - **Ejemplo 5:**
 sample text
 ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/image_2023-11-06_211559041.png)

---

**Referencias:**
- [Ejemplo 1](https://www.geeksforgeeks.org/buffer-overflow-attack-with-example/)
- [Ejemplo 2](https://owasp.org/www-community/attacks/Buffer_overflow_attack)
- [Ejemplo 3](https://cwe.mitre.org/data/definitions/122.html)
- [Ejemplo 4](https://learn.microsoft.com/en-us/cpp/sanitizers/error-heap-buffer-overflow?view=msvc-170)
- [Ejemplo 5](https://owasp.org/www-community/attacks/Buffer_overflow_attack)
