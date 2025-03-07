## Agriconecta Core

Este módulo de Magento agrega un nuevo elemento de menú principal al panel de administración de Magento. 

**Características**

* Crea un elemento de menú de nivel superior en el panel de administración.
* No agrega ninguna funcionalidad adicional; es solo un menú principal.

**Instalación**

1. **Descarga el módulo:** Descarga el archivo del módulo y descomprímelo. 
2. **Copia al directorio de Magento:** Copia el contenido del módulo descomprimido en el directorio raíz de tu instalación de Magento. 
3. **Habilita el módulo:** Habilita el módulo ejecutando el siguiente comando en tu terminal desde el directorio raíz de Magento:
   ```bash
   php bin/magento module:enable Agriconecta_Core 
   ```
4. **Compila y despliega:** Compila y despliega los archivos estáticos de Magento ejecutando los siguientes comandos:
   ```bash
   php bin/magento setup:upgrade
   php bin/magento setup:static-content:deploy 
   ```
5. **Vaciar la caché:** Vacía la caché de Magento: 
   ```bash
   php bin/magento cache:flush
   ```

**Desinstalación**

1. **Deshabilita el módulo:** Deshabilita el módulo ejecutando el siguiente comando:
   ```bash
   php bin/magento module:disable Agriconecta_Core 
   ```
2. **Elimina el módulo:** Elimina los archivos del módulo del directorio de Magento. 

**Personalización**

Puedes cambiar el nombre y el icono del menú padre modificando el archivo de configuración del módulo. 

**Soporte**
Si tienes algún problema o pregunta, crea un issue en el repositorio del módulo. 
