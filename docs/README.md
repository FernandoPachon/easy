# Store theme Easy

Este proyecto es el resultado del seguimiento del bootcamp de `Vtex U`, su objetivo era lograr crear una replica de alguna tienda, y poder implementar elemento custom.
![](https://github.com/FernandoPachon/store-theme-easy/blob/main/assets/img/desktop.jpeg?raw=true)

 ### *Si has decidido usar este ropositorio como guia, es porque ya tienes conocimientos basicos sobre `WorkSpace` y `Vtex`.*
### Palabras clave
* Linkear: usar en la consola `vtex link`
* Matar consola: usar en la consola `control` + `c`
# Configuraciones

## 1. Clonación
Nuestro primer paso sera clonar este repositorio, puedes poner `/generate` al final del link para crear una  copia.

## 2. Editar manifest
En esta altura ya el proyecto esta montado en nuestro editor de codigo, buscamos el archivo `manifest.json`, modificaremos el vendor por el de nuestro partnert y le daramos un nombre a nuestro tema base *"store-theme"*.
     
   ```json
 {
  "vendor": "itgloberspartnercl",
  "name": "store-theme",
  "version": "0.0.1",
  "builders": {
    "assets": "0.x",
    "styles": "2.x",
    "sitemap": "0.x",
    "store": "0.x",
    "docs": "0.x"
 },
     
  ```
  ## 3. Instalar apps
  Antes que nada verificaremos que nuestras apps que esten siendo declaradas en las dependencias esten correctamente instalas, para ello usaremos en la consola el comando `vtex ls` y esperaremos una respuesta similar a esta.
  
   ```json
   
Edition Apps in itgloberspartnercl at workspace user
vtex.admin                              3.54.5 
vtex.admin-apps                         3.29.2
vtex.admin-audit                        2.3.0
vtex.admin-binding                      0.28.0
vtex.admin-cms                          1.10.0
vtex.admin-collections                  0.162.3
vtex.admin-defense-mode                 0.4.2
vtex.admin-docs                         0.4.3
vtex.admin-home                         2.37.0
vtex.admin-insights                     4.4.2
vtex.admin-inventory                    0.49.3
vtex.admin-login                        1.24.2
vtex.admin-logistics                    1.36.1
vtex.admin-mercadolivre-opportunities   0.7.9
vtex.admin-orders                       0.134.2
vtex.admin-pages                        4.49.8
vtex.admin-payment-affiliations         0.1.1
vtex.admin-pickup-points                2.13.2
vtex.admin-pricing-settings             1.6.1
vtex.admin-sales-performance            1.1.3
vtex.admin-sellers                      1.3.7
vtex.admin-sku-binding                  0.5.0
vtex.admin-sponsor                      1.0.2
vtex.admin-suggestions                  2.35.1
vtex.admin-users                        1.16.1
vtex.admin-vendor-invite                0.12.0
vtex.app-install-monitor                0.1.1
vtex.asset-server                       0.15.5
vtex.audit-io                           0.1.4
vtex.auth-admin                         3.60.1
vtex.auth-server                        0.18.0
vtex.billing                            0.24.0
vtex.broadcaster                        0.9.0
vtex.builder-hub                        0.285.4
vtex.cartman                            0.3.1
vtex.checkout                           0.6.0
vtex.client-admin-settings              0.7.0
vtex.colossus-legacy-proxy              2.3.5
vtex.developer-docs-integration         0.5.6
vtex.dotnet-messenger-sender            0.1.7
vtex.evolution-manager-graphql          0.15.3
vtex.file-manager                       0.11.0
vtex.frontend-metrics-gateway           0.7.0
vtex.invoice-notifier                   0.8.2
vtex.marketplace-network                0.17.1
vtex.messages-templates                 0.10.1
vtex.messenger-core                     0.1.9
vtex.mkp-category-mapper-ui             1.20.2
vtex.my-account                         0.41.0
vtex.my-authentication                  1.5.0
vtex.myuser-io                          2.18.1
vtex.notification-generator             0.6.2
....................................... e.t.c   
     
  ```
  
 Es probable que las dependencias custom no esten instaladas, para ello puedes clonarlo directamente de [Boton de whasapp](https://github.com/FernandoPachon/component-custom-Button-Whastapp " Boton de Whatsapp"), [Add to cart](https://github.com/FernandoPachon/component-custom-add-to-card-info "add to cart"), [Bullets diagramation](https://github.com/FernandoPachon/component-custom-bullets-diagramation "bullets diagramation"), [Department search](https://github.com/FernandoPachon/component-custom-departent-search "deparment search"), [Pdf reader](https://github.com/FernandoPachon/component-custom-pdf-reader "Quick order"), [Pdf reader](https://github.com/FernandoPachon/component-custom-quick-order "quick-order"), en cada repositorio encontraras las configuraciones necesarias.
 
 ## 4.Enlazar tu workspace en el `CMS`
 
 El nombre del tema base que se le ha asignado en el `manifest.json` lo asignaremos en el `CMS`, para ello linkearemos y lanzaremos en una pestaña nuestro tema base
    ```json
    
        https://yourWorkspace--yourPartner.myvtex.com/admin  

  ```
