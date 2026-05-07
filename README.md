# Taller-pr-ctico-03-Laboratorio-Ecosistema-Odoo
## Fase 1: Integración de Módulos
En el apartado de aplicaciones deberemos buscar e instalar los modulos de Inventario y facturacion
Una vez creado abrimos VS code y crearemos un archivo donde lo llamaremos clientes_mock.csv para crear unos clientes ficticios.
En ese archivo escribiremos esto:
<img width="684" height="244" alt="image" src="https://github.com/user-attachments/assets/94d86f96-cc5d-4859-a05d-fc2b3fb97e31" />

Una vez guardado el archivo nos dirirgiremos a odoo, nos vamos al apartado de ventas y una vez dentro a clientes. Una vez hecho eso en la parte superior
le damos al engranage y le daremos a importar archivo y buscamos nuestro arvicho clientes_mock.csv , despues le damos a tets e importar, nos quedaria una cosa asi:
<img width="1574" height="658" alt="image" src="https://github.com/user-attachments/assets/8087abd4-41d5-4740-97f7-acd6858ebdf9" />

Ahora crearemos un flujo de ventas, nos dirigiremos a ventas y presupuestos y le daremos a crear. Eligiremos un cliente cualquiera. 
Deberemos crear un producto para vender en mi caso voy a poner monitor, deberemos poner el precio etc.. una vez terminado lo creamos
<img width="1714" height="786" alt="image" src="https://github.com/user-attachments/assets/8c282365-eb73-4ed4-b37f-af4c316f9a57" />
Ahora confirmaremos la entrega, simplemente en el icono del camion pinchamos y lo validamos.
Ahora crearemos la factura, volvemos al pedido y le daremos a crear factura normal y ya estaria.

### Fase 2: Elaboración de Informes
En la pagina principal de odoo  nos ireemos a ajustes, una vez dentro buscamos la parte Tecnico despues en interfaz de usuario y vistas.
Ajustes → Técnico → Interfaz de usuario → Vistas
<img width="900" height="748" alt="image" src="https://github.com/user-attachments/assets/7e0cf2b7-c36a-490c-9b09-07ceb3453f6b" />
Una vez dentro en el buscador deberemos poner este archivo: sale.report_saleorder_document y buscarlo por clave 
<img width="610" height="269" alt="image" src="https://github.com/user-attachments/assets/7deaab98-1369-40b1-b764-f132e3e357cf" />
Una vez buscado clicamos y nos aparecera un XML bastante extenso, dentro del XML, al final (antes de </div>), añadimos los siguiente:
<div class="row mt32 mb32" id="legal_warning">
    <div class="col-12">
        <p style="color: red; font-weight: bold; border-top: 1px solid black; padding-top: 10px;">
            Atención: Este documento vinculante está sujeto a las condiciones generales de venta de DAM/DAW S.L. (CIF: B-12345678).
        </p>
        <p class="text-muted" style="font-size: 10px; text-align: justify;">
            Protección de datos: En cumplimiento de la Ley Orgánica 3/2018 y el RGPD europeo, le informamos que sus datos serán tratados de forma estrictamente confidencial.
        </p>
    </div>
</div>







