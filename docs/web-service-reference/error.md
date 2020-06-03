---
title: Error
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: Error 要素は、特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。
ms.openlocfilehash: 9c28f63aa79446d89152868c81c85ffa7b3a8b39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460681"
---
# <a name="error"></a>Error

**Error**要素は、特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 **RuleValidationErrorType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FieldUri (ルール)](fielduri-rule.md) <br/> |検証エラーの原因となったルールフィールドへの URI を指定します。  <br/> |
|[ErrorCode](errorcode.md) <br/> |ルールの述語またはアクションごとに、検証に失敗したことを示すルールの検証エラーコードを表します。  <br/> |
|[ErrorMessage](errormessage.md) <br/> |検証エラーの理由を表します。  <br/> |
|[FieldValue](fieldvalue.md) <br/> |検証エラーの原因となったフィールドの値を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

