---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: ErrorCode 要素は、ルールの述語またはアクションごとに失敗した検証を説明するルール検証エラー コードを表します。
ms.openlocfilehash: a582b09a579074a6728bb79b351b8c7a120c05de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517113"
---
# <a name="errorcode"></a>ErrorCode

**ErrorCode 要素は**、ルールの述語またはアクションごとに失敗した検証を説明するルール検証エラー コードを表します。 
  
```XML
<ErrorCode/>
```

 **RuleValidationErrorCodeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[エラー](error.md) <br/> |特定のルール プロパティ値、述語プロパティ値、またはアクション プロパティ値に対する 1 つの検証エラーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、次のいずれかの文字列に制限されます。
  
- ADOperationFailure
    
- ConnectedAccountNotFound
    
- CreateWithRuleId
    
- EmptyValueFound
    
- DuplicatedPriority
    
- DuplicatedOperationOnTheSameRule
    
- FolderDoesNotExist
    
- InvalidAddress
    
- InvalidDateRange
    
- InvalidFolderId
    
- InvalidSizeRange
    
- InvalidValue
    
- MessageClassificationNotFound
    
- MissingAction
    
- MissingParameter
    
- MissingRangeValue
    
- NotSettable
    
- RecipientDoesNotExist
    
- RuleNotFound
    
- SizeLessThanZero
    
- StringValueTooBig
    
- サポートされていないAddress
    
- UnexpectedError
    
- サポートされていないRule
    
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

