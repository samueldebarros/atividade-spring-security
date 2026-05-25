# atividade-spring-security

Parte 1 - Conceitos: Spring Security
1. Explique com suas palavras o que é Spring Security.
   
R: ele é um framework focado em fornecer autenticação (verificar quem é o usuário) e autorização (verificar o que o usuário pode fazer) para aplicações java.

2. Para que serve o método csrf().disable()?
R: Ele serve para desabilitar a proteção contra ataques do tipo CSRF

3. Explique o que significa SessionCreationPolicy.STATELESS.
R: essa configuração diz ao Spring Security para não criar e nem utilizar sessões HTTP no servidor para armazenar o estado do usuário. Isso significa que a aplicação não vai guardar "memória" de quem está logado. 

4. Qual a função do permitAll()?
R: A função do permitAll() é liberar o acesso público a determinados endpoints.

5. Explique o que faz o requestMatchers().
R: o requestMatchers() serve para mapear e selecionar quais rotas ou URLs específicas aplicar uma determinada regra de segurança.

6. Qual a função do anyRequest().authenticated()?
R: essa instrução define uma regra de segurança para o restante da aplicação. Ela diz que qualquer outra requisição deve ser obrigatoriamente autenticada.

7. O que é uma API Stateless?
R: uma API Stateless é aquela que não armazena nenhuma informação sobre as sessões dos clientes no servidor, fazendo com q cada requisição feita pelo cliente para o servidor seja isolada

9. Explique o que a lambda abaixo faz:
session -> session.sessionCreationPolicy(SessionCreationPolicy.STATELESS)

Essa expressão lambda configura o gerenciamento de sessões do Spring Security utilizando a sintaxe atual do Spring Boot
