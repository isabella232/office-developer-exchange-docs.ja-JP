---
title: EWS アプリケーションの種類
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ca4e8b90-d0d8-4d55-aa92-19e21659d4f5
description: Exchange の EWS を使用して作成できる、最も一般的な種類のアプリケーションについて説明します。
ms.openlocfilehash: 1ce739f453ba1bc6f1b5d38edae3776daa562ffb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758885"
---
# <a name="ews-application-types"></a>EWS アプリケーションの種類

Exchange の EWS を使用して作成できる、最も一般的な種類のアプリケーションについて説明します。
  
[EWS および Exchange のアーキテクチャ](ews-applications-and-the-exchange-architecture.md)には、以下を含め、一貫した方法で最も一般的な種類のアプリケーションを作成するために使用できる一貫した開発モデルが用意されています。 
  
- [クライアント アプリケーション](#bk_clientapps)EWS を使用して、Exchange データにアクセスするためのスタンドアロン アプリケーションです。 Outlook と Outlook Web App は、クライアント アプリケーションの例を示します。 
    
- [ポータル アプリケーション](#bk_portalapps): 空き時間情報や連絡先情報などの情報を含めることによって、既存の web ページを拡張するアプリケーションが、Exchange から取得します。 Exchange データを取得する、SharePoint web パーツは、ポータル アプリケーションの例です。 
    
- [サービス アプリケーション](#bk_serviceapps)バック グラウンド ジョブの統合や既存のシステムに Exchange からのデータを同期するために使用します。 たとえば、CRM アプリケーションを Exchange からの連絡先情報を同期化するアプリケーションです。 
    
クライアント、ポータル、またはサービス アプリケーションの間でのアイテムの情報を取得するために使用される EWS のコードを変更するのに必要はありませんので交換 - から情報を取得するためにこれらのアプリケーション モデルの一般的なコード ベースを使用できます。 次の 1 つのアプリケーションからの変更点は、メールボックス アクセスと認証メカニズムです。 などのクライアント アプリケーション通常を使用して、ユーザーが直接アクセスし、基本認証または NTLM 認証では、サービス アプリケーションの可能性がありますメールボックスへのアクセスと OAuth の認証に偽装を使用するが。
  
## <a name="client-applications"></a>クライアント アプリケーション
<a name="bk_clientapps"> </a>

EWS クライアント アプリケーションは、EWS を使用して Exchange ストアから情報を取得するスタンドアロン アプリケーションです。EWS クライアント アプリケーションは、直接クライアント アクセスまたは代理人アクセスを使用して、メールボックス ストアからデータを取得します。EWS を使用するクライアント アプリケーションの例を次に示します。
  
- Outlook (メール ヒント、可用性、ユーザー不在時状態などの機能の中)
    
- デバイス用 OWA
    
- Outlook for Mac 2011
    
- Lync (空き時間情報用)
    
ユーザーが独自のログオン資格情報をユーザー自身のメールボックス内の情報へのアクセスに制限されるように、直接アクセスし、基本認証または NTLM 認証では、クライアント アプリケーション通常使用します。 クライアント アプリケーションもサポートされている別のユーザーのメールボックスにアクセスする権限が与えられているユーザーのアクセスを委任します。
  
## <a name="portal-applications"></a>ポータル アプリケーション
<a name="bk_portalapps"> </a>

ポータル アプリケーションは、既存の Web ページまたはポータルを拡張して、Exchange メールボックス情報をページの個人用コンポーネントとして含めます。SharePoint Web パーツは最も一般的なポータル アプリケーションであり、パーソナライズ エキスペリエンスをユーザーに提供します。そのために、よく表示される SharePoint ポータル ページだけでなく、未読メッセージや最新メッセージ、予定表イベントなど、Exchange メールボックス データのビューを提供します。EWS ポータル アプリケーションは、直接クライアント アクセス、代理人アクセス、または偽装を使用して、メールボックス ストアからデータを取得します。Exchange 2013 と SharePoint 2013 の両方が、サーバー相互認証のための OAuth 認証プロトコルをサポートしているので、OAuth は最もシームレスでセキュリティ保護された認証方法を提供します。
  
## <a name="service-applications"></a>サービス アプリケーション
<a name="bk_serviceapps"> </a>

サービス アプリケーションは通常、既存のアプリケーションに組み込まれるバックグラウンド ジョブであり、Exchange を拡張してシステムと Exchange ストアの間でデータを相互に関連付けます。一般に、サービス アプリケーションにはユーザー インターフェイスがありません。また、サービス アプリケーションは認証とアクセスに偽装または OAuth を使用します。EWS サービス アプリでは、ユーザーを偽装するサービス アカウントを作成することは一般的です。一組のユーザーを偽装する権限を単一のアカウントに付与でき、それらのアカウントに代わってメールボックス操作を実行できるからです。たとえば、EWS サービス アプリケーションは、サービス アカウントと偽装を使用して、CRM ソリューションのマーケティング リストと Exchange 配布グループの間でデータを同期させることができます。
  
## <a name="see-also"></a>関連項目


- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [EWS アプリケーションと Exchange のアーキテクチャ](ews-applications-and-the-exchange-architecture.md)
    
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)
    

