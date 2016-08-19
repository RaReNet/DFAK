# Establishing Trust

Above, we mention some basic ways to begin to [establish trust](https://hackpad.com/The-Digital-First-Aid-Kit-PdhSvxKOM5M#:h=Trust) between someone seeking help and someone helping out. This section addresses how to add a technical layer of trust onto that, and understand the tools that help you maintain a secure conversation with only the person you think you're conversing with. It's important to note that while this section is rather technical, do the best you can - it is better to use encryption tools than to not use them!

Encryption tools like OTR ("Off The Record") and PGP ("Pretty Good Privacy") provide many benefits. Encrypted messages or files with OTR or PGP are protected from anyone peeking at them or tampering with them from when they leave your computer until they reach their destination. The problem, though, is knowing for certain if their destination is the 'right' one.

To use encryption tools like these, you must know the right address to send the encrypted message to - this is not just an email account or IM nickname, but requires more specific information - the encryption 'key' that goes with that account. Most of this is managed by your computer, but it is important for you to provide the final sign-off! Theoretically, if you were trying to establish secure communications with someone, an attacker could replace the specific encryption information with their own and read your communication. To defend against this, there are a few tricks.

## Website Trust
Secure websites (those starting with HTTPS) have a system where browsers rely on a limited number of trustworthy companies to manage this. This makes it relatively easy for users, but if any of these companies are compromised (which has happened!) or are willing to cooperate with a government that may be a threat to you, the entire trust network becomes a problem (this same model is also used for a specific type of email security which is called S/MIME).

## Trust in Communication Tools
For email, chat and secure phone calls, it is a bit more 'direct.' The ideal situation is that you meet someone in person to exchange the fingerprint information. There is no risk of someone 'intercepting' and changing this in a face-to-face meeting! Obviously that's not always possible. Different tools have different ways around this problem. [Security in a Box has an entire chapter](https://securityinabox.org/en/chapter-7) devoted to private communications.

### Chat: 'OTR'
In chat or instant messaging, the current standard for trust is called OTR, or Off The Record. This is not the same as 'off the record' messaging in GChat, which only means that Google does not store a permanent log of the conversation. OTR provides the basic benefits above (secured end-to-end and proof against tampering), but notably also provides an additional layer of security - each conversation session is protected separately. This means that if someone is able to store all of your private chat conversations, breaking the encryption of one chat provides no ability to read any of the other chats. This also allows a degree of 'deniability,' i.e while your conversation is protected and authenticated, there is no way to prove that any of the messages came from you as opposed to someone else. OTR works in Adium, Jitsi and [Pidgin](https://securityinabox.org/en/pidgin_main).

To benefit from all of this, however, you must find a way to 'authenticate' the person you are chatting with.  You only have to do this once per device for each secure contact (and you can use apps like [KeySync](https://guardianproject.info/apps/keysync/) to help). The key to linking this digital trust with a person you know is through a shared secret - you can call each other and directly compare a code unique to your accounts, or use a question-and-answer method where you know only this specific person would know a secret word you've agreed on or a specific piece of private information.

Resources:s
• Authentication in OTR: [https://securityinabox.org/en/pidgin_securechat](https://securityinabox.org/en/pidgin_securechat)
• OTR Technical details: [https://otr.cypherpunks.ca/](https://otr.cypherpunks.ca/)
• Email: PGP

## Trust in Email: PGP

PGP (or Pretty Good Privacy) and its open source equivalent, GPG (Gnu Privacy Guard) allow you to encrypt emails and files for yourself or to send to others.  With plugins like [Enigmail for Thunderbird](https://securityinabox.org/en/thunderbird_main) or [GPGOL](http://www.gpg4win.org/) for Outlook, you can use PGP very effectively to protect the contents of your email (though not the subject, or who you're emailing with).

To send a PGP encrypted email, you do not need your own PGP keys. PGP Keys come in pairs, a public one and a private one.  The public one is like a house address that anyone can know but only someone with the 'private' key can access the account to receive messages sent to that address. By the same magic of PGP, only the person at that address (with the private key) can send messages out from that address (which can be verified by the public part of the key). See the resources listed below for more in-depth discussions on how PGP works.

The problem, of course, is finding the public key 'address' - there are digital phonebooks for PGP keys where you can search for emails or names ([https://sks-keyservers.net/i/#extract](https://sks-keyservers.net/i/#extract) and [https://pgp.mit.edu/](https://pgp.mit.edu/) are popular) - but there is no central authority guaranteeing that these keys belong to the right person. It's completely possible that someone has uploaded their own key and even a fake email address, impersonating someone else.

Again, the trick is to verify that the key is correct using another method - many people will exchange slips of paper with their key 'fingerprint' (see some at the top of this document associated with email help-desks!), or post them on their twitter profiles or web pages. The problem is that this only works for a small community of friends, not on a global internet scale.

For people who are relatively safe and can be public about their contact network, you can 'sign' the PGP keys of other people you have met and verified. This helps fix the trust problem by creating a 'web of trust,' i.e. if you have verified someone's key and you trust them to verify the keys of others, you can also trust any key they have signed off on.

Generally, however, this is not a huge problem as long as you have reasonable trust that you have the right key and right email address of the person you want to communicate with, and treat any unexpected changes in keys and email addresses with suspicion.

Resources:
• [https://pressfreedomfoundation.org/encryption-works#pgp](https://pressfreedomfoundation.org/encryption-works#pgp)
• [https://www.cryptoparty.in/brief#crypto](https://www.cryptoparty.in/brief#crypto)

## Trust in Encrypted Voice: ZRTP

### Encrypted Voice: ZRTP
ZRTP is in many ways similar to OTR, in that it changes for every conversation, protecting the history of your communications.  ZRTP is the standard in fully encrypted voice calls (using [Jitsi](https://securityinabox.org/en/jitsi), [RedPhone](https://whispersystems.org/#privacy), or [Silent Circle](https://silentcircle.com/)). It requires you to read aloud a short series of characters to the person you're speaking with in order to authenticate the call using your voice in combination with these unique characters.

Resources:
• [https://jitsi.org/Documentation/ZrtpFAQ#faqHow](https://jitsi.org/Documentation/ZrtpFAQ#faqHow)
• [https://silentcircle.com/web/faq-zrtp/?#7](https://silentcircle.com/web/faq-zrtp/?#7)
