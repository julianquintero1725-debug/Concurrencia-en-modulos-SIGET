# Concurrencia en el SIGET - Productor y Consumidor

Este repositorio contiene la tarea de concurrencia del curso Sistemas Operativos, donde se simula un escenario del SIGET (Sistema Inteligente de Gestión del Tráfico) usando el problema clásico de productor-consumidor.

## De qué trata

Se simulan 2 sensores de tráfico (productores) que generan datos y los guardan en un buffer compartido, mientras un módulo de análisis (consumidor) los va procesando. Los 3 corren al mismo tiempo como hilos concurrentes.

Para evitar que se pierdan o se dañen datos, la solución usa:

- **Semáforos**: uno cuenta los espacios vacíos del buffer y otro los datos listos para procesar.
- **Mutex**: para que solo un hilo a la vez pueda tocar el buffer compartido.

## Archivos

- `simulador_siget_productor_consumidor.cpp` — código fuente de la simulación.
- `relatoria_concurrencia_siget.pdf` — relatoría técnica con la explicación de la lógica y las conclusiones.
- Video de evidencia de ejecución (link o archivo, según cómo se haya subido).

## Cómo compilar y ejecutar

Se necesita un compilador con soporte para C++20.

## Autor

Julian Quintero Copete
