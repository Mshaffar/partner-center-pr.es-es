---
title: Escenarios comunes de facturación mensual
ms.topic: article
ms.date: 05/13/2020
description: 'Escenarios comunes en el centro de Partners cuando se usa la facturación mensual: incluye la adición de nuevas suscripciones, el cambio de la cantidad de licencias y la suspensión de suscripciones.'
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: facturación, pagos, pedidos, uso, facturación mensual, suscripciones, archivo de conciliación
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c51e6dfa2471570f30b1b957317bff1e6081bb79
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795623"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Ejemplos de escenarios de facturación mensuales para nuevas suscripciones, cambios de cantidades de licencias o suspensiones

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas

Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) son aplicables si usa la facturación mensual en el centro de Partners.

## <a name="new-monthly-subscription"></a>Nueva suscripción mensual

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00 |

El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Tarifa de ciclo   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Cambiar cantidad de licencias

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00    |

El 1 de febrero aumenta la cantidad de licencias de uno a dos. El archivo de conciliación basado en licencias del 15 de febrero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |12/2/2018    |Prorrateo de instancia de ciclo   |-4,00       |1        |-4,00   |
|1/13/2018         |31/1/2018    | Prorrateo de instancia de ciclo   |2.45       |1        |2.45    |
|1/2/2018         |12/2/2018    | Prorrateo de instancia de ciclo   |1.55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Prorrateo de instancia de ciclo   |4.00       |2        |8.00    |

El precio mensual es 4,00 y hay 31 días en el período de servicio 1/13/2018 – 2/12/2018. Esto equivale a un precio diario de 0,129 (4/31).

Hay 19 días en el período de proporciones 1/13/2018 a 1/31/2018.

Precio por unidad de proporciones = 2,451 = 19 x 0,129

Hay 12 días en el período de proporciones 2/1/2018 a 2/12/2018.

Precio por unidad de proporciones = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspender antes de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00    |

El 1 de febrero suspende una suscripción. El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Cuota de cancelación|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspender después de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Precio del ciclo|4.00|1|4.00

El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Precio del ciclo|4.00|1|4.00

El 1 de marzo se suspende la suscripción. El archivo de conciliación basado en licencias del 15 de marzo contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Cuota de cancelación|-1,72|1|-1,72

El precio mensual es 4,00 y hay 28 días en el período de servicio 2/13/2018 – 3/12/2018. Esto equivale a un precio diario de 0,143 (4/28).

Precio por unidad = días del período de servicio x precio diario x número de licencias.

Hay 12 días en el período de cancelación 3/1/2018 a 3/12/2018.

Por lo tanto, el precio por unidad =-1,716 (12 x 0,143 x (-1)).
