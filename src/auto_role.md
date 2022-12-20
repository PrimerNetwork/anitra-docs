# Auto Role

The Auto-Role feature is meant to assign a person a role when they join the server.

You *are* able to specify what role(s) should be assigned to bot accounts upon join, and to people upon join.

> **Note**
>
> Anitra requires the `Manage Roles` permission for this to work.
>
> Anitra also needs to be above the role(s) you would like to add to the Auto Role feature.
>
> ![Role hierarchy fix](../assets/role_hierarchy_fix.gif)

## Examples

### User Accounts

Let's say that we want bot accounts to recieve the `test-bot` role, we would have run `/autorole add bot role: @test-bot`, and this would happen whenever a bot joins:

![Role assigned to bot](../assets/bot_join.png)

### Bot Accounts

Now let's say we wanted user accounts (people) to recieve the `member` role, we would _then_ run `/autorole add user role: @Member`, which would then lead to this happen when ever a person joins:

![Role assigned to a person](../assets/user_join.png)

## Removing the role(s)

Removing the role(s) that you no longer want to be assigned is as simple as `/autorole remove <user|bot> role: @role`, and Anitra will no longer assign these role(s) to the user/bot accounts.

If you would like to know which role(s) you are able to remove, run `/autorole list`. This will show the list of role(s) that Anitra originally was suppose to assign, which will then allow you to remove the role(s) you desire.
