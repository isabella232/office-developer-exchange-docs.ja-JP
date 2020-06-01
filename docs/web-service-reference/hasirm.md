---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: HasIrm 要素は、会話内の少なくとも1つのメッセージと現在のフォルダーが IRM で保護されたメッセージであるかどうかを指定します。
ms.openlocfilehash: 1596610ed5f6b2bac353900624fbec9140aaa693
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462781"
---
# <a name="hasirm"></a>HasIrm

**Hasirm**要素は、会話内の少なくとも1つのメッセージと現在のフォルダーが IRM で保護されたメッセージであるかどうかを指定します。 
  
```XML
<HasIrm> true | false </HasIrm>
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

スレッドに少なくとも1つのメッセージがあり、現在のフォルダーに IRM がある場合は、 **Hasirm**要素のテキスト値は**true**です。 それ以外の場合、値は**false**になります。
  
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

