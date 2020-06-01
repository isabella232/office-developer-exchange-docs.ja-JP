---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: AppStatus 要素の値は、メールアプリの状態を示します。
ms.openlocfilehash: d833947fd62d500418f257829d241a2e0b3bca9c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464778"
---
# <a name="appstatus"></a>AppStatus

**Appstatus**要素の値は、メールアプリの状態を示します。 
  
```XML
<AppStatus/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[メタデータ](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>テキスト値

**Appstatus**要素のテキスト値は、メールアプリの状態を示します。 ユーザーがメールアプリの状態に関連する問題を修正できる場合、 [actionurl](actionurl.md)要素は修正を実行するための url を提供します。 
  
**表1AppStatus の値**

|**値**|**説明**|
|:-----|:-----|
|Null または0  <br/> |メールアプリの状態は正常です。  <br/> |
|1.0  <br/> |メールアプリを自動的に更新できませんでした。 メールアプリを Office ストアから再インストールする必要があります。  <br/> |
|1.1  <br/> |メールアプリを自動的に更新できませんでした。 メールアプリには、強化されたアクセス許可が必要です。そのためには、確認とインストールの確認が必要です。  <br/> |
|1.2  <br/> |メールアプリを自動的に更新できませんでした。 現在のライセンスの有効期限が切れているか、無効です。 Office ストアからメールアプリを更新してください。  <br/> |
|2.0  <br/> |メールアプリのライセンスを自動的に更新できませんでした。 メールアプリのライセンスは、Office ストアから回復する必要があります。  <br/> |
|2.1  <br/> |メールアプリのライセンスを自動的に更新できませんでした。 現在のライセンスの有効期限が切れています。 このアプリの新しいライセンスを Office ストアからインストールする必要があります。  <br/> |
|3.0  <br/> |メールアプリの Office ストアの状態が変更されました。 これは、メールアプリに問題があることを示している可能性があります。 詳細については、「Office ストアのメールアプリ」ページにアクセスしてください。  <br/> |
|3.1  <br/> |メールアプリが Office ストアから削除されました。  <br/> |
|3.2  <br/> |メールアプリで問題が検出され、一時的に Office ストアから引き出されています。  <br/> |
|3.3  <br/> |メールアプリは、30日以内に Office ストアから削除されます。  <br/> |
|4.0  <br/> |メールアプリは、メールクライアントによって自動的に無効にされています。  <br/> |
|4.1  <br/> |パフォーマンス上の理由から、メールアプリは Outlook によって無効にされています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [メタデータ](metadata-ex15websvcsotherref.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

