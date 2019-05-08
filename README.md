# Twitch Themer

A Visual Studio Code extension that listens to twitch chat and allows viewers to change the streamers VS Code theme by sending **!theme**

| Release | vNext
| -- | --
| [![Build Status](https://dev.azure.com/michaeljolley/vscode-twitch-themer/_apis/build/status/MichaelJolley.vscode-twitch-themer?branchName=master)](https://dev.azure.com/michaeljolley/vscode-twitch-themer/_build/latest?definitionId=1&branchName=master) | [![Build Status](https://dev.azure.com/michaeljolley/vscode-twitch-themer/_apis/build/status/MichaelJolley.vscode-twitch-themer?branchName=vNext)](https://dev.azure.com/michaeljolley/vscode-twitch-themer/_build/latest?definitionId=1&branchName=vNext)



![](./resources/screenshot-example.gif)  

## Twitch Chat Commands

#### Receive a list of available theme names 

This will send a list of installed VS Code themes to the requestor via whisper. 

```
!theme list
```
`Note: Only 1 whisper per user will be sent per day.`

#### Set VS Code theme

This command will set the theme of the streamers' VS Code workspace to the theme specified.

```
!theme {theme name}
```
`Note: The theme must be previously installed and available within VS Code.`

#### Reset VS Code theme

This command will set the theme of the streamers' VS Code workspace back to the theme that was used at the time the extension connected to chat.

```
!theme reset
```
`Note: Everytime the extension disconnects from chat, the theme will be reset.`

---

## How to connect to Twitch

- You can login to the twitch chat client using `Twitch Themer: Sign In` command. Execute the commands from vscode command pallete. This will open the Twitch Authentication page. Login to your twitch account. The token is stored in secure keystorage.

- You can logout from the chat once you are done with your twitch session.
- Connect to the chat client using `Twitch Themer: Chat Connect` command.
- Disconnect from the chat client using `Twitch Themer: Chat Disconnect` commands

---

## Attribution & Credits

* Thanks to [Sivamuthu Kumar](https://github.com/ksivamuthu) for the authentication code that we blatantly plagiarized from his [VSCode Peacock Twitch Extension](https://github.com/ksivamuthu/vscode-peacock-twitch-client).
* Thanks to [Brian Clark](https://github.com/clarkio) for his videos on creating VS Code extensions and his [VSCode Twitch Highlighter](https://github.com/clarkio/vscode-twitch-highlighter) extension that really is what brought about the idea for this extension.

## Release Notes

See [CHANGELOG.md](CHANGELOG.md)
