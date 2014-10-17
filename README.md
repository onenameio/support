### Welcome to Onename Support.
You'll find answers to some frequently asked questions here. If you cannot find your question here, feel free to email support@onename.io.

Questions
----

General:
* [What is OneName?](#general_1)
* [What do you mean I'm in control?](#general_2)
* [How can I trust the user profile data you display is correct?](#general_3)
* [I've heard there are multiple blockchains? Which one are you using?](#general_4)
* [If I don't want to register a username and profile through your site, can I do it myself?](#general_5)

Addresses & Private Keys: 
* [How does the automatically generated Bitcoin address work?](#address_1)

Verifications: 
* [Why do I need to publicly tweet/post and not delete the tweet/post?](#verification_1)
* [Why is my Twitter/Facebook/Github verification not showing up?](#verification_2)

General
----

#### <a name="general_1"/>Q: What is OneName?
Think of us as the user directory for Bitcoin. We help you get a Bitcoin username and then create a Bitcoin profile. And the best part is that we do it in a way that puts you in control.

#### <a name="general_2"/>Q: What do you mean I'm in control?
Unlike most services on the web today, OneName is not a walled garden. Instead, it is completely decentralized. Instead of issuing our own usernames in a closed namespace, we're using an open namespace on which anyone can register names. Instead of storing our user profiles in our private database, we store them in an open database called the blockchain for anyone to read.

#### <a name="general_3"/>Q: How can I trust the user profile data you display is correct?
If you view our site, you are viewing data that we are directly reading from the blockchain. However, you shouldn't take our word for it - you can always check the blockchain yourself and verify this data.

#### <a name="general_4"/>Q: I've heard there are multiple blockchains? Which one are you using?
The namespace we are using resides in the Namecoin blockchain, but any other blockchain could have worked as well.

#### <a name="general_5"/>Q: If I don't want to register a username and profile through your site, can I do it myself?
Absolutely! You'll basically need to (1) download a copy of namecoin-qt or namecoind (2) issue a command to register a name (3) issue a command to update your profile. You can find more information [here](http://github.com/opennamesystem).

Addresses & Private Keys.
----

#### <a name="address_1"/>Q: How does the automatically generated Bitcoin address work? 

If you do not provide a Bitcoin address during registration, Onename will generate one for you. The private key of this Bitcoin address is saved on our servers encrypted with your password (we do *not* have access to the private key). The private key is also stored in the backup file that you saved on Dropbox/Gdrive.


Verifications.
----

#### <a name="address_1"/>Q: Why do I need to publicly tweet/post and not delete the tweet/post?
Verifications need to be independently and publicly verifiable i.e., any person who wants to verify the proof should be able to look at it hence the post/tweet needs to be public. Further, Onename can't vouch for the proof on behalf of any user (this is more secure than trusting any single service) meaning you can't auth your Twitter/Facebook with Onename and then try to use that as a proof.  

#### <a name="address_1"/>Q: Why is my Twitter/Facebook/Github verification not showing up?
The verification text needs to be exact, more specifically "Verifying myself: My Bitcoin username is +<username>" needs to be in the text. This requirement is because of security reasons and we can't allow arbitrary methods of phrasing the proof text. 
