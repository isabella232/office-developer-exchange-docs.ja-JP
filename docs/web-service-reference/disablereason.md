---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: DisableReason 要素は、アプリを無効にする理由を指定します。
ms.openlocfilehash: 1406d69647bde5389dc9bb61adf7537a57d5adfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463672"
---
# <a name="disablereason"></a>DisableReason

**DisableReason**要素は、アプリを無効にする理由を指定します。 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 **DisableReasonType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[DisableApp](disableapp.md) <br/> |アプリを無効にする要求を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**DisableReason 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|NoReason  <br/> |理由の指定なし  <br/> |
|OutlookClientPerformance  <br/> |電子メールクライアントのパフォーマンスを向上させるため。  <br/> |
|OWAClientPerformance  <br/> |Web アプリクライアントのパフォーマンスを向上させる。  <br/> |
|MobileClientPerformance  <br/> |モバイルクライアントのパフォーマンスを向上させる。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

