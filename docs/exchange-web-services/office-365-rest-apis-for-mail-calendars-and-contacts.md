---
title: メール、カレンダー、連絡先用の Microsoft Graph の Outlook API
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3b2e71a6-5fa5-4008-b243-d3a6e9173b3d
description: Office 365 または Exchange Online において、メール、予定表、連絡先へのアクセスに使用できる Microsoft Graph API の詳細です。
ms.openlocfilehash: 3065de389157345afd5ed07e302ace99e2048bdf
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353295"
---
# <a name="microsoft-graph-rest-apis-for-mail-calendars-and-contacts"></a><span data-ttu-id="dab83-103">メール、予定表、連絡先用の Microsoft Graph の REST API</span><span class="sxs-lookup"><span data-stu-id="dab83-103">Office 365 REST APIs for mail, calendars, and contacts</span></span>

<span data-ttu-id="dab83-104">Office 365 または Exchange Online において、メール、予定表、連絡先へのアクセスに使用できる Microsoft Graph API の詳細です。</span><span class="sxs-lookup"><span data-stu-id="dab83-104">Find information about the Office 365 APIs that you can use to access mail, calendars, and contacts in Office 365 or Exchange Online.</span></span>

<span data-ttu-id="dab83-105">Office 365 および Exchange Online は、電子メール、予定表、および連絡先で作業する新しい方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="dab83-105">Office 365 and Exchange Online provide a new way to work with email, calendars, and contacts.</span></span> <span data-ttu-id="dab83-106">Microsoft Graph のメール、予定表、連絡先用の REST API は、Exchange データにアクセスして操作する強力で簡単な方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="dab83-106">The Mail, Calendar, and Contact REST APIs provide a powerful, easy-to-use way to access and manipulate Exchange data.</span></span> <span data-ttu-id="dab83-107">これらの API は、認証用の OAuth バージョン 2.0、データ抽象化用の OData バージョン 4.0 および JSON など、オープンな標準に基づいています。</span><span class="sxs-lookup"><span data-stu-id="dab83-107">These APIs are based on open standards: OAuth version 2.0 for authentication, and OData version 4.0 and JSON for data abstraction.</span></span> <span data-ttu-id="dab83-108">これには以下の利点があります。</span><span class="sxs-lookup"><span data-stu-id="dab83-108">This provides the following advantages:</span></span>

- <span data-ttu-id="dab83-109">これらの API は認証に OAuth を求めるため、アプリケーションがユーザーの資格情報を処理または格納する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="dab83-109">Because these APIs require OAuth for authentication, your application does not have to handle or store user credentials.</span></span>

- <span data-ttu-id="dab83-p102">OAuth は、ユーザー データへの厳格に範囲指定されたアクセス許可を要求できるようにします。たとえば、アクセス許可を要求して、ユーザーの予定表のみを読み取るようにアプリケーションを設計する場合があります。</span><span class="sxs-lookup"><span data-stu-id="dab83-p102">OAuth makes it possible to request tightly scoped permissions to user data. For example, you might design your application to request permission and read only a user's calendar.</span></span>

## <a name="work-with-email-and-mail-folders"></a><span data-ttu-id="dab83-112">電子メールおよびメール フォルダーで作業する</span><span class="sxs-lookup"><span data-stu-id="dab83-112">Work with email and mail folders</span></span>

<span data-ttu-id="dab83-p103">[メール API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) を使用して、電子メールの取得、作成、更新、削除、移動、コピー、および送信を行うことができます。また、メール フォルダーの取得、作成、更新、および削除を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="dab83-p103">You can use the [Mail API](https://developer.microsoft.com/graph/docs/concepts/outlook-mail-concept-overview) to get, create, update, delete, move, copy, and send email. You can also get, create, update, and delete mail folders.</span></span> 
  
## <a name="work-with-events-calendars-and-calendar-groups"></a><span data-ttu-id="dab83-115">イベント、予定表、および予定表グループで作業する</span><span class="sxs-lookup"><span data-stu-id="dab83-115">Work with events, calendars, and calendar groups</span></span>

<span data-ttu-id="dab83-p104">[予定表 API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) を使用して、イベントの取得、作成、更新、および削除を行うことができます。また、予定表グループおよび予定表の取得、作成、更新、および削除を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="dab83-p104">You can use the [Calendar API](https://developer.microsoft.com/graph/docs/concepts/outlook-calendar-concept-overview) to get, create, update, and delete events. You can also get, create, update, and delete calendar groups and calendars.</span></span> 
  
## <a name="work-with-contacts-and-contact-folders"></a><span data-ttu-id="dab83-118">連絡先および連絡先フォルダーで作業する</span><span class="sxs-lookup"><span data-stu-id="dab83-118">Work with contacts and contact folders</span></span>

<span data-ttu-id="dab83-p105">[連絡先 API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) を使用して、ユーザーのメールボックス内の連絡先の取得、作成、更新、および削除を行うことができます。また、連絡先フォルダーの取得を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="dab83-p105">You can use the [Contacts API](https://developer.microsoft.com/graph/docs/concepts/outlook-contacts-concept-overview) to get, create, update, and delete contacts in a user's mailbox. You can also get contact folders.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="dab83-121">次のステップ</span><span class="sxs-lookup"><span data-stu-id="dab83-121">Next steps</span></span>

<span data-ttu-id="dab83-122">[「Microsoft Graph ドキュメント」](https://developer.microsoft.com/graph/docs/concepts/overview)のページにマウス ポインターを合わせて、環境設定および API 使用開始にあたってのガイダンスを含む、メール、予定表、連絡先の API のより詳細な情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="dab83-122">Head over to the [Developing on the Office 365 platform](https://developer.microsoft.com/graph/docs/concepts/overview) page to get more information about the Mail, Calendar, and Contacts APIs, including guidance for setting up your environment and getting started with the APIs.</span></span> 

<span data-ttu-id="dab83-123">また、[「Microsoft Graph のクイック スタート」](https://developer.microsoft.com/graph/quick-start)と[コード サンプル](https://developer.microsoft.com/office/gallery/?filterBy=Samples,Microsoft%20Graph)を必ず確認し、これらの API の動作をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dab83-123">Also be sure to check out the starter projects and code samples to see these APIs in action.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="dab83-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="dab83-124">See also</span></span>

- [<span data-ttu-id="dab83-125">Microsoft Graph のドキュメント</span><span class="sxs-lookup"><span data-stu-id="dab83-125">Microsoft Graph documentation</span></span>](https://developer.microsoft.com/graph/docs/concepts/overview)   

