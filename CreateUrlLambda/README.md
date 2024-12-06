# URL - Lambda

Serviço que realiza o encurtamento da URL.
O aplicação utiliza as funções lambda da AWS.

Para execução basta realizar uma requisição:
```bash
curl --request POST \
  --url https://rjnuvjwhcxul3q2oul24sk2iqe0lxnxw.lambda-url.us-east-2.on.aws/ \
  --header 'Content-Type: application/json' \
  --header 'User-Agent: insomnia/10.0.0' \
  --data '{
	"originalUrl": "https://youtu.be/ffrtx2nT7s4",
	"expirationTime": "1728529200000"
}'
```