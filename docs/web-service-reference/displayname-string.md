---
title: DisplayName (string)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DisplayName
api_type:
- schema
ms.assetid: e7efbbe1-6629-4d11-bed1-ed899e3f9d77
description: DisplayName 要素は、フォルダー、連絡先、配布リスト、委任ユーザー、場所、またはルールの表示名を定義します。
ms.openlocfilehash: 3fc0faca0425bc6de3f71c154926991d922c8a79
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520864"
---
# <a name="displayname-string"></a>DisplayName (string)

**DisplayName 要素は**、フォルダー、連絡先、配布リスト、委任ユーザー、場所、またはルールの表示名を定義します。 
  
```XML
<DisplayName/>
```

 **String**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |メールボックス内の予定表フォルダーを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[Rule (RuleType)](rule-ruletype.md) <br/> |ユーザーのメールボックス内のルールを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
|[UserId](userid.md) <br/> |代理人ユーザーまたはフォルダー アクセス許可を持つユーザーを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

この要素を使用する場合は、表示名を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の使用例は、新しいフォルダーを作成し、フォルダーの DisplayName を "TestFolder" に設定する方法を示しています。
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

