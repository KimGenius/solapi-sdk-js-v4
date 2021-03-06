# CoolSMS SDK for Javascript
You can send text messages, Kakaotalk in Korea using this package.

## Installing
To use the SDK, simply use npm package manager CLI. Type the following into a terminal window.

```bash
npm install coolsms-sdk-v4
```

## Usage

```javascript
const { config, Group } = require('coolsms-sdk-v4')
config.init({
  apiKey: 'ENTER API_KEY',
  apiSecret: 'ENTER API_SECRET'
})
send({
  text: 'Hello CoolSMS',
  to: 'Receiver Number',
  from: 'Sender Number'
})
async function send (message, agent = {}) {
  console.log(await Group.sendSimpleMessage(message, agent))
}
```

## Examples

[Group Message](https://github.com/coolsms/coolsms-sdk-js-v4/blob/develop/example/groupMessage.js), 
[Simple Message](https://github.com/coolsms/coolsms-sdk-js-v4/blob/develop/example/simpleMessage.js),
[Scheduled Messages](https://github.com/coolsms/coolsms-sdk-js-v4/blob/develop/example/scheduleMesssage.js),

[more examples can be found at coolsms-v4-examples](https://github.com/coolsms/coolsms-v4-examples)
## Opening Issues

If you encounter a bug with the COOLSMS SDK for Javascript we would like to hear about it. Search the [existing issues](https://github.com/coolsms/coolsms-sdk-js-v4/issues) and try to make sure your problem doesn’t already exist before opening a new issue. It’s helpful if you include the version of the SDK, Node.js or browser environment and OS you’re using. Please include a stack trace and reduced repro case when appropriate, too.

## License

Licensed under the MIT License.
