---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: GetServerTimeZones 要素は、Exchange サーバーからタイムゾーン定義を取得するための要求のルート要素です。
ms.openlocfilehash: 797e4543c94b0628242bcf544fe9a735ebaa5a63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460940"
---
# <a name="getservertimezones"></a>GetServerTimeZones

**GetServerTimeZones**要素は、Exchange サーバーからタイムゾーン定義を取得するための要求のルート要素です。 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |[GetServerTimeZones 操作](getservertimezones-operation.md)が、各タイムゾーンの完全な定義または名前と識別子のみを返すかどうかを指定します。 この属性は省略可能です。 既定値は **true** です。  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>ReturnFullTimeZoneData 属性

|**値**|**説明**|
|:-----|:-----|
|**false** <br/> |各タイムゾーンの完全な定義を返します。  <br/> |
|**false** <br/> |各タイムゾーンの名前と識別子のみを返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Rid](ids.md) <br/> |要求されたタイムゾーン定義を指定するタイムゾーン定義識別子の配列を含みます。 この要素は省略できます。 この要素が[GetServerTimeZones 操作](getservertimezones-operation.md)要求に含まれていない場合、サーバー上で使用可能なすべてのタイムゾーン定義が応答で返されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetServerTimeZones 操作](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

