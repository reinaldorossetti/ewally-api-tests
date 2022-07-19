# ewally-api-tests
Testes de API com Postman e Newman.

Postman is an API platform for testing and building and using APIs. Postman simplifies each step of the API lifecycle and streamlines collaboration so you can create better APIs—faster.


Pré-requisitos:
- node-js 12+
- Libs newmam e newman-reporter-htmlextra:
    - run: npm install -g newman
    - run: npm install -g newman-reporter-htmlextra

Reporte:
```
https://reinaldorossetti.github.io/ewally-api-tests/index.html
```

Comando para rodar via newman:
```
newman run collections/ewally.postman_collection.json -e collections/ewally.postman_environment.json -r htmlextra --reporter-htmlextra-title "Ewally - API AUTOMATION" --reporter-htmlextra-export testResults/index.html \
                --timeout-request 45000 --delay-request 600 --suppress-exit-code
```
