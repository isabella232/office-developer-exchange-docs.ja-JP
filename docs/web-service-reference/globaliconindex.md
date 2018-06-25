---
title: GlobalIconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d28ed70-4cfe-46e4-8d15-593c6e355bcf
description: GlobalIconIndex 要素は、会話のすべての項目のグローバル アイコン インデックスを識別します。
ms.openlocfilehash: e8d78bfcfc0e57df9230db86e080d1ee29878094
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831727"
---
# <a name="globaliconindex"></a><span data-ttu-id="641be-103">GlobalIconIndex</span><span class="sxs-lookup"><span data-stu-id="641be-103">GlobalIconIndex</span></span>

<span data-ttu-id="641be-104">**GlobalIconIndex**要素は、会話のすべての項目のグローバル アイコン インデックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="641be-104">The **GlobalIconIndex** element identifies the global icon index for all items in a conversation.</span></span> 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MaillrmForwarded | MaillrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 <span data-ttu-id="641be-105">**IconIndexType**</span><span class="sxs-lookup"><span data-stu-id="641be-105">**IconIndexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="641be-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="641be-106">Attributes and elements</span></span>

<span data-ttu-id="641be-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="641be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="641be-108">属性</span><span class="sxs-lookup"><span data-stu-id="641be-108">Attributes</span></span>

<span data-ttu-id="641be-109">なし。</span><span class="sxs-lookup"><span data-stu-id="641be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="641be-110">子要素</span><span class="sxs-lookup"><span data-stu-id="641be-110">Child elements</span></span>

<span data-ttu-id="641be-111">なし。</span><span class="sxs-lookup"><span data-stu-id="641be-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="641be-112">親要素</span><span class="sxs-lookup"><span data-stu-id="641be-112">Parent elements</span></span>

<span data-ttu-id="641be-113">[会話 (ConversationType)](conversation-conversationtype.md) | [アイテム](item.md) | [連絡先](contact.md) | [DistributionList](distributionlist.md) | [メッセージ](message-ex15websvcsotherref.md) | [カレンダー項目](calendaritem.md) | [PostItem](postitem.md) | [タスク](task.md)</span><span class="sxs-lookup"><span data-stu-id="641be-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="641be-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="641be-114">Text value</span></span>

<span data-ttu-id="641be-115">次の表には、 **GlobalIconIndex**要素の使用可能なテキスト値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="641be-115">The following table contains the possible text values for the **GlobalIconIndex** element.</span></span> 
  
