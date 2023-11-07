# BufferOverflow
Investigue 5 ejemplos de BufferOverflow en internet y explique como derivaron en fallas de seguridad.

### Ejemplos de BufferOverflow:

- **Ejemplo 1: CVE-2021-3156**

  En este ejemplo el error radica en en una parte del código del programa "sudo", especificamente en la parte que gestionaba la verificación de contraseñas. El problema esta en la forma en que se manejaban ciertos caracteres especiales en las contraseñas, específicamente los caracteres '!' y '-'. Cuando un usuario intentaba utilizar una contraseña que contenía estos caracteres especiales, el "sudo" interpretaba incorrectamente la entrada y permitía que el usuario ejecutara comandos con privilegios de superusuario, incluso si no tenía permisos para hacerlo. Esto significaba que un atacante potencial podría utilizar una contraseña manipulada para eludir las restricciones de seguridad y ejecutar comandos peligrosos en el sistema.
  
  ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/CVE-2021-3156_1.png)
  
  ![](https://github.com/raulvillalpando/BufferOverflow/blob/main/CVE-2021-3156_2.png)
  
- **Ejemplo 2:**
  sample text
  ![]()

- **Ejemplo 3:**
 sample text
 ![]()

 - **Ejemplo 4:**
 sample text
 ![]()

 - **Ejemplo 5:**
 sample text
 ![]()

---

**Referencias:**
- [Ejemplo 1](https://blog.qualys.com/vulnerabilities-threat-research/2021/01/26/cve-2021-3156-heap-based-buffer-overflow-in-sudo-baron-samedit)
- [Ejemplo 2]()
- [Ejemplo 3]()
- [Ejemplo 4]()
- [Ejemplo 5]()
