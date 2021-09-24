---
title: AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cff8ef19-3e19-4107-9b35-c8a2b87a41bc
description: AddNewTelUriContactToGroup 要素は、AddNewTelUriContactToGroup WSDL 操作の入力データを指定します。
ms.openlocfilehash: 0d260679da8ca1ae78afef200f047263808d6e32
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522181"
---
# <a name="addnewteluricontacttogroup"></a>AddNewTelUriContactToGroup

**AddNewTelUriContactToGroup** 要素は **、AddNewTelUriContactToGroup** WSDL 操作の入力データを指定します。 
  
```XML
<AddNewTelUriContactToGroup>
   <TelUriAddress/>
   <ImContactSipUriAddress/>
   <ImTelephoneNumber/>
   <GroupId/>
</AddNewTelUriContactToGroup>
```

 **AddNewTelUriContactToGroupType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[TelUriAddress](teluriaddress.md)  | [ImContactSipUriAddress](imcontactsipuriaddress.md)  | [ImTelephoneNumber](imtelephonenumber.md)  | [GroupId](groupid.md)
  
### <a name="parent-elements"></a>親要素

なし。
  
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

- [AddNewTelUriContactToGroup 操作](addnewteluricontacttogroup-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

