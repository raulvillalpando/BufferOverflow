# BufferOverflow
Investigue 5 ejemplos de BufferOverflow en internet y explique como derivaron en fallas de seguridad.

### Ejemplos de BufferOverflow:

- **Ejemplo 1: CVE-2021-3156**

  En este ejemplo el error radica en en una parte del código del programa "sudo". Específicamente en la parte que gestionaba la verificación de contraseñas. El problema esta en la forma en que se manejaban ciertos caracteres especiales en las contraseñas. Se originó debido a un error en la eliminación de caracteres de escape en los comandos. Cuando Sudo ejecuta un comando en modo shell, debería escapar caracteres especiales con una barra invertida, pero el error permitió que se leyera más allá del último carácter si terminaba con una barra invertida sin escapar. Además, un error en el intérprete de la línea de comandos permitía la explotación de esta vulnerabilidad al habilitar el modo de shell sin ejecutar un comando, por lo que los usuarios no privilegiados podían elevaran sus privilegios a root en sistemas vulnerables.
  
  ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/CVE-2021-3156_1.png)
  
  ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/CVE-2021-3156_2.png)
  
- **Ejemplo 2: CVE-2023-45573**

  Esta vulnerabilidad permite a un atacante remoto ejecutar código arbitrario en dispositivos de red D-Link. A través del parámetro "n" de la función mrclfile_del.asp, lo que causa un BufferOverflow. El código es parte de la función sub_42FD38 y muestra cómo se maneja el parámetro "n" en el proceso, lo que lleva a un BufferOverflow cuando no se maneja correctamente.

  ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/CVE-2023-45573.png)

- **Ejemplo 3:**

 Para este caso se afecta específicamente la app "MP4Box". Se causa un BufferOverflow en el archivo isom_write_c. El problema se encuentra en el manejo incorrecto de los datos de tamaño de muestra (sampleSize) en la tabla stsz. El error se produce cuando se intenta escribir más datos de los que la ubicación de memoria puede contener. Se está sobrescribiendo la memoria más allá de los límites que deberían respetarse.

 ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/CVE-2023-46927.png)

 - **Ejemplo 4:**
 sample text
 ![]()

 - **Ejemplo 5:**
 sample text
 ![]()

---

**Referencias:**
- [Ejemplo 1](https://blog.qualys.com/vulnerabilities-threat-research/2021/01/26/cve-2021-3156-heap-based-buffer-overflow-in-sudo-baron-samedit)
- [Ejemplo 2](https://github.com/Archerber/bug_submit/blob/main/D-Link/DI-7xxxx/bug7.md)
- [Ejemplo 3](https://github.com/gpac/gpac/commit/a7b467b151d9b54badbc4dd71e7a366b7c391817?diff=unified)
- [Ejemplo 4]()
- [Ejemplo 5]()
