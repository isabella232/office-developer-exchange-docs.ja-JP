---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: AppStatus 要素の値は、メール アプリケーションのステータスを示します。
ms.openlocfilehash: cf213fc3d7be02c411e9c2e83a4ff153dbefe098
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759427"
---
# <a name="appstatus"></a>AppStatus

**AppStatus**要素の値は、メール アプリケーションのステータスを示します。 
  
```XML
<AppStatus/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[メタデータ](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>テキスト値

**AppStatus**要素のテキスト値は、メール アプリケーションのステータスを示します。 ユーザーは、メール アプリケーションの状態に関連する問題を修正することができます、 [ActionUrl](actionurl.md)要素は、この修正プログラムを実行する URL を提供します。 
  
**表 1 です。AppStatus 値**

|**値**|**説明**|
|:-----|:-----|
|Null または 0  <br/> |メール アプリケーションでは、正常な状態があります。  <br/> |
|1.0  <br/> |メール アプリケーションが自動的に更新できませんでした。 メール アプリケーションでは、Office ストアから再インストールする必要があります。  <br/> |
|1.1  <br/> |メール アプリケーションが自動的に更新できませんでした。 メール アプリケーションは、拡張されたアクセス許可を必要とし、確認とインストールを確認する必要があります。  <br/> |
|1.2  <br/> |メール アプリケーションを自動的に更新することができませんでした。 現在のライセンスは期限が切れているか、無効です。 Office ストアからのメール アプリケーションを更新してください。  <br/> |
|2.0  <br/> |メール アプリケーションのライセンスを自動的に更新できませんでした。 メール アプリケーションのライセンスは、Office ストアから回復する必要があります。  <br/> |
|2.1  <br/> |メール アプリケーションのライセンスを自動的に更新できませんでした。 現在のライセンスの有効期限が切れています。 このアプリケーション用の新しいライセンスは、Office ストアからインストールする必要があります。  <br/> |
|3.0  <br/> |メール アプリケーションの Office のストアの状態が変更されました。 メール アプリケーションに関連した問題がある可能性があります。 詳細については Office ストアにメール アプリケーションのページに移動します。  <br/> |
|3.1  <br/> |メール アプリが Office ストアから削除されました。  <br/> |
|3.2  <br/> |メール アプリケーションで問題が検出され、が一時的に Office ストアから引き出されています。  <br/> |
|3.3  <br/> |30 日以内、メール アプリを Office ストアから削除されます。  <br/> |
|4.0  <br/> |メール アプリケーションは、メール クライアントによって自動的に無効にされています。  <br/> |
|4.1  <br/> |パフォーマンス上の理由から、Outlook によってメール アプリケーションを無効にされています。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |該当しない  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [メタデータ](metadata-ex15websvcsotherref.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

