---
title: Error (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: Error 要素には、自動検出エラー応答が含まれる。
ms.openlocfilehash: 2f96f8b9d6d154aac6f10924095b5a5864e76750
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530890"
---
# <a name="error-pox"></a>Error (POX)

**Error 要素** には、自動検出エラー応答が含まれる。 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Error (POX)](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Time  <br/> |エラー応答が返された時刻を表します。  <br/> |
|ID  <br/> |クライアント アクセス サーバーの役割がインストールされている 2007 Microsoft Exchange Serverコンピューターの名前のハッシュを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |エラー自動検出応答のエラー コードが含まれる。  <br/> |
|[Message (POX)](message-pox.md) <br/> |エラー自動検出応答のエラー メッセージが含まれる。  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |エラー自動検出応答のデバッグ データを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |自動検出エラー応答が含まれる。  <br/> |
   
## <a name="see-also"></a>関連項目



[POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)

