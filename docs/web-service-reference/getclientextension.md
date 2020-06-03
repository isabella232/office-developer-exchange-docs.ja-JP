---
title: GetClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c96c2b4c-45cb-482a-a3bb-7a11a0fff43b
description: GetClientExtension 要素は、クライアント拡張機能を取得する要求を表します。
ms.openlocfilehash: caa069195a3b82af4e5b5984dcb6e4124b11899b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526341"
---
# <a name="getclientextension"></a>GetClientExtension

**Getclientextension**要素は、クライアント拡張機能を取得する要求を表します。 
  
```XML
<GetClientExtension>
   <RequestedExtensionIds/>
   <UserParameters/>
   <IsDebug/>
</GetClientExtension>
```

 ****
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[RequestedExtensionIds](requestedextensionids.md)  | [Userparameters](userparameters.md)  | [Isdebug](isdebug.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

