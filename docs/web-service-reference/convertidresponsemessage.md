---
title: ConvertIdResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponseMessage
api_type:
- schema
ms.assetid: 7a439cae-0268-4328-9ded-af56ad642227
description: ConvertIdResponseMessage 要素には、収束 Tid 操作要求の状態と結果が含まれています。
ms.openlocfilehash: cd0154f87390be3516ced4be53f5371d4a348c49
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456221"
---
# <a name="convertidresponsemessage"></a>ConvertIdResponseMessage

**ConvertIdResponseMessage**要素には、[収束 tid 操作](convertid-operation.md)要求の状態と結果が含まれています。 
  
- [ConvertIdResponse](convertidresponse.md) 
- [ResponseMessages](responsemessages.md)
- [ConvertIdResponseMessage](convertidresponsemessage.md)
  
```xml
<ConvertIdResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <AlternateId/>
</ConvertIdResponseMessage>
```

 **ConvertIdResponseMessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**ResponseClass** <br/> | [[コンバーター tid 操作](convertid-operation.md)の応答の状態について説明します。<br/><br/>この属性には、次の値が有効です。<br/><br/>-成功  <br/>-Warning  <br/>-エラー  <br/> |
   
#### <a name="responseclass-attribute-values"></a>ResponseClass 属性の値

|**値**|**説明**|
|:-----|:-----|
|**Success** <br/> |満たされる要求を記述します。  <br/> |
|**Warning** <br/> | 完全には処理されなかった、または予期しない結果が発生した要求を記述します。  <br/> |
|**Error** <br/> | 満たされない要求を記述します。<br/><br/>エラーのソースの例を次に示します。  <br/><br/>-無効な属性または要素  <br/>-範囲外の属性または要素  <br/>-不明なタグ  <br/>-コンテキスト内で有効ではない属性または要素  <br/>-クライアントによる権限のないアクセス試行  <br/>-有効なクライアント側の呼び出しに応答した場合のサーバー側障害<br/><br/>エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MessageText](messagetext.md) <br/> |応答の状態を説明するテキストを提供します。  <br/> |
|[ResponseCode](responsecode.md) <br/> |要求で発生した特定のエラーを識別するエラーコードを提供します。  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |現在未使用で、今後の使用のために予約されています。 この要素には0の値が含まれています。  <br/> |
|[MessageXml](messagexml.md) <br/> |エラー応答に関する追加情報を提供します。  <br/> |
|[AlternateId](alternateid.md) <br/> |応答で変換された id を記述します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージを含みます。  <br/> |
   
## <a name="remarks"></a>注釈

変換された識別子ごとに1つの応答メッセージが返されます。 エラー応答コードが返された場合、 [Alternateid](alternateid.md)要素は応答から失われます。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [ConvertId 操作](convertid-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

