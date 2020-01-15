# babel-plugin-demand-loading

![version](https://img.shields.io/badge/version-v1.0.0-brightgreen.svg?style=flat-square) [![MIT](https://img.shields.io/dub/l/vibe-d.svg?style=flat-square)](http://opensource.org/licenses/MIT) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://reactjs.org/docs/how-to-contribute.html#your-first-pull-request)

---

### 下载支持
支持babel6、babel7

#### babel6 1.x.x
```
npm install babel-plugin-demand-loading@1 --save-dev
```

#### babel7 2.x.x
```
npm install babel-plugin-demand-loading@2 --save-dev
```
### 使用说明
```
// e.g.
// .babelrc
"plugins": [
    [
      "babel-plugin-demand-loading",
      {
        "library": "yournpm"
      },
      "syntax-decorators"
    ],
  ]
  
// index.js
import { helloworld } from 'yournpm';

      ↓ ↓ ↓ ↓ ↓ ↓

var _helloworld = require('yournpm/helloworld');
import {fromat} from 'yournpm';
```


