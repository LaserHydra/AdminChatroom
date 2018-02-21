**Admin Chatroom** allows admins to talk privately with each other in-game.

## Permissions

- **adminchatroom.allowed** -- Allows player to slap other players

## Commands

- **a msg** -- Send a message to the chatroom
- **a `<invite/kick> <playerid/playername>`** -- Kick or Invite a player to the room

## Configuration

```json
{
  "General": {
    "Allowed To Join Permission": "AdminChatroom.allowed"
  }
}
```
## Localization

The default messages are in the `AdminChatroom.json` file under the `oxide/lang/en` directory. To add support for another language, create a new language folder (ex. de for German) if not already created, copy the default language file to the new folder, and then customize the messages.

## Frequently Asked Questions

**Question:** How do I change the color of the messages?

**Answer:** Change the lang file and edit the line with ["ChatFormat"] An example is [AdminChat] <color=red>{0}</color>: {1} - That will change the senders name.
