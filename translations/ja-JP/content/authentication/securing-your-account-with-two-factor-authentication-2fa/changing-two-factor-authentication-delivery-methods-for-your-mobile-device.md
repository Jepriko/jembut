---
title: モバイルデバイスに対する 2 要素認証配信方法の変更
intro: 認証コードの受信方法を、テキストメッセージとモバイルアプリケーションとの間で切り替えることができます。
redirect_from:
  - /articles/changing-two-factor-authentication-delivery-methods
  - /articles/changing-two-factor-authentication-delivery-methods-for-your-mobile-device
  - /github/authenticating-to-github/changing-two-factor-authentication-delivery-methods-for-your-mobile-device
  - /github/authenticating-to-github/securing-your-account-with-two-factor-authentication-2fa/changing-two-factor-authentication-delivery-methods-for-your-mobile-device
versions:
  fpt: '*'
  ghec: '*'
topics:
  - 2FA
shortTitle: Change 2FA delivery method
---

{% note %}

**Note:** Changing your primary method for two-factor authentication invalidates your current two-factor authentication setup, including your recovery codes. Keep your new set of recovery codes safe. Changing your primary method for two-factor authentication does not affect your fallback SMS configuration, if configured. For more information, see "[Configuring two-factor authentication recovery methods](/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication-recovery-methods#setting-a-fallback-authentication-number)."

{% endnote %}

{% data reusables.user_settings.access_settings %}
{% data reusables.user_settings.security %}
3. [SMS delivery] の隣にある [**Edit**] をクリックします。 ![SMS 配信オプションの編集](/assets/images/help/2fa/edit-sms-delivery-option.png)
4. [Delivery options] の下にある [**Reconfigure two-factor authentication**] をクリックします。 ![2FA 配信オプションの切り替え](/assets/images/help/2fa/2fa-switching-methods.png)
5. 2 要素認証を TOTP モバイルアプリケーションで設定するかテキストメッセージで設定するかを決めます。 詳しい情報については「[2 要素認証の設定](/articles/configuring-two-factor-authentication)」を参照してください。
    - TOTP モバイルアプリケーションで 2 要素認証を設定するには、[**Set up using an app**] をクリックします。
    - テキストメッセージ (SMS) で 2 要素認証を設定するには、[**Set up using SMS**] をクリックします。

## 参考リンク

- [2 要素認証について](/articles/about-two-factor-authentication)
- [2 要素認証のリカバリ方法の設定](/articles/configuring-two-factor-authentication-recovery-methods)
