---
title: AddNewTelUriContactToGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abff2306-a3a7-489a-b548-2edbc1eb5cc4
description: AddNewTelUriContactToGroupResponse 要素は、AddNewTelUriContactToGroup WSDL 操作の結果データを指定します。
ms.openlocfilehash: dfbf208cd5fc59902b16661658985442d4fa57e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464918"
---
# <a name="addnewteluricontacttogroupresponse"></a>AddNewTelUriContactToGroupResponse

**AddNewTelUriContactToGroupResponse**要素は、 **AddNewTelUriContactToGroup** WSDL 操作の結果データを指定します。 
  
```XML
<AddNewTelUriContactToGroupResponse>
   <Persona/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
</AddNewTelUriContactToGroupResponse>
```

 **AddNewTelUriContactToGroupResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Persona](persona.md)  | [Messagetext](messagetext.md)  | 応答[Secmode](responsecode.md)  | [DescriptiveLinkKey](descriptivelinkkey.md)
  
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
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [AddNewTelUriContactToGroup 操作](addnewteluricontacttogroup-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

