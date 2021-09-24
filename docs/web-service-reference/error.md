---
title: Error
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: Error 要素は、特定のルール プロパティ値、述語プロパティ値、またはアクション プロパティ値に対する 1 つの検証エラーを表します。
ms.openlocfilehash: aeeda25ccc3e657e99bd6f2fea12322fdd3e720d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530862"
---
# <a name="error"></a>Error

**Error 要素は**、特定のルール プロパティ値、述語プロパティ値、またはアクション プロパティ値に対する 1 つの検証エラーを表します。 
  
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
|[FieldUri (Rule)](fielduri-rule.md) <br/> |検証エラーの原因となるルール フィールドの URI を指定します。  <br/> |
|[ErrorCode](errorcode.md) <br/> |ルールの述語またはアクションごとに失敗した検証を説明するルール検証エラー コードを表します。  <br/> |
|[ErrorMessage](errormessage.md) <br/> |検証エラーの理由を表します。  <br/> |
|[FieldValue](fieldvalue.md) <br/> |検証エラーの原因となるフィールドの値を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ValidationErrors](validationerrors.md) <br/> |エラーが発生した各ルール フィールドのルール検証エラーの配列を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

