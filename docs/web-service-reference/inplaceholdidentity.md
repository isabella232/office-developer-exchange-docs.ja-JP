---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: InPlaceHoldIdentity 要素は、メールボックス アイテムを保持する保留リストの ID を指定します。
ms.openlocfilehash: 0a5f02b908adf49328461c6e3676dab3698879c3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547212"
---
# <a name="inplaceholdidentity"></a>InPlaceHoldIdentity

**InPlaceHoldIdentity** 要素は、メールボックス アイテムを保持する保留リストの ID を指定します。 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetHoldOnMailboxes](setholdonmailboxes.md)  | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>テキスト値

**InPlaceHoldIdentity 要素のテキスト** 値は、メールボックス保持識別子です。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

