---
title: AddNewTelUriContactToGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abff2306-a3a7-489a-b548-2edbc1eb5cc4
description: AddNewTelUriContactToGroupResponse 要素は、AddNewTelUriContactToGroup の WSDL 操作の結果のデータを指定します。
ms.openlocfilehash: ddf038af2f4dec8cff98c4453e867af1fe7b8076
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759296"
---
# <a name="addnewteluricontacttogroupresponse"></a>AddNewTelUriContactToGroupResponse

**AddNewTelUriContactToGroupResponse**要素は、 **AddNewTelUriContactToGroup**の WSDL 操作の結果のデータを指定します。 
  
```XML
<AddNewTelUriContactToGroupResponse>
   <Persona/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
</AddNewTelUriContactToGroupResponse>
```

 **AddNewTelUriContactToGroupResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ペルソナ](persona.md) | [メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
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

- [AddNewTelUriContactToGroup 操作](addnewteluricontacttogroup-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

