---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: HiddenRecipient 要素は、権限のないユーザーから非表示にする必要がある組織のポリシーによって受信者が追加されたことを示します。
ms.openlocfilehash: bfe57fabc02ff00c801672b71ccdb0bf1b916bd9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457642"
---
# <a name="hiddenrecipient"></a>HiddenRecipient

**HiddenRecipient**要素は、権限のないユーザーから非表示にする必要がある組織のポリシーによって受信者が追加されたことを示します。 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
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
|[受信者 Trackingイベント](recipienttrackingevent.md) <br/> |受信者に対する1つのイベントに関する情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素は、 **true**または**false**のいずれかになります。 値**true**は、ユーザーが組織のポリシーによって追加されたことを示します。値が**false**の場合は、ユーザーが組織のポリシーによって追加されていないことを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

