# GTM-Consent-Mode
Read more here about Consent Mode -> https://support.google.com/analytics/answer/9976101?hl=en and here https://developers.google.com/tag-platform/devguides/consent
Privacy regulations, such as the European Union's GDPR, restrict websites from gathering information about visitors without their consent. Users commonly provide consent by interacting with a consent banner. Depending on how your products are configured, Google uses mechanisms such as cookies or HTTP requests that include user data to support analytics, conversion measurement, and remarketing.

You can configure these mechanisms to be consent-aware. When consent-aware, tag functionality depends upon the level of consent. For example, you can configure Google tags to not write or read cookies until the user provides consent. When a visitor grants consent, it restores tag functionality, based on the behavior you configure.

Follow these steps to set up correctly:
1. Download a template from the template gallery.
2. Create a new Tag with the Consent mode template, which will trigger on Consent Initialization trigger type.
 - 'Consent Command' should be 'Default'.
 - Click 'Add settings' to be able to add Advertising, Analytics, Personalization consent states. (Here you can select your Variable which can be false, true, granted or denied).
3. Create another new tag with a Consent mode template that will trigger when a user updates the consent status on your website.
 - 'Consent Command' should be 'Update'.
 - Click Add settings to be able to add Advertising, Analytics, Personalization consent states. (Here you can select your Variable which can be false, true, granted or denied)
4. Publish changes.

> Note:
> granted or true - means that the user has agreed to collect certain data.
> denied or false - means that the user has not agreed to the data collection.
