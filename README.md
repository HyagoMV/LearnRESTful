# LearnRESTful


# Método: PUT - RFC 2616
- Método Idempotente
 - Operação que produzirá os mesmos resultados se executada repetidas vezes
 - A entra, A sai
- Inclui todos as propriedades existentes no recurso armazenado no servidor e
- Pode incluir novas propriedades que devem ser acrescentada ao recurso armazenado no servidor
- Solicita que o recurso seja armazenada
  - Se o recurso já existir, então DEVE-SE substitui-la e retorna o código 200 (OK)
  - Se o recurso não existir e é possível criar um novo recurso DEVE-SE retorna código 201 (Created) ou 204 (No Content)
  - Se o recurso não existir e não é possível criar um novo recurso OU o recurso não  puder ser modificado um código de erro apropiado DEVE SER retornado

# Método: PATCH
- Método Idempotente e Não Idempotente
- Inclui somente as propriedades que devem ser modificadas no recurso armazenado no servidor
