**Admin Chatroom** allows admins to talk privately with each other in-game.

[BitBucket IssueTracker](https://bitbucket.org/austinv900/oxide-plugins/issues)

There might be some bugs. Just Post a comment with the error and we will work out the kinks

## Permissions
This plugin uses Oxide's permission system. To assign a permission, use grant user <username|steamid> <permission>. To remove a permission, use revoke user <username|steamid> <permission>.

- **adminchatroom.allowed** -- (allows player to slap other players).

**Ex.** grant user austinv900 adminchatroom.allowed

**Ex.** revoke user austinv900 adminchatroom.allowed

**Ex.** grant group moderator adminchatroom.allowed

## Commands

- `a msg` -- Send a message to the chatroom
- `a <invite/kick> <playerid/playername>` -- Kick or Invite a player to the room.

## Configuration

You can configure the settings in the AdminChatroom.json file under the oxide/config directory.

```json
{
  "General": {
    "Allowed To Join Permission": "AdminChatroom.allowed"
  }
}
```
## Localization

The default messages are in the AdminChatroom.en.json under the oxide/lang directory. Language files are also available for French,German, Russian, and Spanish. To add support for another language, just copy one of the defaults, change the language code (en, fr, de, ru, or es), and then customize the messages.

```json
{
  "ChatFormat": "[AdminChat] {0}: {1}",
  "NotInvited": "You have not have access to this chatroom",
  "PlayerAdded": "{0} has been added to the admin chat",
  "PlayerRemoved": "{0} has been kicked from the chatroom",
  "SendCommandInfo": "You have been invited to the admin chatroom. please use /{0} msg - To chat",
  "InviteFailed": "Failed to invite {0} to the chat. Is he already present?"
}
```

## Frequently Asked Questions

**Question:** How do I change the color of the messages?
**Answer:** Change the lang file and edit the line with ["ChatFormat"] An example is [AdminChat] <color=red>{0}</color>: {1} - That will change the senders name.
