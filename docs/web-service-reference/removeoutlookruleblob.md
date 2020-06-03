---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: RemoveOutlookRuleBlob 要素は、Microsoft Outlook のルール blob を削除するかどうかを示します。
ms.openlocfilehash: b4202ab52bf16d1ad1546ec963cd8b9dacd2bd63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467670"
---
# <a name="removeoutlookruleblob"></a>RemoveOutlookRuleBlob

**Removeoutlookruleblob**要素は、Microsoft Outlook のルール blob を削除するかどうかを示します。 
  
[UpdateInboxRules](updateinboxrules.md)
  
[RemoveOutlookRuleBlob](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UpdateInboxRules](updateinboxrules.md) <br/> |サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値が**true の場合**は、Outlook ルール blob を削除する必要があることを示します。 テキスト値が**false**の場合は、Outlook ルール blob を削除しないようにする必要があります。 
  
## <a name="remarks"></a>注釈

受信トレイルールの更新を許可するには、この要素を**true**に設定します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[UpdateInboxRules の操作](updateinboxrules-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

