### HarunaRequest

Example Usage
```js
const HarunaRequest = require("./HarunaRequest.js");
const wrapper = new HarunaRequest("localhost:1024", "my_secret_password");
wrapper.getVote("510810429828890624")
    .then(data => {
        if (!data.user) {
            console.log("User not voted.");
        } else {
            console.log('User voted', data);
        }
    });
```