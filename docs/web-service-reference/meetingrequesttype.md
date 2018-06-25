---
title: MeetingRequestType
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
description: MeetingRequestType 要素は、会議出席依頼の種類について説明します。
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832432"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

**MeetingRequestType**要素は、会議出席依頼の種類について説明します。 
  
```xml
<MeetingRequestType/>
```

 **MeetingRequestTypeType**
## <a name="attributes-and-elements"></a>属性および要素

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

テキスト値は必須です。 次の表は、この要素の使用可能なテキスト値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|FullUpdate  <br/> |会議出席依頼が既存の要求に完全な更新であることを識別します。 フル更新には、時間と情報が更新されました。  <br/> |
|InformationalUpdate  <br/> |情報コンテンツの更新のみを含む会議出席依頼を識別します。  <br/> |
|NewMeetingRequest  <br/> |新しい会議出席依頼と会議出席依頼を識別します。  <br/> |
|なし  <br/> |会議出席依頼の種類にすることを示しますが定義されていません。  <br/> |
|古い  <br/> |として古い会議出席依頼を識別します。  <br/> |
|PrincipalWantsCopy  <br/> |会議出席依頼が代理人に会議のメッセージを転送するには情報とマークされている彼のコピーのあるプリンシパルに属していることを示します。  <br/> |
|SilentUpdate  <br/> |会議出席依頼を既存の会議に更新プログラムがサイレントとして識別します。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

