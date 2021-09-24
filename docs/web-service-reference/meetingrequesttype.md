---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: MeetingRequestType 要素は、会議出席依頼の種類を記述します。
ms.openlocfilehash: 1a8371331691bb9dee5595b0130ec0c3c75c47c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539375"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

**MeetingRequestType** 要素は、会議出席依頼の種類を記述します。 
  
```xml
<MeetingRequestType/>
```

 **MeetingRequestTypeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 次の表に、この要素で使用できるテキスト値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|FullUpdate  <br/> |会議出席依頼を既存の要求の完全な更新として識別します。 完全な更新では、時間と情報コンテンツが更新されました。  <br/> |
|InformationalUpdate  <br/> |更新された情報コンテンツのみを含む会議出席依頼を識別します。  <br/> |
|NewMeetingRequest  <br/> |会議出席依頼を新しい会議出席依頼として識別します。  <br/> |
|なし  <br/> |会議出席依頼の種類が定義されていないかどうかを示します。  <br/> |
|古い  <br/> |会議出席依頼を古いとして識別します。  <br/> |
|PrincipalWantsCopy  <br/> |会議出席依頼が、会議メッセージを代理人に転送し、そのコピーが情報としてマークされているプリンシパルに属する場合を示します。  <br/> |
|SilentUpdate  <br/> |会議出席依頼を既存の会議に対するサイレント更新として識別します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

