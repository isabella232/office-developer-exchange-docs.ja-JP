---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: ErrorCode 要素は、各ルール述語またはアクションの検証に失敗したことを示すルールの検証エラーコードを表します。
ms.openlocfilehash: 6432aeee786d74a9afcb346cb66765f9001257de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460079"
---
# <a name="errorcode"></a>ErrorCode

**ErrorCode**要素は、各ルール述語またはアクションの検証に失敗したことを示すルールの検証エラーコードを表します。 
  
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
|[Error](error.md) <br/> |特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素のテキスト値は、次の文字列のいずれかに制限されています。
  
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
    
- 誤 Singrangevalue
    
- NotSettable 可能
    
- RecipientDoesNotExist
    
- RuleNotFound
    
- Sizeless0
    
- StringValueTooBig
    
- アン Supportedaddress
    
- UnexpectedError
    
- アン Supportedrule
    
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

