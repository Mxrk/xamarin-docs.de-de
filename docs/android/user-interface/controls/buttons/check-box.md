---
title: CheckBox
ms.prod: xamarin
ms.assetid: A884AF10-D5EA-72CA-2301-B80CEC7FFBE7
ms.technology: xamarin-android
author: conceptdev
ms.author: crdun
ms.date: 02/06/2018
ms.openlocfilehash: f6f594d86cab8b1173ee9f67402862e1ec2890b2
ms.sourcegitcommit: b07e0259d7b30413673a793ebf4aec2b75bb9285
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/26/2019
ms.locfileid: "68510369"
---
# <a name="checkbox"></a>CheckBox

In diesem Abschnitt erstellen Sie ein Kontrollkästchen für die Auswahl von Elementen, indem Sie das[`CheckBox`](xref:Android.Widget.CheckBox)
Widget verwenden. Wenn das Kontrollkästchen gedrückt ist, gibt eine Popup-Meldung den aktuellen Zustand an.

Öffnen Sie die Datei **Resources/Layout/Main. axml** und fügen Sie das [`CheckBox`](xref:Android.Widget.CheckBox) Element (innerhalb des [`LinearLayout`](xref:Android.Widget.LinearLayout) Elements)hinzu:

```xml
<CheckBox android:id="@+id/checkbox"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="check it out" />
```

Um etwas zu tun, wenn der Status geändert wird, fügen Sie den folgenden Code am Ende der [`OnCreate()`](xref:Android.App.Activity.OnCreate*) Methode hinzu:

```csharp
CheckBox checkbox = FindViewById<CheckBox>(Resource.Id.checkbox);

checkbox.Click += (o, e) => {
    if (checkbox.Checked)
        Toast.MakeText (this, "Selected", ToastLength.Short).Show ();
    else
        Toast.MakeText (this, "Not selected", ToastLength.Short).Show ();
};
```

Dadurch wird das [`CheckBox`](xref:Android.Widget.CheckBox)-Element aus dem Layout erfasst, anschließend das Klick-Ereignis behandelt, das die Aktion definiert, die beim Klicken auf das Kontrollkästchen ausgeführt werden soll. Wenn Sie darauf klicken, wird die [`Checked`](xref:Android.Widget.CompoundButton.Checked)
Eigenschaft aufgerufen, um den neuen Zustand des Kontrollkästchens zu überprüfen. Wenn das Kontrollkästchen aktiviert ist, wird ein [`Toast`](xref:Android.Widget.Toast) mit der Meldung "ausgewählt" angezeigt, andernfalls wird "nicht ausgewählt" angezeigt. Die [`CheckBox`](xref:Android.Widget.CheckBox)
verarbeitet seine eigenen Zustandsänderungen, sodass Sie nur den aktuellen Statusabfragen müssen.

Führen Sie es aus.

> [!TIP]
> Wenn Sie den Zustand selbst ändern müssen (z. B. beim Laden einer gespeicherten [`CheckBoxPreference`](xref:Android.Preferences.CheckBoxPreference), verwenden Sie den Setter der [`Checked`](xref:Android.Widget.CompoundButton.Checked)
> Eigenschaft oder die[`Toggle()`](xref:Android.Widget.CompoundButton.Toggle)
> -Methode.

*Teile dieser Seite sind Änderungen, die auf der vom Android Open Source-Projekt erstellten und freigegebenen Arbeit basieren und gemäß den in der*
[*Creative Commons 2,5-Zuweisungs Lizenz*](http://creativecommons.org/licenses/by/2.5/)beschriebenen Begriffen verwendet werden.
