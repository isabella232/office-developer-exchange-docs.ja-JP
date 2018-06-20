---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: InPlaceHoldIdentity 要素は、メールボックス アイテムを保持する保留リストの id を指定します。
ms.openlocfilehash: 954e6ad6c3e0b7786d6bbb8230dba913a32359bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831938"
---
# <a name="inplaceholdidentity"></a>InPlaceHoldIdentity

**InPlaceHoldIdentity**要素は、メールボックス アイテムを保持する保留リストの id を指定します。 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>テキスト値

**InPlaceHoldIdentity**要素のテキスト値は、メールボックスの保留中の識別子です。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

