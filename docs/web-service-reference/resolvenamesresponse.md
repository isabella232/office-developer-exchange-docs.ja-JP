---
title: ResolveNamesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponse
api_type:
- schema
ms.assetid: 5e7be1e2-44ea-403f-9135-2388d030078c
description: ResolveNamesResponse 要素は、ResolveNames 要求への応答を定義します。
ms.openlocfilehash: 686a7b2799f32ab9017cfe786f6dff8c67f0b98c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833164"
---
# <a name="resolvenamesresponse"></a>ResolveNamesResponse

**ResolveNamesResponse**要素は、ResolveNames 要求への応答を定義します。 
  
```xml
<ResolveNamesResponse>
   <ResponseMessages/>
</ResolveNamesResponse>
```

 **ResolveNamesResponseType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
[ResolveNames 操作](resolvenames-operation.md)

