---
title: OnlineMeetingSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4c7af00c-8dca-40f4-9420-e042a0b5303c
description: OnlineMeetingSettings 要素は、オンライン会議の設定を指定します。
ms.openlocfilehash: dd830330ba1a09f04aca933853f4169e0cd78838
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832647"
---
# <a name="onlinemeetingsettings"></a>OnlineMeetingSettings

**OnlineMeetingSettings**要素は、オンライン会議の設定を指定します。 
  
```XML
<OnlineMeetingSettings>
   <LobbyBypass/>
   <AccessLevel/>
   <Presenters/>
</OnlineMeetingSettings>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[LobbyBypass](lobbybypass.md) | [AccessLevel](accesslevel.md) | [発表](presenters.md)
  
### <a name="parent-elements"></a>親要素

[カレンダー項目](calendaritem.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

