---
title: エラー (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: Error 要素には、自動検出エラー応答が含まれています。
ms.openlocfilehash: 3135a352365fe3000ce2d202ad78452d5c8ccc7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760318"
---
# <a name="error-pox"></a>エラー (POX)

**Error**要素には、自動検出エラー応答が含まれています。 
  
[(POX) を自動検出](autodiscover-pox.md)
  
[応答 (POX)](response-pox.md)
  
[アカウント (POX)](account-pox.md)
  
[エラー (POX)](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|時刻型 (Time)  <br/> |エラー応答が返された時刻を表します。  <br/> |
|ID  <br/> |クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの名前のハッシュを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[エラー コード (POX)](errorcode-pox.md) <br/> |エラー自動検出応答のエラー コードが含まれています。  <br/> |
|[メッセージ (POX)](message-pox.md) <br/> |エラー自動検出応答のエラー メッセージが含まれています。  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |自動検出応答エラーのデバッグ データを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |自動検出エラー応答が含まれています。  <br/> |
   
## <a name="see-also"></a>関連項目



[交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

