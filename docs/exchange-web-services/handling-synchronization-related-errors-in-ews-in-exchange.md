---
title: Exchange における EWS での同期に関連するエラーの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの同期に関連するエラーを処理する方法を説明します。
ms.openlocfilehash: f62937ec444d64b0b358581371f1260f565215b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455941"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Exchange における EWS での同期に関連するエラーの処理

Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの同期に関連するエラーを処理する方法を説明します。
  
アプリケーションがアイテムとフォルダーを同期する場合は、同期に関連するエラーを処理する必要があります。 これらのエラーは実行時、または EWS アプリケーションを開発するときに処理することができます。 これらのエラーのほとんどは、EWS マネージ API では [ResponseCodeType](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) 列挙体で、Exchange Web サービス (EWS) では [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) 要素で定義されています。 
  
**表 1. 同期に関連するエラーとその処理方法**

|**エラー**|**発生するタイミング**|**処理方法**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData  <br/> | 無効な同期状態の値を使用してアイテムまたはフォルダーを同期するとき。  <br/>  後続の要求にルート フォルダーが含まれている場合に、最初の SyncFolderHierarchy 要求でルート フォルダーを除外したとき。  <br/>  後続の要求で別のルート フォルダーを使用したとき。  <br/> | 送信している同期状態の値が、以前の同期の際に戻された同期状態の値と一致していることを確認します。  <br/>  アイテムを同期するときにフォルダー階層の同期状態を送信していないことを確認します (その逆に、フォルダー階層を同期する場合にアイテムの同期状態を送信していないことも確認します)。  <br/>  適切なルート フォルダーの同期状態を送信していることを確認します。  <br/>  各要求で同じルート フォルダーが指定されていることを確認します。  <br/>  以前の要求で null のルート フォルダーが指定されていないこと、現在の要求にルートのルート フォルダーが含まれていることを確認します。null とルートは同じものとして扱われません。  <br/> |
|ErrorSyncFolderNotFound  <br/> |サーバ―上にないフォルダーのサブフォルダーまたはアイテムを同期するとき。  <br/> |要求で指定したフォルダー ID が、以前の同期応答でサーバーから返されたフォルダー ID と一致することを確認します。  <br/> |
|ErrorTimeoutExpired  <br/> |送信した要求数が多すぎるとき。  <br/> |[調整される](ews-throttling-in-exchange.md)ことを避けるため、バッチ処理あたりのアイテム数を 10 に制限します。  <br/> |
|[ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |サーバーがオフラインまたは接続に問題がある場合に、EWS に接続するとき。  <br/> |サーバーとの接続を確認し、要求を後で再試行します。これは、一時的なサービス エラーまたはネットワーク エラーである可能性があります。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Exchange で EWS を使用してフォルダーを同期させる](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用してアイテムを同期する](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

