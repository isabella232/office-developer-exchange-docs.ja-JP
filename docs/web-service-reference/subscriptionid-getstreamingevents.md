---
title: サブスクリプション Id (GetStreamingEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f86c178-2311-4844-82db-c2a0e469d116
description: サブスクリプション Id 要素は、ストリーミングのサブスクリプションの識別子を表します。
ms.openlocfilehash: eb451e611c4922fa3b9cff7edec54dfb8260f5f5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839618"
---
# <a name="subscriptionid-getstreamingevents"></a>サブスクリプション Id (GetStreamingEvents)

**サブスクリプション Id**要素は、ストリーミングのサブスクリプションの識別子を表します。 
  
```XML
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetStreamingEvents](getstreamingevents.md) <br/> |サーバーからストリーミングの通知を要求するクライアントによって使用される演算を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、GUID です。
  
## <a name="remarks"></a>備考

サブスクリプションの識別子を表す GUID は、サブスクリプションが作成されると、クライアント アクセス サーバーによって生成されます。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetStreamingEvents の操作](getstreamingevents-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

