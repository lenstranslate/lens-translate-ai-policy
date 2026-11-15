# Privacy Policy — Lens Translate AI

**Last updated: 15 November 2026**

> DRAFT. Engineering-authored and matched to the code as written. Before publishing
> on Google Play, replace the contact address, confirm the translation
> provider's current retention terms, and have it reviewed by a qualified
> professional if you are selling subscriptions in the EU.

## 1. Who we are

Lens Translate AI ("the app", "we") is a photo translation application for
Android. The app is designed to work without an account, and we do not operate a
server that stores your translations.

Contact: `lens56315@gmail.com`
Published: https://lenstranslate.github.io/lens-translate-ai-policy/

## 2. Summary

- Your **photographs are never uploaded**. Text recognition runs on your phone.
- Only the **recognised text** is sent to a translation service, and only when you
  start a translation and no on-device engine is available.
- No account. No analytics SDK. No advertising SDK in this version.
- Your history is stored **only on your phone**, and you can delete it at any time.

## 3. What is processed on your device

| Data | Purpose | Storage |
| --- | --- | --- |
| Photograph you select or capture | Text recognition | App cache; a compressed copy is kept only if you save the translation |
| Recognised text | Display, translation, history | SQLite in the app sandbox |
| Translated text | Display, history | SQLite in the app sandbox |
| Language pair, theme, engine choice | Preferences | SQLite in the app sandbox |
| Daily usage counters | Free-tier limits | SQLite in the app sandbox |
| On-device translation models | Offline translation | Downloaded by the app to your phone (about 30 MB per language) |

Text recognition uses Google ML Kit's on-device text recognition. On-device
translation uses Google ML Kit's on-device translation. Both run locally; ML Kit
does not transmit the image or the text.

## 4. What leaves your device

**Cloud translation.** When on-device translation is unavailable for your language
pair (or you choose "Cloud"), the recognised text is sent over HTTPS to:

- **MyMemory** — `https://api.mymemory.translated.net`

What is sent: the recognised text and the source/target language codes.
What is **not** sent: your photograph, your name, your email, your device
identifier, your location, or any account identifier (the app has no account).

MyMemory is a third-party free service. Its own privacy practices govern text
after it reaches their servers; consult their policy. **If you are translating
confidential documents, use on-device translation instead.**

**Speech recognition.** Voice features use your phone's speech service (usually
Google's). Depending on your device configuration, audio may be processed by that
provider. This is controlled by your device settings and Android, not by this app.
The microphone is active only while you hold an active listening session.

**Purchases.** If you subscribe, Google Play processes the payment. We never
receive your card details. Only the entitlement status (active/inactive) is read
from Play Billing.

## 5. What we do NOT do

- We do not upload your photographs.
- We do not create user accounts or ask for an email.
- We do not include advertising or analytics SDKs in this version.
- We do not sell data.
- We do not send text in the background.

If advertising is added later, this policy will be updated before that build is
released, and ads will never cover translation results or the camera capture
surface.

## 6. Retention and deletion

All app data lives in the app's private storage on your phone. You can delete it
at any time:

- **History → Clear history** — deletes stored translations (favourites are kept
  unless you confirm full deletion).
- **Settings → Delete all history** — removes all translations and stored images.
- **Settings → Reset app settings** — returns preferences to defaults.
- **Uninstalling the app** removes everything the app stored.

We hold no server-side copy of your translations, so there is nothing for us to
delete on our side.

## 7. Legal bases (GDPR, for EU users)

Where the GDPR applies:

- **Legitimate interest / performance of a contract** — processing necessary to
  provide the translation you requested.
- **Consent** — cloud translation of text, which you trigger explicitly and can
  avoid entirely by using on-device translation.

## 8. Your rights

You may request access, rectification, erasure, restriction, portability, or
object to processing. Because the app stores data locally, you can exercise most
of these directly (see section 6). For data already transmitted to a translation
provider, contact us and we will help you raise the request with that provider.
You may also complain to your local supervisory authority.

## 9. Children

The app is not directed at children under 13 and does not knowingly collect
personal information from children.

## 10. Security

- All network requests use HTTPS.
- The app contains no API keys or secrets.
- App data sits in Android's per-app sandbox.
- On-device processing is used wherever technically possible.

No system is perfectly secure. Avoid translating highly sensitive documents with
cloud translation enabled.

## 11. Changes

Material changes will be shown in the app before taking effect, with the updated
date at the top of this policy.

## 12. Contact

`support@lenstranslate.example`

---

### Data safety summary (for the Play Console form)

| Question | Answer |
| --- | --- |
| Does the app collect or share user data? | Yes — "Text" and "Photos" categories; see below |
| Photos | Accessed on device, **not** collected, **not** shared |
| Text (recognised) | Shared with a translation provider when cloud translation is used |
| Approximate location / precise location | Not collected |
| Personal info (name, email, phone) | Not collected |
| Financial info | Not collected by us (Google Play handles payments) |
| Health / fitness | Not collected |
| Messages / contacts / calendar | Not collected |
| App activity / in-app search | Not collected |
| Device or other IDs | Not collected |
| Data encrypted in transit | Yes (HTTPS) |
| User can request deletion | Yes, in-app (History and Settings) |
| Data collected for advertising | No |
