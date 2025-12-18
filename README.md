# Gasolinera

## Enunciado

A una gasolinera llegan vehículos según una Exponencial de media 2 minutos.
Los vehículos pueden ser de tres tipos, y la probabilidad de que sea de uno
de dichos tipos es:

| Tipo | Vehículo  | Probabilidad |
|------|-----------|--------------|
| 1    | TURISMO   | 75%          |
| 2    | FURGONETA | 15%          |
| 3    | CAMIÓN    | 10%          |

La gasolinera tiene 2 servicios: **llenado del depósito** y **lavado de vehículos**. Todos los de tipo 2 y 3 entran sólo al llenado del depósito, mientras que el 67% de los TURISMOS (tipo 1) van a llenar su depósito y el 33% restante de los TURISMOS van a lavarlo.

Para el **lavado de coches** hay un encargado todo el día, y el tiempo de lavado dura según una Normal de media 5 min y desviación típica 0.5 min. El carril de espera sólo permite 3 vehículos así que el resto se va.

Para el **llenado del depósito** de vehículos hay diez surtidores de cuatro tipos: GASOLEO-A (2 surtidores) (goa), GASOLEO-A+ (2 surtidores) (go+), GASOLINA 95 (4 surtidores) (ga95), GASOLINA 98 (2 surtidores) (ga98). Los vehículos tipo 3 utilizan goa, los de tipo 2 go+, los de tipo 1 el 80% ga95 y el 20% ga98.

La gasolinera está distribuida de tal forma que los surtidores pueden considerarse como carriles independientes. Los vehículos que llegan se sitúan en el carril que menos vehículos tenga. Hay 2 empleados para el llenado del depósito durante la noche (desde las 0.00 h. a las 7.00) y 3 empleados el resto del día.

Cuando el surtidor se queda libre, el vehículo se sitúa delante y el propietario abre su depósito (**tiempo inicial**); después uno de los empleados le llena el depósito (**tiempo de llenado**); al final cierra el depósito, arranca y se va (**tiempo final**); todos los tiempos se distribuyen según una Uniforme entre los siguientes valores para cada tipo de vehículo:

| Tipo | T. Inicial     | T. Llenado      | T. Final       |
|------|----------------|-----------------|----------------|
| 1    | UNIF(0.3, 0.8) | UNIF(3.5, 4.5)  | UNIF(0.5, 1)   |
| 2    | UNIF(0.5, 1)   | UNIF(5,6)       | UNIF(0.7, 1.2) |
| 3    | UNIF(0.5, 1)   | UNIF(8.5, 10.5) | UNIF(0.7, 1.2) |

Realice una simulación en Arena de 3 días de funcionamiento usando los datos que se proporcionan. Calcular:
- Los tiempos medios en el llenado del depósito de cada tipo de vehículo y en el lavado de los tipo 1.
- El número medio de vehículos esperando en cada carril a que su surtidor quede libre.
- El número medio de vehículos situados en los surtidores esperando ser atendidos por los empleados.
- La utilización de cada surtidor.
- La utilización de los empleados y del encargado.
- El número medio de espera en lavado.
- El tiempo medio entre abandonos en lavado.

Analice el modelo y proponga una mejora asociada al aumento del/los recursos crítico/s y/o disminución de los recursos infrautilizados.
