---

copyright:
  years: 2019
lastupdated: "2019-06-13"

keywords: IAM, identity, access management, role

subcollection: hyper-protect-dbaas-for-mongodb

---

{:shortdesc: .shortdesc}
{:external: target="_blank" .external}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:important: .important}

# Identity and Access Management 角色及動作
{: #iam}

您帳戶中使用者的 {{site.data.keyword.cloud_notm}} {{site.data.keyword.ihsdbaas_mongodb_full}} 服務實例存取權是由 {{site.data.keyword.cloud_notm}} Identity and Access Management (IAM) 所控制。每位存取您帳戶中 {{site.data.keyword.cloud_notm}} {{site.data.keyword.ihsdbaas_mongodb_full}} 服務的使用者都必須獲指派已定義 IAM 角色的存取原則。此原則決定使用者可在所選取服務或實例環境定義內執行的動作。容許的動作是由 {{site.data.keyword.cloud_notm}} 服務自訂及定義為容許對服務執行的作業。動作接著會對映至 IAM 使用者角色。
{: shortdesc}

原則會啟用在不同層次授與的存取權。部分選項包括下列項目：

* 您帳戶中所有服務實例的存取權
* 您帳戶中個別服務實例的存取權
* 實例內特定資源的存取權

在您定義存取原則的範圍之後，請指派可決定使用者存取層次的角色。請檢閱下列各表，以概述每個角色在 {{site.data.keyword.cloud_notm}} {{site.data.keyword.ihsdbaas_mongodb_full}} 服務內容許的動作。

下表詳述對映至平台管理角色的動作。平台管理角色可讓使用者對平台層次的服務資源執行作業，例如指派使用者對服務的存取權、建立或刪除實例，以及將實例連結至應用程式。

|平台管理角色|動作說明|範例動作                                                 |
|------------------------|----------------------|----------------------------------------------------------------|
|檢視者                  |可以檢視服務實例，但無法進行修改|<ul><li>列出叢集</li><li>檢視叢集的詳細資料</li></ul>|
|編輯者                  |執行所有平台動作，但管理帳戶以及指派存取原則除外|<ul><li>將服務連結至叢集</li></ul>|
|操作員                  |執行配置及操作服務實例所需的平台動作，例如檢視服務的儀表板|<ul><li>將服務連結至叢集</li></ul>|
|管理者                  |根據將指派此角色的資源來執行所有平台動作，包括將存取原則指派給其他使用者|<ul><li>移除叢集</li><li>建立叢集</li><li>更新使用者存取原則</li><li>檢視者、編輯者及操作員可執行的所有動作</li></ul>|
{: caption="表 1. IAM 使用者角色及動作"}

如需在使用者介面中指派使用者角色的相關資訊，請參閱[管理對資源的存取權](/docs/iam?topic=iam-iammanidaccser#iammanidaccser)。
