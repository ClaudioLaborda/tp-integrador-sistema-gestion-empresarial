# Trabajo Práctico Integrador — Sistemas de Gestión Empresarial

Implementación de un circuito integral de gestión comercial, abastecimiento, inventario y
facturación sobre **ERPNext** (Frappe Framework), desarrollado para la cátedra
**Sistemas de Gestión Empresarial** de la Tecnicatura Universitaria en Tecnologías de la Información (UTN — Facultad Regional Santa Fe).

## Alcance del Proyecto

Simulación de la operatoria completa de una empresa distribuidora bajo esquema de inventario perpetuo, 
garantizando la trazabilidad documentaria entre módulos:

* **Inventario:** Configuración de depósitos, alta de artículos y apertura inicial de stock mediante conciliación.
* **CRM y Ventas:** Captación y calificación desde *Lead* y *Prospect*, oportunidades, cotizaciones,
* conversión a clientes sin duplicados y pedidos de venta.
* **Compras:** Solicitudes de materiales, pedidos de cotización, ofertas de proveedor, órdenes de compra,
* recepción en almacén y facturas de compra.
* **Logística y Facturación:** Remitos de entrega, facturas de venta vinculadas y análisis contable de costos y márgenes.

## Entorno y Documentación

* **Instancia ERPNext (GitHub Codespaces):** https://fluffy-enigma-wrx5rpx4xjqhv4g-8000.app.github.dev/
* **Informe Técnico Completo:** [`Informe Trabajo Practico ERP.pdf`](./Informe%20Trabajo%20Practico%20ERP.pdf)

## Levantar y Apagar el Entorno

### 1. Iniciar el entorno (Levantar)
1. Abrir el Codespace del laboratorio desde GitHub.
2. En la terminal integrada (dentro del directorio `frappe-bench`), iniciar los servicios base y levantar ERPNext:
   ```bash
   sudo service mariadb start
   sudo service redis-server start
   bench start
   ```
3. Abrir el enlace del puerto **8000** (verificar que esté en visibilidad **Public** para la defensa) e iniciar sesión en ERPNext.

### 2. Detener el entorno (Apagar)
1. En la terminal donde se ejecuta `bench start`, presionar `Ctrl + C` para detener los servicios de forma ordenada.
2. Detener el contenedor desde la paleta de comandos (`Ctrl + Shift + P` → *Codespaces: Stop Current Codespace*) o desde el panel de Codespaces en GitHub para evitar el consumo innecesario de horas.

## Integrantes

Claudio Oscar Laborda · Cristian Hernan Marcos Nozralah · Lucas Rojas
