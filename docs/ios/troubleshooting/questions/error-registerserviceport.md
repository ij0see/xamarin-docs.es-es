---
title: Error de iOS Designer con RegisterServicePort
ms.topic: troubleshooting
ms.prod: xamarin
ms.assetid: 929A0080-B126-4744-BF88-A4A1EFBB6CC2
ms.technology: xamarin-ios
author: bradumbaugh
ms.author: brumbaug
ms.date: 04/03/2018
ms.openlocfilehash: 9edcc822b170c3463908b9f5fb1db8b798346e3e
ms.sourcegitcommit: aa9b9b203ab4cd6a6b4fd51e27d865e2abf582c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/30/2018
ms.locfileid: "39350711"
---
# <a name="ios-designer-error-with-registerserviceport"></a>Error de iOS Designer con RegisterServicePort

## <a name="sample-error"></a>Error de ejemplo
> System.AggregateException: Se produjeron uno o más errores,---> System.SystemException: RegisterServicePort (com.xamarin.MTHosting.2a0b1, com.apple.PowerManagement.control): Kernel devuelto: -308 (-308): servidor (ipc/mig) muerto

## <a name="explanation"></a>Explicación
Errores con `RegisterServicePort` y mensajes de error similares al igual que anteriormente suelen ser un problema con spyware o software malintencionado en el equipo. Tenga en cuenta la [comentario en este informe de errores](https://bugzilla.xamarin.com/show_bug.cgi?id=21907#c4) para obtener más información, junto con el vínculo a la [foro de debate de Apple](https://discussions.apple.com/thread/5596008) acerca de cómo quitar una posible infección. 

Para ayudar a diagnosticar el problema, abra la aplicación macOS **consola** y elimine todos los archivos dentro de la **informes de diagnóstico de usuario** sección [ http://screencast.com/t/y9i3NKcuMy ](http://screencast.com/t/y9i3NKcuMy). A continuación, inicie Visual Studio para Mac e intenta utilizar el diseñador. Si los nuevos archivos de registro aparecen en esta sección después de que el diseñador no pudo inicializar, guarde estos para que podamos analizar.  

Tenga en cuenta que es lo más importante para que busque el archivo: 
> /usr/lib/libimckit.dylib

Independientemente de los resultados anteriores, si no existe ese archivo, el problema de malware o spyware mencionado anteriormente está presente en el equipo.  

El siguiente vínculo consta de los pasos para quitar este malware y spyware: [http://www.thesafemac.com/arg-genieo/](http://www.thesafemac.com/arg-genieo/)  

