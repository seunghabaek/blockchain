# Typescript를 사용하는 과정에서의 Tip

### ts-node를 설치하는 이유

ts-node를 설치하게 되면, 빌드없이 typescript 사용 가능.
production을 위한 건 아니고, staging 환경에서만 사용.

### nodemon

nodemon을 설치하게 되면 서버를 다시 refresh할 필요가 없다.

### 모듈 import 시 has no default export 해결방법

1. import \* as crypto from "crypto"
2. tsconfig.json에 "esModuleInterop":true 옵션 추가

### js로 구성된 모듈을 typescript에서 읽지 못할때

npm -i -D @types/{module name} 을 해서 typescript가 javascript로 이뤄진 모듈의 type을 읽을 수 있도록 해준다.
https://github.com/DefinitelyTyped/DefinitelyTyped 이 레포에서 typescript의 모든 type들이 추가되고 있다.
