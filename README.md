## Onename Support & FAQ

You'll find answers to some frequently asked questions here. If you cannot find the answer to your question, please email `support@onename.io`.

## General

#### Q: What is OneName?

Think of us as the user directory for Bitcoin. We help you get a Bitcoin username and then create a Bitcoin profile. And the best part is that we do it in a way that puts you in control.

#### Q: What do you mean I'm in control?

Unlike most services on the web today, OneName is not a walled garden. Instead, it is completely decentralized. Instead of issuing our own usernames in a closed namespace, we're using an open namespace on which anyone can register names. Instead of storing our user profiles in our private database, we store them in an open database called the blockchain for anyone to read.

#### Q: How can I trust the user profile data you display is correct?

If you view our site, you are viewing data that we are directly reading from the blockchain. However, you shouldn't take our word for it - you can always check the blockchain yourself and verify this data.

#### Q: I've heard there are multiple blockchains? Which one are you using?

The namespace we are using resides in the Namecoin blockchain, but any other blockchain could have worked as well.

#### Q: If I don't want to register a username and profile through your site, can I do it myself?

Absolutely! You'll basically need to (1) download a copy of namecoin-qt or namecoind (2) issue a command to register a name (3) issue a command to update your profile. You can find more information [here](http://github.com/opennamesystem).

## Accounts

#### When I signed up, I was given a 12-word passphrase. What if I forgot it?

If you forgot your login information, you can go to https://onename.io/reset to reset your password and regain access to your account.

## Bitcoin Address

#### Q: How does the automatically generated Bitcoin address work?</a>

If you do not provide a Bitcoin address during registration, Onename will generate one for you. The private key of this Bitcoin address is saved on our servers encrypted with your password (we do *not* have access to the private key). The private key is also stored in the backup file that you saved on Dropbox/Gdrive.

#### Q: How can I change the Bitcoin address?</a>

You can change your Bitcoin address by editing your profile. You can use any Bitcoin address you want e.g., from Coinbase, Blockchain.info etc. Just make sure that you actually own that address before putting it in your profile.  

## Private Keys

#### Q: Who has my private key? 

Only you have access to your private key. Onename encypts your private key with the password that you provided and keeps the encrypted copy on our servers. If you forget your password then you can use the backup file you saved during signup to recover the private key. 

## Verifications

#### Q: Why do I need to publicly tweet/post and not delete the tweet/post?

Verifications need to be independently and publicly verifiable i.e., any person who wants to verify the proof should be able to look at it hence the post/tweet needs to be public. Further, Onename can't vouch for the proof on behalf of any user (this is more secure than trusting any single service) meaning you can't auth your Twitter/Facebook with Onename and then try to use that as a proof.

#### Q: Why is my Twitter/Facebook/Github verification not showing up?
The verification text needs to be exact, more specifically "Verifying myself: My Bitcoin username is +<username>" needs to be in the text. This requirement is because of security reasons and we can't allow arbitrary methods of phrasing the proof text. 

## Profile Data

#### Q: How do I put custom data in my profile?

We currently don't support that feature but stay tuned.
