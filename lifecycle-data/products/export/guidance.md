---
title: Guía de exportación de datos del ciclo de vida
description: Guía para exportar información del ciclo de vida del producto
ms.date: 12/16/2020
layout: ContentPage
ms.openlocfilehash: 5e9dddbff5fac32e6d3cf8ef0943151d2dfe5e35
ms.sourcegitcommit: 6ea3221fd5475440480515f04f33988656d71748
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/02/2021
ms.locfileid: "3546873"
---
# <a name="lifecycle-data-export-guidance"></a>Guía de exportación de datos del ciclo de vida
En este documento se describe cómo usar el archivo de exportación del producto.

## <a name="query-information"></a>Información de consultas
En el documento Excel hay campos que ayudan a identificar los datos rellenados en la tabla de productos.

### <a name="end-of-support"></a>Finalización del soporte
El valor "finalización del soporte" filtrará los productos según la fecha de finalización de soporte del producto o las fechas de finalización de la versión.

Valores posibles: Todos (sin filtro aplicado), Año y un Intervalo.

### <a name="family"></a>Familia
El valor "familia" filtra los productos por su nivel primario dentro de la jerarquía conocida como familia.

Valores posibles: Todos (sin filtro aplicado), Nombre de familia

### <a name="group"></a>Grupo
El valor "grupo" filtra los productos dentro de su nivel primario (familia) a un grupo específico.

Valores posibles: Todos (sin filtro aplicado), Nombre de grupo

## <a name="table-columns"></a>Columnas de la tabla
La tabla de productos consta de columnas que definen el producto, las ediciones, las versiones y las fechas de soporte correspondientes.

> [!NOTE]
> Habrá una fila para cada combinación de producto, edición y versión.

### <a name="product"></a>Producto
El nombre del producto.

### <a name="edition"></a>Edición
La columna "edición" se rellenará si el producto contiene ediciones. Si no hay ninguna edición del producto, este campo estará en blanco.

### <a name="release"></a>Release
La columna "versión" se rellenará si el producto tiene varias versiones.
Si el producto solo tiene una versión, este campo estará en blanco.

### <a name="support-policy"></a>Directiva de soporte técnico
Este campo define por qué directiva de soporte técnico se rige el producto.

Valores posibles: [Fija](/lifecycle/policies/fixed), [Moderna](/lifecycle/policies/modern), Componente

### <a name="start-date"></a>Fecha de inicio
La fecha en que se inició el soporte del producto.

### <a name="mainstream-date"></a>Fecha de soporte estándar
Si la directiva de soporte técnico es **Fija** o del **Componente**, esta es la fecha de finalización del soporte estándar del producto.
  
Si la directiva de soporte técnico es **Moderna**, estará en blanco.

### <a name="extended-end-date"></a>Fecha de finalización del soporte extendido
Si la directiva de soporte técnico es **Fija** o del **Componente**, esta es la fecha de finalización del soporte extendido del producto.

Si la directiva de soporte técnico es **Moderna**, estará en blanco.

### <a name="retirement-date"></a>Fecha de retirada
Si la directiva de soporte técnico es **Fija** o del **Componente**, estará en blanco.

Si la directiva de soporte técnico es **Moderna**, esta será la fecha de retirada del producto.

### <a name="release-start-date"></a>Fecha de inicio de la versión
La fecha en que se inició el soporte de la versión. Si el producto solo tiene una versión, este campo estará en blanco.
 
### <a name="release-end-date"></a>Fecha de finalización de la versión
La fecha en la que el soporte técnico finalizó para la versión.
Si el producto solo tiene una versión, este campo estará en blanco.

### <a name="docs-url"></a>Dirección URL de documentos
Dirección URL a documentación más detallada.
