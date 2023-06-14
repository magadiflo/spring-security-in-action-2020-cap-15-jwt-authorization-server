# Servidor de autorización usando JWT

## Para el capítulo 15, sección "implementación de un servidor de autorización para emitir JWT"

## Ejemplo del uso de este servidor

````bash
curl -v -X POST -u client:secret -d "grant_type=password&username=admin&password=12345&scope=read" http://localhost:8080/oauth/token

--- Response ---
< HTTP/1.1 200
<
{ 
  "access_token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2ODY4MDc0NTgsInVzZXJfbmFtZSI6ImFkbWluIiwiYXV0aG9yaXRpZXMiOlsicmVhZCJdLCJqdGkiOiI3ODYyNGZjZi0yYzVmLTQ5MjgtYTYwOC1mM2I3ZjE3ZThlMDUiLCJjbGllbnRfaWQiOiJjbGllbnQiLCJzY29wZSI6WyJyZWFkIl19.XV9Y9akTKrdV5S3g94Eyqh-xVBjxAucVzaFka78qnrI",
  "token_type":"bearer",
  "refresh_token":"eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX25hbWUiOiJhZG1pbiIsInNjb3BlIjpbInJlYWQiXSwiYXRpIjoiNzg2MjRmY2YtMmM1Zi00OTI4LWE2MDgtZjNiN2YxN2U4ZTA1IiwiZXhwIjoxNjg5MzU2MjU4LCJhdXRob3JpdGllcyI6WyJyZWFkIl0sImp0aSI6IjgyMTA4YTFhLTY1OTktNGExMC05ZjE4LTdkMTI0YTE0YWUyOSIsImNsaWVudF9pZCI6ImNsaWVudCJ9.LIMk7NaLcRVfaw9W1y80MYx6m80FHbf8fUm_969r2i4",
  "expires_in":43199,
  "scope":"read",
  "jti":"78624fcf-2c5f-4928-a608-f3b7f17e8e05"
}
````
