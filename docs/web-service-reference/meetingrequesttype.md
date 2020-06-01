---
title: 会議の Requesttype
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: 会議の Requesttype 要素は、会議出席依頼の種類を表します。
ms.openlocfilehash: e90c44dd4124d698ca5ef7655f6429a7167673e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465787"
---
# <a name="meetingrequesttype"></a>会議の Requesttype

会議の**requesttype**要素は、会議出席依頼の種類を表します。 
  
```xml
<MeetingRequestType/>
```

 **会議の Requesttypetype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 次の表に、この要素に使用できるテキスト値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|FullUpdate  <br/> |既存の要求に対する完全な更新として会議出席依頼を識別します。 完全更新により、時間と情報のコンテンツが更新されました。  <br/> |
|InformationalUpdate  <br/> |更新された情報コンテンツのみが含まれている会議出席依頼を識別します。  <br/> |
|NewMeetingRequest  <br/> |会議出席依頼を新しい会議出席依頼として識別します。  <br/> |
|なし  <br/> |会議出席依頼の種類が定義されていないことを示します。  <br/> |
|最新  <br/> |会議出席依頼を古いものとして識別します。  <br/> |
|PrincipalWantsCopy  <br/> |会議出席依頼が代理人に会議メッセージを転送しており、そのコピーが情報としてマークされているプリンシパルに属していることを示します。  <br/> |
|孤立した更新  <br/> |既存の会議へのサイレント更新として会議出席依頼を識別します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

