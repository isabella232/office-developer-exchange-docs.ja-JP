---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: GlobalHasIrm 要素は、会話内の少なくとも1つのメッセージが IRM で保護されたメッセージであるかどうかを指定します。
ms.openlocfilehash: 10b99c9a6421a89a549b69e918087f3e542ffa09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459470"
---
# <a name="globalhasirm"></a>GlobalHasIrm

**Globalhasirm**要素は、会話内の少なくとも1つのメッセージが IRM で保護されたメッセージであるかどうかを指定します。 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[会話 (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>テキスト値

**Globalhasirm**要素のテキスト値は、会話内の少なくとも1つのメッセージが IRM で保護されたメッセージである場合は**true**です。 それ以外の場合、値は**false**になります。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[会話 (ConversationType)](conversation-conversationtype.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

