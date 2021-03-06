---
title: Técnicas de procesamiento en segundo plano de iOS
description: 'Este documento se vincula a las guías que describen diversas técnicas backgrounding en iOS: tareas en segundo plano, servicio de transferencia en segundo plano, captura de fondo y las notificaciones remotas.'
ms.prod: xamarin
ms.assetid: 011A8D48-1CDC-486A-A2B0-C4946118E7A9
ms.technology: xamarin-ios
author: bradumbaugh
ms.author: brumbaug
ms.date: 03/18/2017
ms.openlocfilehash: 33c4613e3698556b41a0d01acf2a4ac359ca5dd8
ms.sourcegitcommit: aa9b9b203ab4cd6a6b4fd51e27d865e2abf582c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/30/2018
ms.locfileid: "39350974"
---
# <a name="ios-backgrounding-techniques"></a>Técnicas de procesamiento en segundo plano de iOS

En las secciones siguientes, exploraremos las siguientes características de iOS junto con las opciones de backgrounding existentes:

-  [Tareas en segundo plano oportunista](~/ios/app-fundamentals/backgrounding/ios-backgrounding-techniques/ios-backgrounding-with-tasks.md#background_tasks_in_iOS_7) -conservar la duración de la batería mediante la ejecución de tareas en segundo plano en fragmentos oportunistas cuando el dispositivo está activo para otro procesamiento.
-  [Servicio de transferencia en segundo plano](~/ios/app-fundamentals/backgrounding/ios-backgrounding-techniques/ios-backgrounding-with-tasks.md#background-transfers) : confiable cargar y descargar archivos, independientemente del tamaño de archivo o el estado de la red.
-  [Captura de fondo](~/ios/app-fundamentals/backgrounding/ios-backgrounding-techniques/updating-an-application-in-the-background.md#background_fetch) -actualización de una aplicación en segundo plano a intervalos determinados en el sistema.
-  [Notificaciones remotas](~/ios/app-fundamentals/backgrounding/ios-backgrounding-techniques/updating-an-application-in-the-background.md#remote_notifications) -usar las notificaciones de inserción para desencadenar las actualizaciones de contenido en segundo plano antes de que el usuario abre la aplicación, con una opción para notificar al usuario o actualizar de forma silenciosa.
-  **En segundo plano las actualizaciones de la interfaz de usuario** : preparar la aplicación de interfaz de usuario para el usuario y actualizar la instantánea de la aplicación, todo ello desde el fondo.
