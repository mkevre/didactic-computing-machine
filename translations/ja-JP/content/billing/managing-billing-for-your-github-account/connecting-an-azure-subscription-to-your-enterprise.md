---
title: Azure サブスクリプションを Enterprise に接続する
intro: 'Microsoft Enterprise Agreement を使用して、Enterprise に含まれている金額を超える {% data variables.product.prodname_actions %} および {% data variables.product.prodname_registry %} の使用を有効化して支払うことができます。'
redirect_from:
  - /github/setting-up-and-managing-your-enterprise/managing-your-enterprise-account/connecting-an-azure-subscription-to-your-enterprise
  - /github/setting-up-and-managing-billing-and-payments-on-github/connecting-an-azure-subscription-to-your-enterprise
  - /github/setting-up-and-managing-your-enterprise/connecting-an-azure-subscription-to-your-enterprise
versions:
  ghec: '*'
shortTitle: Connect an Azure subscription
---

## Azure サブスクリプションと {% data variables.product.product_name %}

{% data reusables.enterprise-accounts.billing-microsoft-ea-overview %} 詳しい情報については、「[{% data variables.product.prodname_actions %} の支払いについて](/billing/managing-billing-for-github-actions/about-billing-for-github-actions)」および「[{% data variables.product.prodname_registry %} の支払いについて](/billing/managing-billing-for-github-packages/about-billing-for-github-packages)」を参照してください。

Azure サブスクリプションに接続した後、利用上限を管理することもできます。 アカウントの利用上限の管理と変更については、「[{% data variables.product.prodname_registry %} の利用上限の管理](/billing/managing-billing-for-github-packages/managing-your-spending-limit-for-github-packages)」および「[{% data variables.product.prodname_actions %} の利用上限の管理](/billing/managing-billing-for-github-actions/managing-your-spending-limit-for-github-actions)」を参照してください。

## Azure サブスクリプションを Enterprise アカウントに接続する

Azure サブスクリプションに接続するには、サブスクリプションに対するオーナーのアクセス許可が必要です。

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.billing-tab %}
{% data reusables.enterprise-accounts.payment-information-tab %}
1. [Payment Information] で、[**Add Azure Subscription**] をクリックします。
1. 画面の指示に従って Microsoft アカウントにサインインします。
1. [Permissions requested] という画面表示を確認します。 規約に同意する場合は、[**Accept**] をクリックします。
1. [Select a subscription] で、Enterprise に接続する Azure サブスクリプション ID を選択します。

   {% note %}

   **Note:** {% data variables.product.company_short %}'s Subscription Permission Validation requests read-only access to display the list of available subscriptions. To select an Azure subscription, you must have owner permissions to the subscription. If the default tenant does not have the right permissions, you may need to specify a different tenant ID. For more information, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-authorization-code) in Microsoft Docs.

   {% endnote %}
1. [**Connect**] をクリックします。

## Enterprise アカウントから Azure サブスクリプションを切断する

Azure サブスクリプションを Enterprise アカウントから切断すると、プランに含まれている金額以上の使用量を利用できなくなります。

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.billing-tab %}
{% data reusables.enterprise-accounts.payment-information-tab %}
1. [Azure subscription] の下で、切断するサブスクリプション ID の右側にある [**{% octicon "trash" aria-label="The trash icon" %}**] をクリックします。
1. 画面表示を確かめてから、[**Remove**] をクリックします。