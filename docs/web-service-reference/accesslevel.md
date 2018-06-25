---
title: AccessLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 09475586-00fa-4e82-a915-5ca263ab4d1c
description: AccessLevel 要素は、オンライン会議のアクセス レベルを指定します。
ms.openlocfilehash: 1bf0a191fad529b555117e4ff992c352615bc79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760420"
---
# <a name="accesslevel"></a>AccessLevel

**AccessLevel**要素は、オンライン会議のアクセス レベルを指定します。 
  
```XML
<AccessLevel/>
```

 **OnlineMeetingSettingsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[OnlineMeetingSettings](onlinemeetingsettings.md) <br/> |オンライン会議の設定を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**AccessLevel**要素のテキスト値を次の表に一覧します。 
  
**AccessLevel 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|全員  <br/> |アクセス レベルは、すべてに開かれています。  <br/> |
|内部  <br/> |アクセス レベルは、内部のみです。  <br/> |
|招待  <br/> |アクセス レベルとは、招待された参加者のみです。  <br/> |
|ロック  <br/> |アクセス レベルはロックされています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
この要素は Exchange Server 2013 で導入されました。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

