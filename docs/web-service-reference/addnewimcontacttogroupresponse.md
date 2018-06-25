---
title: AddNewImContactToGroupResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e1a1c5fa-9e1e-4ee7-bb19-77c29b47ecbb
description: AddNewImContactToGroupResponse 要素は、AddNewImContactToGroup 要求への応答を定義します。
ms.openlocfilehash: dedd5587fd4deef1287b377084c1a4bcfc91e80c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759291"
---
# <a name="addnewimcontacttogroupresponse"></a>AddNewImContactToGroupResponse

**AddNewImContactToGroupResponse**要素は、 **AddNewImContactToGroup**要求への応答を定義します。 
  
```XML
<AddNewImContactToGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</AddNewImContactToGroupResponse>
```

 **AddNewImContactToGroupResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[メッセージ テキスト](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ペルソナ](persona.md)
  
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
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

