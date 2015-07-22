## Onename Support & FAQ

You'll find answers to some frequently asked questions here. If you cannot find the answer to your question, please email `support@onename.io`.

## General

#### Q: What is Onename?

Onename is a BlockchainID registrar and directory service. We help you get a BlockchainID and then create a user profile. And the best part is that we do it in a way that puts you in control.

#### Q: What do you mean I'm in control?

Unlike most services on the web today, Onename is not a walled garden. Instead, it is completely decentralized. Instead of issuing our own usernames in a closed namespace, we're using an open namespace on which anyone can register names. Instead of storing our user profiles in our private database, we store them in an open database called the blockchain for anyone to read.

#### Q: How can I trust the user profile data you display is correct?

If you view our site, you are viewing data that we are directly reading from the blockchain. However, you shouldn't take our word for it - you can always check the blockchain yourself and verify this data.

#### Q: I've heard there are multiple blockchains? Which one are you using?

The namespace we are using resides in the Namecoin blockchain, but any other blockchain could have worked as well.

#### Q: If I don't want to register a username and profile through your site, can I do it myself?

Absolutely! You'll basically need to (1) download a copy of namecoin-qt or namecoind (2) issue a command to register a name (3) issue a command to update your profile. You can find more information [here](https://github.com/blockstack/registrar).

## Accounts

#### When I signed up, I chose a password and was asked to download an account backup file. What is the file for?

The backup file you downloaded is the mechanism we use to let you reset your password. Make sure you safeguard it because without it, you won't be able to reset your password if you forget it.

#### If I forget my password, how can I recover it?

Just go to https://onename.io/reset and you will be able to follow the steps to reset your password. At some point you'll be asked to upload the file you downloaded, and then you can choose a new password for your account.

#### What happens if I forget both my password and my backup file?

As we mention above, your account backup file is required for a password reset, so unfortunately, if you lose both your password and backup file, you lose access to your account.

#### [Early User] When I signed up, I was given a 12-word passphrase and emailed a backup code. How does this work?

We asked our early users (signed up before summer 2014) to write down a 12-word passphrase that gave them access to their accounts. And just in case they lost the passphrase, we emailed them a backup code. If you were one of these users, you can log in to Onename with your email and the 12-word passphrase as the password. Then, if you'd like, you can update your password at any time.

#### [Early User] What if I forget my 12-word passphrase?

If you forgot your passphrase, you can go to https://onename.io/reset to reset your password and regain access to your account. You'll be asked to retreive the backup code that was emailed to you when you signed up.

#### [Early User] What if I forgot my 12-word passphrase and I no longer have the backup code that was emailed to me when I signed up?

Unfortunately, the backup code is the only way for us to help you recover your 12-word passphrase and reset your account. So if you lost both your 12-word passphrase and your backup code, you will no longer have access to your account.

## Bitcoin Address

#### Q: How does the automatically generated Bitcoin address work?</a>

If you do not provide a Bitcoin address during registration, Onename will generate one for you. The private key of this Bitcoin address is saved on our servers encrypted with your password (we do *not* have access to the private key). The private key is also stored in the backup file that you saved on Dropbox/Gdrive.

#### Q: How can I change the Bitcoin address?</a>

You can change your Bitcoin address by editing your profile. You can use any Bitcoin address you want e.g., from Coinbase, Blockchain.info etc. Just make sure that you actually own that address before putting it in your profile.

## Private Keys

#### Q: Who has my private key? 

Only you have access to your private key. Onename encypts your private key with the password that you provided and keeps the encrypted copy on our servers. If you forget your password then you can use the backup file you saved during signup to recover the private key. 

## Public PGP Keys

#### Q: Can I host my own .asc, .pgp, .gpg or .key file? 

Yes, but make sure the mime type is set on your server so that your key file is displayed in the browser as plain text. If the browser tries to send the file to the client as a download, the PGP feature on Onename will not work for you. On a NodeJS/Express server, just add this line to your server.js or app.js file.. ie: 
express.static.mime.define({'text/plain': ['asc']});

## Verifications

#### Q: Why do I need to publicly tweet/post and not delete the tweet/post?

Verifications need to be independently and publicly verifiable i.e., any person who wants to verify the proof should be able to look at it hence the post/tweet needs to be public. Further, Onename can't vouch for the proof on behalf of any user (this is more secure than trusting any single service) meaning you can't auth your Twitter/Facebook with Onename and then try to use that as a proof.

#### Q: Why is my Twitter/Facebook/Github verification not showing up?

*Possible Reason #1) Incorrect proof text:* The verification text needs to be exact, more specifically "Verifying myself: My Bitcoin username is +<username>" needs to be in the text. This requirement is because of security reasons and we can't allow arbitrary methods of phrasing the proof text. 

*Possible Reason #2) Incorrect URL to proof:* You can view your profile data by clicking on "Profile Data" on the left-bottom corner of your profile or by appending ".json" to your profile URL. An examples profile data is [here](https://onename.io/barrysilbert.json). Your profile data will list URLs to different proofs. Make sure that if you visit the proof URL (of Github/Facebook/Twitter) you can see the proof text on that URL. This URL needs to be publicly readable (private accounts don't work). 

#### Q: Do I have to have a Twitter, Facebook AND Github account in there for Verification?

No, but the more you are Verified, the more your associates can trust that your Onename profile is actually you.

## Profile Data

#### Q: How do I put custom data in my profile?

We currently don't support that feature but stay tuned.

#### Q: Why does the DNSchain still say that my username is not found?

First, make sure your username only has lowercase letters. Second, note that it can take a few hours to a day for your username to be fully registered on the Namecoin Blockchain. After that, updates to your profile should only take somewhere between 10 minutes and a couple of hours.

#### Q: How can I find my profile data in the blockchain? 

You can use any Namecoin blockchain explorer to find your record/data in the blockchain. Some examples are a) [Namecha.in](http://namecha.in/name/u/barrysilbert) and b) [Webbtc](http://namecoin.webbtc.com/name/u/barrysilbert).
