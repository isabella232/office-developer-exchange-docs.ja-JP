---
title: 表示名 (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisplayName
api_type:
- schema
ms.assetid: e7efbbe1-6629-4d11-bed1-ed899e3f9d77
description: DisplayName 要素では、フォルダー、連絡先、配布リスト、ユーザーの代理人、場所、またはルールの表示名を定義します。
ms.openlocfilehash: 53f4e083d9e6617206e383d4408e08ed7ea0fe08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760106"
---
# <a name="displayname-string"></a>表示名 (文字列)

**DisplayName**要素では、フォルダー、連絡先、配布リスト、ユーザーの代理人、場所、またはルールの表示名を定義します。 
  
```XML
<DisplayName/>
```

 **文字列型 (String)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |メールボックスの予定表フォルダーを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[メッセージ](contactsfolder.md) <br/> |メールボックスの連絡先フォルダーを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[ルール (RuleType)](rule-ruletype.md) <br/> |ユーザーのメールボックス内のルールを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
|[ユーザー Id](userid.md) <br/> |代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

表示名を表すテキスト値は、この要素を使用する場合に必要です。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

[TestFolder] フォルダーの表示名を設定すると、新しいフォルダーを作成する方法を次の例に示します。
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

