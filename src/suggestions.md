# Suggestions

This feature allows people to suggest features for your server, or service (depending on how you intend to use it).

> **Note**
>
> Anitra requires the `Send Messages` and `Embed Links` permissions to do this. This includes every [channel](#what-does-each-channel-mean) that has been enabled.

## Setup

Firstly, you (as an administrator) need to setup a `Pending` channel, before doing anything else. This can be set up using the `/suggestions configure channel type:Pending channel:#channel`

Secondly, you have to actually enable the feature. This can be achieved by running `/suggestions configure enabled:True`.

After these are both configured, you will be able to enable other channels. Alternatively you could only enable the `Pending` channel only. People will still be able to submit suggestions using `/suggest`.

### What does each channel mean?

Here is a detailed tabel explaining each channel type's purpose:

| Channel Type | Purpose                                                                                       | Required? |
| ------------ | --------------------------------------------------------------------------------------------- | --------- |
| Approving    | The channel to post suggestions that have been approved by administrators.                    | No        |
| Pending      | The channel to post suggestions that have been sent and are being reviewed by administrators. | Yes       |
| Denied       | The channel to post suggestions that have been denied by administrators.                      | No        |

<br>

Decided that you no longer want to use this feature? No problem! Simply run `/suggestions configure enabled:False` to do this.

## Managing Suggestions

Now that we've enabled suggestions, how do we actually manage them?

This can be achieved by running `/suggestions <approve|deny> suggestion:ID reason:reason`.

Some examples could be:
- `/suggestions approve suggestion:42 reason:This is indeed a great suggestion! We shall implement it right away.`
- `/suggestions deny suggestion deny suggestion:70 reason:This is a good suggestion, however due to a Discord limitation, we are unable to achieve this.`

