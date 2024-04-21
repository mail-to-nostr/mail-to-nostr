# mail-to-nostr.com

mail-to-nostr.com is a Mail to Nostr one-way gateway. It forwards mails send to your public key as direct message to your nostr account.

# Motivation

We often came over websites in the internet, where we just need a throwaway mail address. We know there are services where you can generate some but we were just thinking, why not just relay it to your nostr account? And here we are.

# How does it work

Just use your publickey @ mail-to-nostr.com and every mail which will be send there will be forwarded to your nostr account.

You can use the hexadecimal version, like 0123456789ABCDEF...0123456789ABCDEF@mail-to-nostr.com or the npub version like npub...@mail-to-nostr.com

# Technically

Some technical aspects of the service. Which of course could change over time.

## General

- Forward mails to @mail-to-nostr.com to the public keys provided
- Support 0123456789ABCDEF...0123456789ABCDEF public key
- Support npub... public key
- Mails are forwarded as private message
- Plain text mail content ist forwarded as presented
- HTML mail content is converted to markdown and forwarded
- Mail Attachments are not send and dropped
- We provide some basic mail header information to the recipient
- Answering to mails is not possible, we are a mail to nostr one way
- There is a rate limit active to counteract spammers
- There are ip bans active to counteract spammers

## Relays

Right now we are connected to following nostr relays:

- wss://relay.damus.io
- wss://nos.lol
- wss://nostr.wine
- wss://nostr.oxtr.dev
- wss://relay.snort.social
- wss://relay.current.fyi

If you point your client here you should get the direct messages.

## Rate Limit and Bans

For now we use rate limits, to prevent addresses to be spammed. It is mail sender server sensitive and receiver public key.

If you violate the limits to heavy your /24 ip pool will be banned from using mail-to-nostr.com for a certain time. Also we ban typical spamming patterns we see. Also the whole /24 ip pool. We may easy that in the future, but for now it's that.

## Open Sourcing

We are thinking about open sourcing the base functions of the gateway. But as always, limit time, limit resources.

## Free of charges

For now using the service is free of charges. But it is not guaranteed, that it always stays this way, depending if some relays will start charging for direct messages.

# Privacy

Is it save and private to use? Not much more save and private then other services in the web. We are not reading or saving any data but theoretically we could, of course. So don't use it for any conversation where you really want to be private.

And again for the nation states: WE ARE NOT SAVING ANY DATA. So don't bother us with requests.

# Disclaimer

mail-to-nostr.com only serves as mail to nostr gateway.
We are not responsible for any mail content. Please address any complaints directly to the mails author.
We don't save any data about the mails author or the mail.
The content of the mail is provided "as is", with no guarantees of completeness, accuracy, usefullness or timeliness.
There is no guarantees for the server running all the time. Downtimes are to be expected.
By using this service you accept this conditions and terms.

# Contact

You can reach us here npub14e8g06yf0kp900vu3mq8fu9jhl6pueh4xpc7u0lly5wuvug8e7gqr96utv
