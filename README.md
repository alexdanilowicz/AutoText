# ![Logo](img/autotextlogo.png) AutoText


# Setup

### Install:


```
node
```
```
yarn
```

### Dependencies:

To install dependencies run:
```
$ yarn
```

Or manually add them:

```
$ yarn add vcard-json
$ yarn add shelljs
$ yarn add prompt-confirm
$ yarn
```


Make sure you also have `node` to run javascript in the commandline.


## Getting Contacts File:


1) Go to your contacts app, and select the contacts you want to send your message to.

2) You can skip ordering and select multiple with the "command" key

3) Then, select File > Export vCard, and save it to the same directory with the autotext script (.sh) and sendMessage js with it.

Now, once you have your contacts.vcf in your working directory, run:

```
$ node sendMessage.js
```

You'll have a chance to see the message and confirm before sending in the command line.

Then, you'll see your messages sent on iMessage!

## Example:

```
$ node sendMessage.js
You're going to send the text:

yooooooooo UNIQUE_CONTACT. How's your summer?

<<<<-- where UNIQUE_CONTACT is replaced by their name --->>>>

To:
Alex
isabel


? Are you sure you wish to proceed? (Y/n)
```

## Craft your Message:

Currently, the message is just hardcoded into the .js file as `MESSAGE`. You can edit it directly. It will replace `UNIQUE_CONTACT` with the contact's first word in their name.

## Troubleshooting:

- ensure iMessage is open

## Acknowledgements:

Awesome vcf reader by Andrew Pace:
https://github.com/andrewppace/vcard-json