|<span data-ttu-id="641be-116">**値**</span><span class="sxs-lookup"><span data-stu-id="641be-116">**Value**</span></span>|<span data-ttu-id="641be-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="641be-117">**Description**</span></span>|
|:-----|:-----|
|||
|<span data-ttu-id="641be-118">Default</span><span class="sxs-lookup"><span data-stu-id="641be-118">Default</span></span>  <br/> |<span data-ttu-id="641be-119">既定のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-119">Specifies the default icon.</span></span>  <br/> |
|<span data-ttu-id="641be-120">PostItem</span><span class="sxs-lookup"><span data-stu-id="641be-120">PostItem</span></span>  <br/> |<span data-ttu-id="641be-121">投稿アイテムのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-121">Specifies the icon for a post item.</span></span>  <br/> |
|<span data-ttu-id="641be-122">MailRead</span><span class="sxs-lookup"><span data-stu-id="641be-122">MailRead</span></span>  <br/> |<span data-ttu-id="641be-123">開封済みのメールを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-123">Specifies the mail read icon.</span></span>  <br/> |
|<span data-ttu-id="641be-124">MailUnread</span><span class="sxs-lookup"><span data-stu-id="641be-124">MailUnread</span></span>  <br/> |<span data-ttu-id="641be-125">未読のメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-125">Specifies the unread mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-126">MailReplied</span><span class="sxs-lookup"><span data-stu-id="641be-126">MailReplied</span></span>  <br/> |<span data-ttu-id="641be-127">[メール] アイコンに、返信を指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-127">Specifies the replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-128">MailForwarded</span><span class="sxs-lookup"><span data-stu-id="641be-128">MailForwarded</span></span>  <br/> |<span data-ttu-id="641be-129">転送されたメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-129">Specifies the forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-130">MailEncrypted</span><span class="sxs-lookup"><span data-stu-id="641be-130">MailEncrypted</span></span>  <br/> |<span data-ttu-id="641be-131">暗号化されたメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-131">Specifies the encrypted mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-132">MailSmimeSigned</span><span class="sxs-lookup"><span data-stu-id="641be-132">MailSmimeSigned</span></span>  <br/> |<span data-ttu-id="641be-133">/Multipurpose をセキュリティで保護されたインターネット メール拡張 (S/MIME) 署名されたメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-133">Specifies the Secure/Multipurpose Internet Mail Extensions (S/MIME) signed mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-134">MailEncryptedReplied</span><span class="sxs-lookup"><span data-stu-id="641be-134">MailEncryptedReplied</span></span>  <br/> |<span data-ttu-id="641be-135">[メール] アイコンを暗号化された応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-135">Specifies the encrypted replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-136">MailSmimeSignedReplied</span><span class="sxs-lookup"><span data-stu-id="641be-136">MailSmimeSignedReplied</span></span>  <br/> |<span data-ttu-id="641be-137">秒/MIME 署名返信メールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-137">Specifies the S/MIME signed replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-138">MailEncryptedForwarded</span><span class="sxs-lookup"><span data-stu-id="641be-138">MailEncryptedForwarded</span></span>  <br/> |<span data-ttu-id="641be-139">暗号化された転送されたメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-139">Specifies the encrypted forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-140">MailSmimeSignedForwarded</span><span class="sxs-lookup"><span data-stu-id="641be-140">MailSmimeSignedForwarded</span></span>  <br/> |<span data-ttu-id="641be-141">S/MIME 署名されたメール] アイコンを転送するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-141">Specifies the S/MIME signed forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-142">MailEncryptedRead</span><span class="sxs-lookup"><span data-stu-id="641be-142">MailEncryptedRead</span></span>  <br/> |<span data-ttu-id="641be-143">暗号化された読み取りメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-143">Specifies the encrypted read mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-144">MailSmimeSignedRead</span><span class="sxs-lookup"><span data-stu-id="641be-144">MailSmimeSignedRead</span></span>  <br/> |<span data-ttu-id="641be-145">メール開封済みの S/MIME 署名を指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-145">Specifies the S/MIME signed read mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-146">MailIrm</span><span class="sxs-lookup"><span data-stu-id="641be-146">MailIrm</span></span>  <br/> |<span data-ttu-id="641be-147">情報権利管理の IRM で保護されたメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-147">Specifies the Information Rights Management (IRM)-protected mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-148">MailIrmForwarded</span><span class="sxs-lookup"><span data-stu-id="641be-148">MailIrmForwarded</span></span>  <br/> |<span data-ttu-id="641be-149">[メール] アイコンを転送された IRM で保護されたを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-149">Specifies the IRM-protected forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-150">MailIrmReplied</span><span class="sxs-lookup"><span data-stu-id="641be-150">MailIrmReplied</span></span>  <br/> |<span data-ttu-id="641be-151">返信 IRM で保護されたメール] アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-151">Specifies the IRM-protected replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-152">SmsSubmitted</span><span class="sxs-lookup"><span data-stu-id="641be-152">SmsSubmitted</span></span>  <br/> |<span data-ttu-id="641be-153">ショート メッセージ サービス (SMS) のルーティングのために送信するメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-153">Specifies the icon for mail submitted for Short Message Service (SMS) routing.</span></span>  <br/> |
|<span data-ttu-id="641be-154">SmsRoutedToDeliveryPoint</span><span class="sxs-lookup"><span data-stu-id="641be-154">SmsRoutedToDeliveryPoint</span></span>  <br/> |<span data-ttu-id="641be-155">SMS が外部の配信ポイントにルーティングするためのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-155">Specifies the icon for SMS routing to an external delivery point.</span></span>  <br/> |
|<span data-ttu-id="641be-156">SmsRoutedToExternalMessagingSystem</span><span class="sxs-lookup"><span data-stu-id="641be-156">SmsRoutedToExternalMessagingSystem</span></span>  <br/> |<span data-ttu-id="641be-157">SMS が外部のメッセージング システムにルーティングするためのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-157">Specifies the icon for SMS routing to an external messaging system.</span></span>  <br/> |
|<span data-ttu-id="641be-158">SmsDelivered</span><span class="sxs-lookup"><span data-stu-id="641be-158">SmsDelivered</span></span>  <br/> |<span data-ttu-id="641be-159">SMS 配信されたメールのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-159">Specifies the SMS delivered mail icon.</span></span>  <br/> |
|<span data-ttu-id="641be-160">OutlookDefaultForContacts</span><span class="sxs-lookup"><span data-stu-id="641be-160">OutlookDefaultForContacts</span></span>  <br/> |<span data-ttu-id="641be-161">連絡先の既定のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-161">Specifies the default icon for contacts.</span></span>  <br/> |
|<span data-ttu-id="641be-162">AppointmentItem</span><span class="sxs-lookup"><span data-stu-id="641be-162">AppointmentItem</span></span>  <br/> |<span data-ttu-id="641be-163">予定項目のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-163">Specifies the appointment item icon.</span></span>  <br/> |
|<span data-ttu-id="641be-164">AppointmentRecur</span><span class="sxs-lookup"><span data-stu-id="641be-164">AppointmentRecur</span></span>  <br/> |<span data-ttu-id="641be-165">定期的な予定のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-165">Specifies the recurring appointment icon.</span></span>  <br/> |
|<span data-ttu-id="641be-166">AppointmentMeet</span><span class="sxs-lookup"><span data-stu-id="641be-166">AppointmentMeet</span></span>  <br/> |<span data-ttu-id="641be-167">会議アイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-167">Specifies the meeting icon.</span></span>  <br/> |
|<span data-ttu-id="641be-168">AppointmentMeetRecur</span><span class="sxs-lookup"><span data-stu-id="641be-168">AppointmentMeetRecur</span></span>  <br/> |<span data-ttu-id="641be-169">定期的な会議のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-169">Specifies the recurring meeting icon.</span></span>  <br/> |
|<span data-ttu-id="641be-170">AppointmentMeetNY</span><span class="sxs-lookup"><span data-stu-id="641be-170">AppointmentMeetNY</span></span>  <br/> |<span data-ttu-id="641be-171">会議への暫定的な応答のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-171">Specifies the icon for a tentative response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="641be-172">AppointmentMeetYes</span><span class="sxs-lookup"><span data-stu-id="641be-172">AppointmentMeetYes</span></span>  <br/> |<span data-ttu-id="641be-173">会議の指定承認アイコンです。</span><span class="sxs-lookup"><span data-stu-id="641be-173">Specifies the meeting acceptance icon.</span></span>  <br/> |
|<span data-ttu-id="641be-174">AppointmentMeetNo</span><span class="sxs-lookup"><span data-stu-id="641be-174">AppointmentMeetNo</span></span>  <br/> |<span data-ttu-id="641be-175">会議の辞退したアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-175">Specifies the meeting declined icon.</span></span>  <br/> |
|<span data-ttu-id="641be-176">AppointmentMeetMaybe</span><span class="sxs-lookup"><span data-stu-id="641be-176">AppointmentMeetMaybe</span></span>  <br/> |<span data-ttu-id="641be-177">会議にも応答のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-177">Specifies the icon for a maybe response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="641be-178">AppointmentMeetCancel</span><span class="sxs-lookup"><span data-stu-id="641be-178">AppointmentMeetCancel</span></span>  <br/> |<span data-ttu-id="641be-179">会議キャンセルのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-179">Specifies the meeting cancel icon.</span></span>  <br/> |
|<span data-ttu-id="641be-180">AppointmentMeetInfo</span><span class="sxs-lookup"><span data-stu-id="641be-180">AppointmentMeetInfo</span></span>  <br/> |<span data-ttu-id="641be-181">会議を指定する情報のアイコンです。</span><span class="sxs-lookup"><span data-stu-id="641be-181">Specifies the meeting information icon.</span></span>  <br/> |
|<span data-ttu-id="641be-182">TaskItem</span><span class="sxs-lookup"><span data-stu-id="641be-182">TaskItem</span></span>  <br/> |<span data-ttu-id="641be-183">作業項目のアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-183">Specifies the task item icon.</span></span>  <br/> |
|<span data-ttu-id="641be-184">TaskRecur</span><span class="sxs-lookup"><span data-stu-id="641be-184">TaskRecur</span></span>  <br/> |<span data-ttu-id="641be-185">定期的なタスクのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-185">Specifies the recurring task icon.</span></span>  <br/> |
|<span data-ttu-id="641be-186">TaskOwned</span><span class="sxs-lookup"><span data-stu-id="641be-186">TaskOwned</span></span>  <br/> |<span data-ttu-id="641be-187">アイコンを所有するタスクを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-187">Specifies the task owned icon.</span></span>  <br/> |
|<span data-ttu-id="641be-188">TaskDelegated</span><span class="sxs-lookup"><span data-stu-id="641be-188">TaskDelegated</span></span>  <br/> |<span data-ttu-id="641be-189">委任されたタスクのアイコンを指定します。</span><span class="sxs-lookup"><span data-stu-id="641be-189">Specifies the task delegated icon.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="641be-190">備考</span><span class="sxs-lookup"><span data-stu-id="641be-190">Remarks</span></span>

<span data-ttu-id="641be-191">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="641be-191">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="641be-192">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="641be-192">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="641be-193">要素情報</span><span class="sxs-lookup"><span data-stu-id="641be-193">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="641be-194">名前空間</span><span class="sxs-lookup"><span data-stu-id="641be-194">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="641be-195">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="641be-195">Schema name</span></span>  <br/> |<span data-ttu-id="641be-196">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="641be-196">Types schema</span></span>  <br/> |
|<span data-ttu-id="641be-197">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="641be-197">Validation file</span></span>  <br/> |<span data-ttu-id="641be-198">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="641be-198">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="641be-199">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="641be-199">Can be empty</span></span>  <br/> |<span data-ttu-id="641be-200">false</span><span class="sxs-lookup"><span data-stu-id="641be-200">false</span></span>  <br/> |
   

