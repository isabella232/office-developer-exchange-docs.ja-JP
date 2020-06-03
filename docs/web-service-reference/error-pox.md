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
description: Error 要素には、自動検出エラー応答が含まれます。
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530650"
---
# <a name="error-pox"></a>エラー (POX)

**Error**要素には、自動検出エラー応答が含まれます。 
  
[自動検出 (POX)](autodiscover-pox.md)
  
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

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|Time  <br/> |エラー応答が返された時刻を表します。  <br/> |
|ID  <br/> |クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの名前のハッシュを表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ErrorCode (POX)](errorcode-pox.md) <br/> |エラー自動検出応答のエラーコードが含まれています。  <br/> |
|[メッセージ (POX)](message-pox.md) <br/> |エラー自動検出応答のエラーメッセージが含まれています。  <br/> |
|[DebugData (POX)](debugdata-pox.md) <br/> |エラー自動検出応答のデバッグデータが保存されています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[アカウント (POX)](account-pox.md) <br/> |自動検出エラー応答を格納します。  <br/> |
   
## <a name="see-also"></a>関連項目



[Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)

