## Cenário 02: Acesso e visualização do Dashboard.

### Caso de Teste 01: Acesso ao Dashboard após login bem-sucedido.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C02-CT01 | Verificar a exibição correta do Dashboard após login com sucesso. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar autenticado com credenciais válidas.     |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema com sucesso              |
| **QUANDO** for redirecionado automaticamente após o login         |
| **ENTÃO** a tela do Dashboard deve ser exibida com os atalhos e widgets principais |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir corretamente a interface do Dashboard.     |

https://jam.dev/c/e7006ee9-17bf-4b76-96b3-30d797227351

---

### Caso de Teste 02: Verificação da exibição dos widgets do Dashboard.

| ID       | Descrição                                                 |
| :------- | :-------------------------------------------------------- |
| C02-CT02 | Os widgets padrão devem ser exibidos corretamente no Dashboard. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar na tela do Dashboard após login.         |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário está autenticado                          |
| **E** está visualizando o Dashboard                              |
| **QUANDO** a página for carregada                                |
| **ENTÃO** widgets como \"Time at Work\" e \"My Actions\" devem ser exibidos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Todos os widgets principais devem ser visíveis e funcionais.     |

https://jam.dev/c/3be85f48-5cde-40ac-87e0-d3d1889e763d

---  

### Caso de Teste 03: Acesso ao Dashboard com sessão expirada.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C02-CT03 | O sistema deve redirecionar o usuário para o login se a sessão estiver expirada. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário estava logado, mas a sessão expirou.                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema anteriormente            |
| **E** permaneceu inativo por um longo período                    |
| **QUANDO** tentar acessar o Dashboard novamente                  |
| **ENTÃO** o sistema deve redirecioná-lo para a página de login    |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A sessão expirada deve ser tratada corretamente com redirecionamento. |

https://jam.dev/c/3ecf9910-4689-4333-82e4-0fc426db28c9

Tive que limpar o cookies para forçar a sessão expirada.