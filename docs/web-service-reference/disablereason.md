---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: DisableReason 要素は、アプリケーションを無効にする理由を指定します。
ms.openlocfilehash: f900bd1b98b294900f767c778b9c5f87f74042ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760069"
---
# <a name="disablereason"></a>DisableReason

**DisableReason**要素は、アプリケーションを無効にする理由を指定します。 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 **DisableReasonType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DisableApp](disableapp.md) <br/> |アプリケーションを無効にする要求を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**DisableReason 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|NoReason  <br/> |理由指定なし  <br/> |
|OutlookClientPerformance  <br/> |電子メール クライアントのパフォーマンスを向上させるには。  <br/> |
|OWAClientPerformance  <br/> |Web アプリケーションのクライアントのパフォーマンスを向上します。  <br/> |
|MobileClientPerformance  <br/> |モバイル クライアントのパフォーマンスを向上させるには。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

