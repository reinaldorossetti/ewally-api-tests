# ewally-api-tests
Testes de API com Postman e Newman.

Postman is an API platform for testing and building and using APIs. Postman simplifies each step of the API lifecycle and streamlines collaboration so you can create better APIs—faster.


Reporte:
```
https://reinaldorossetti.github.io/ewally-api-tests/index.html
```

Comando para rodar via newman:
```
newman run collections/ewally.postman_collection.json -e collections/ewally.postman_environment.json -r htmlextra --reporter-htmlextra-title "Ewally - API AUTOMATION" --reporter-htmlextra-export testResults/index.html \
                --timeout-request 45000 --delay-request 600 --suppress-exit-code
```
