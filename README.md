# Bootcamp GoStack - RocketSeat

RocketSeat bootcamp, an educational startup that teaches basic and advanced topics in software development trough Javascript stack: Node.js, React.JS and React Native.

## Challenge 04

Basic React Native concepts, using TDD to develop a GitHub repositories simple app, to list, and like Git repositories, integrated with the api from [Challenge 02](thub.com/dhaubert/rocketseat-gostack-desafio02)

### Config API
Change baseURL of the running API on `services/api.js`. Default address is localhost on port 3333.

For different environments:
- ios with emulator: localhost
- ios or android with physical device: IP address when backend and device is in the same network. Run `ipconfig` on windows and `ifconfig` on linux to check what is your IP on LAN.
- Android with Emulador (android, option1): [localhost](http://localhost) (run the command `adb reverse tpc:3333 tcp:3333`.
- Android with Emulador (android, option2): specific IP address of the machine running the emulator is 10.0.2.2.
- Android with Emulador (genymotion): specific IP address of the machine running the emulator is 10.0.3.2.

```javascript
import axios from "axios";

const api = axios.create({
  baseURL: "http://localhost:3333",
});

export default api;
```

### Dependencies
Run inside the project directory to install all the dependencies.
```bash
yarn
```

### Development
Run inside the project directory. Make sure you have port 3333 available. 
```bash
yarn start
```

To install the app and open the emulator
```
yarn android
```

To debug console logs, press `ctrl+m` on android emulator and select the option `debug`. It will open a browser tab, and all console logs will be displayed on the browser console, pressing `F12` on chrome and firefox.

### Tests
Run inside the project directory. 1 tests, 1 suites. Implemented on Jest.
```bash
yarn test
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
