Aquí tienes el texto actualizado con la opción de instalación desde Composer:

---

## Agriconecta Core

Este módulo de Magento agrega un nuevo elemento de menú principal al panel de administración de Magento. 

### **Características**

* Crea un elemento de menú de nivel superior en el panel de administración.
* No agrega ninguna funcionalidad adicional; es solo un menú principal.

### **Instalación**

#### **Opción 1: Instalación mediante Composer (Recomendada)**

1. **Ejecuta el siguiente comando en la terminal desde el directorio raíz de tu instalación de Magento:**
   ```bash
   composer require agriconecta/module-core
   ```
2. **Habilita el módulo:**  
   ```bash
   php bin/magento module:enable Agriconecta_Core 
   ```
3. **Compila y despliega:**  
   ```bash
   php bin/magento setup:upgrade
   php bin/magento setup:static-content:deploy 
   ```
4. **Vacía la caché:**  
   ```bash
   php bin/magento cache:flush
   ```

#### **Opción 2: Instalación manual**

1. **Descarga el módulo:** Descarga el archivo del módulo y descomprímelo.  
2. **Copia al directorio de Magento:** Copia el contenido del módulo descomprimido en el directorio raíz de tu instalación de Magento.  
3. **Habilita el módulo:**  
   ```bash
   php bin/magento module:enable Agriconecta_Core 
   ```
4. **Compila y despliega:**  
   ```bash
   php bin/magento setup:upgrade
   php bin/magento setup:static-content:deploy 
   ```
5. **Vacía la caché:**  
   ```bash
   php bin/magento cache:flush
   ```

### **Desinstalación**

1. **Deshabilita el módulo:**  
   ```bash
   php bin/magento module:disable Agriconecta_Core 
   ```
2. **Si lo instalaste con Composer, elimínalo con:**  
   ```bash
   composer remove agriconecta/module-core
   ```
3. **Si lo instalaste manualmente, elimina los archivos del módulo del directorio de Magento.**  

### **Personalización**

Puedes cambiar el nombre y el icono del menú padre modificando el archivo de configuración del módulo.  

### **Soporte**

Si tienes algún problema o pregunta, crea un issue en el repositorio del módulo en Packagist:  
🔗 [Agriconecta Core en Packagist](https://packagist.org/packages/agriconecta/module-core)

---
