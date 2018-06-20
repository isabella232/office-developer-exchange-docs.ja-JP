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
description: GetServerTimeZones 要素は、Exchange サーバーからのタイム ゾーン定義を取得する要求のルート要素です。
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760862"
---
# <a name="getservertimezones"></a>GetServerTimeZones

**GetServerTimeZones**要素は、Exchange サーバーからのタイム ゾーン定義を取得する要求のルート要素です。 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 **GetServerTimeZonesType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ReturnFullTimeZoneData** <br/> |[GetServerTimeZones 操作](getservertimezones-operation.md)が完全な定義のみの名前や各タイム ゾーンの識別子を返すかどうかを指定します。 この属性は、省略可能です。 既定値は、 **true を指定**します。  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a>ReturnFullTimeZoneData 属性

|**値**|**説明**|
|:-----|:-----|
|**true** <br/> |各タイム ゾーンの完全な定義を返します。  <br/> |
|**false** <br/> |名と各タイム ゾーンの識別子を返します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Id](ids.md) <br/> |要求されたタイム ゾーン定義を指定するタイム ゾーン定義の識別子の配列が含まれています。 この要素はオプションです。 [GetServerTimeZones 操作](getservertimezones-operation.md)の要求には、この要素が含まれていない、サーバーで利用可能なすべてのタイム ゾーン定義が応答で返されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetServerTimeZones 操作](getservertimezones-operation.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

