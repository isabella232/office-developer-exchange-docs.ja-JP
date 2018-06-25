---
title: Exchange における EWS での同期に関連するエラーの処理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a0807b90-645a-4ea6-aee1-96828df14be0
description: Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの同期に関連するエラーを処理する方法を説明します。
ms.openlocfilehash: 6de27d585e467d900941f34b2210877d17205502
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758894"
---
# <a name="handling-synchronization-related-errors-in-ews-in-exchange"></a>Exchange における EWS での同期に関連するエラーの処理

Exchange の EWS マネージ API または EWS を使用して開発したアプリケーションの同期に関連するエラーを処理する方法を説明します。
  
場合は、アプリケーションでは、アイテムとフォルダーを同期、同期に関連するエラーを処理する必要があります。 または、EWS アプリケーションを開発するとき、実行時にこれらのエラーを処理することができます。 これらのエラーのほとんどは、EWS マネージ api では、 [ResponseCodeType](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx)列挙体および[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx)の要素では、Exchange Web サービス (EWS) によって定義されます。 
  
**表 1 です。同期に関連するエラーと、それらを処理する方法**

|**Error**|**しようとするときに発生しています.**|**処理方法**|
|:-----|:-----|:-----|
|ErrorInvalidSyncStateData   <br/> | 無効な同期状態の値を使用してアイテムまたはフォルダーを同期するとき。  <br/>  後続の要求にルート フォルダーが含まれている場合に、最初の SyncFolderHierarchy 要求でルート フォルダーを除外したとき。  <br/>  後続の要求で別のルート フォルダーを使用したとき。  <br/> | 送信している同期状態の値が、以前の同期の際に戻された同期状態の値と一致していることを確認します。  <br/>  アイテムを同期するときにフォルダー階層の同期状態を送信していないことを確認します (その逆に、フォルダー階層を同期する場合にアイテムの同期状態を送信していないことも確認します)。   <br/>  適切なルート フォルダーの同期状態を送信していることを確認します。  <br/>  各要求で同じルート フォルダーが指定されていることを確認します。  <br/>  以前の要求で null のルート フォルダーが指定されていないこと、現在の要求にルートのルート フォルダーが含まれていることを確認します。null とルートは同じものとして扱われません。  <br/> |
|ErrorSyncFolderNotFound  <br/> |サーバ―上にないフォルダーのサブフォルダーまたはアイテムを同期するとき。  <br/> |要求で指定したフォルダー ID が、以前の同期応答でサーバーから返されたフォルダー ID と一致することを確認します。  <br/> |
|ErrorTimeoutExpired  <br/> |送信した要求数が多すぎるとき。  <br/> |10 個のアイテムを 1 つの[制限](ews-throttling-in-exchange.md)が表示されないようにするのにはバッチにバッチを制限します。  <br/> |
|[ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx) <br/> |サーバーがオフラインまたは接続に問題がある場合に、EWS に接続するとき。   <br/> |サーバーとの接続をチェックし、要求を後ほど再試行します。これは、一時的なサービス エラーまたはネットワーク エラーの可能性があります。  <br/> |
   
## <a name="see-also"></a>関連項目


- [Exchange のメールボックス同期と EWS](mailbox-synchronization-and-ews-in-exchange.md)
    
- [Exchange EWS を使用してフォルダーを同期します。](how-to-synchronize-folders-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して項目を同期します。](how-to-synchronize-items-by-using-ews-in-exchange.md)
    
- [ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)
    

