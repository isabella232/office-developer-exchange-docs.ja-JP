---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: GetServerTimeZones 要素は、サーバーからタイム ゾーン定義を取得する要求のルートExchangeです。
ms.openlocfilehash: b710334e5778f8bc27ba7ac07c6bf9c2e2d3392e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533540"
---
# <a name="getservertimezones"></a>GetServerTimeZones

**GetServerTimeZones** 要素は、サーバーからタイム ゾーン定義を取得する要求のルートExchangeです。 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |[GetServerTimeZones](getservertimezones-operation.md)操作が完全な定義を返すのか、各タイム ゾーンの名前と識別子のみを返すのかを指定します。 この属性は省略可能です。 既定値は **true** です。  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>ReturnFullTimeZoneData 属性

|**値**|**説明**|
|:-----|:-----|
|**true** <br/> |各タイム ゾーンの完全な定義を返します。  <br/> |
|**false** <br/> |各タイム ゾーンの名前と識別子のみを返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Ids](ids.md) <br/> |要求されたタイム ゾーン定義を指定するタイム ゾーン定義識別子の配列を格納します。 この要素は省略できます。 この要素が [GetServerTimeZones](getservertimezones-operation.md) 操作要求に含まれていない場合、サーバーで使用可能なすべてのタイム ゾーン定義が応答で返されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetServerTimeZones 操作](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

