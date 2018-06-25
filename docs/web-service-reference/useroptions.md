---
title: UserOptions
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1acbb8a3-9110-4427-a06c-7e6e627e969f
description: UserOptions 要素は、返信メッセージのオプションの一覧を指定します。
ms.openlocfilehash: 8a5bdbc254e3c0bce8822633d2714bc928f15f13
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839941"
---
# <a name="useroptions"></a>UserOptions

**UserOptions**要素は、メッセージの返信のオプションの一覧を指定します。 
  
```XML
<UserOptions>
   <VotingOptionData>
</UserOptions>
```

 **ArrayOfVotingOptionDataType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[VotingOptionData](votingoptiondata.md)
  
### <a name="parent-elements"></a>親要素

[VotingInformation](votinginformation.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[VotingInformation](votinginformation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

