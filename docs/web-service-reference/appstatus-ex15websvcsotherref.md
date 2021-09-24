---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: AppStatus 要素の値は、メール アプリの状態を示します。
ms.openlocfilehash: 69f481b197db513761b97d4fbba38452bbb4a9a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525317"
---
# <a name="appstatus"></a>AppStatus

**AppStatus 要素** の値は、メール アプリの状態を示します。 
  
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

**AppStatus** 要素のテキスト値は、メール アプリの状態を示します。 ユーザーがメール アプリの状態に関連する問題を修正できる場合 [、ActionUrl](actionurl.md) 要素は修正を実行するための URL を提供します。 
  
**表 1.AppStatus の値**

|**値**|**説明**|
|:-----|:-----|
|Null または 0  <br/> |メール アプリの状態は正常です。  <br/> |
|1.0  <br/> |メール アプリを自動的に更新する方法が設定されていない。 メール アプリは、メール ストアから再インストールOfficeがあります。  <br/> |
|1.1  <br/> |メール アプリを自動的に更新する方法が設定されていない。 メール アプリにはアクセス許可の増加が必要であり、インストールするには確認と確認が必要です。  <br/> |
|1.2  <br/> |メール アプリを自動的に更新できなかった。 現在のライセンスの有効期限が切れているか、無効です。 メール アプリは、メール ストアからOfficeしてください。  <br/> |
|2.0  <br/> |メール アプリ のライセンスを自動的に更新する必要があります。 メール アプリのライセンスは、メール ストアから回復するOfficeがあります。  <br/> |
|2.1  <br/> |メール アプリ のライセンスを自動的に更新する必要があります。 現在のライセンスの有効期限が切れています。 このアプリの新しいライセンスは、アプリストアからインストールするOfficeがあります。  <br/> |
|3.0  <br/> |メール Officeストアの状態が変更されました。 これは、メール アプリに問題がある可能性があります。 詳細については、[メール アプリ] ページの [Officeストア] に移動します。  <br/> |
|3.1  <br/> |メール アプリは、メール ストアからOfficeされました。  <br/> |
|3.2  <br/> |メール アプリで問題が検出され、一時的にメール ストアからOfficeされました。  <br/> |
|3.3  <br/> |メール アプリは、30 日以内に Officeストアから削除されます。  <br/> |
|4.0  <br/> |メール アプリはメール クライアントによって自動的に無効になっています。  <br/> |
|4.1  <br/> |パフォーマンス上の理由から、メール アプリOutlook無効になっています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |該当なし  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [メタデータ](metadata-ex15websvcsotherref.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

