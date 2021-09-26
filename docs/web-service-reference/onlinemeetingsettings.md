---
title: OnlineMeetingSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4c7af00c-8dca-40f4-9420-e042a0b5303c
description: OnlineMeetingSettings 要素は、オンライン会議の設定を指定します。
ms.openlocfilehash: 22942f181ca4be5a9c831db9d3649e64190d97d8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541932"
---
# <a name="onlinemeetingsettings"></a>OnlineMeetingSettings

**OnlineMeetingSettings** 要素は、オンライン会議の設定を指定します。 
  
```XML
<OnlineMeetingSettings>
   <LobbyBypass/>
   <AccessLevel/>
   <Presenters/>
</OnlineMeetingSettings>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[LobbyBypass](lobbybypass.md)  | [AccessLevel](accesslevel.md)  | [発表者](presenters.md)
  
### <a name="parent-elements"></a>親要素

[CalendarItem](calendaritem.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

