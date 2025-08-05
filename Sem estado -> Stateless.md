Significa que **cada solicitação (requisição) do cliente para o servidor deve conter toda a informação necessária para que o servidor entenda e processe essa solicitação.**

O servidor não deve armazenar _nenhum_ contexto de sessão sobre o cliente entre as requisições. Cada requisição é independente das anteriores.

Exemplo: 

Se um cliente precisa de autenticação, o token de autenticação deve ser enviado em _cada_ requisição. O servidor não "se lembra" de que o cliente já se autenticou em uma requisição anterior.