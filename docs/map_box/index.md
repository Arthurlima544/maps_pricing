
## **MapBox Maps**

### **Desempenho**

Para a análise de desempenho, tem alguns recursos voltados para desenvolvedores que rodam projetos em modo Debug e Profile, permitindo testes focados em gargalos na renderização de mapas.

Podemos ver os aspectos de desempenho que podem ser visualizados em modo debug através do [**Link**](https://docs.mapbox.com/android/maps/guides/debugging-and-profiling/performance-stats/)

Assim como os serviços do Google, possui um sistema de logs de eventos, registrando consumos na API e dados por data.

### **Confiabilidade**

Nos termos do SLA, se o cliente tiver um pedido ativo e as APIs do Mapbox cobertas e usadas de acordo com esse pedido não estiverem disponíveis 99,9% do tempo durante o mês, o cliente será elegível para receber um Crédito de Serviço. Para isso, é preciso solicitar o crédito pelo e-mail: [**info@mapbox.com**.](mailto:info@mapbox.com)


### **Documentacao e Suporte**

A documentação deixa a desejar, com falta de organização entre os assuntos. Não possui uma página específica para a configuração no Flutter.

Sobre o suporte, dependendo do plano, o Mapbox fornece serviços adicionais:

- Plano Individual: suporte por e-mail, tempo de resposta de 3 dias úteis.
- Plano Negócios: suporte por e-mail, tempo de resposta de 4 horas a 1 dia útil (dependendo da prioridade).
- Plano Premium: suporte por e-mail, tempo de resposta de 30 minutos, engenheiro de suporte dedicado, orientação de soluções, avaliação guiada para nova solução, acesso a recursos beta do Mapbox.

Para cada nível de problema, os planos possuem diferentes períodos de resposta. Por exemplo, problemas mais críticos são respondidos rapidamente (30 minutos) se forem críticos e se o cliente estiver com o plano Premium, como no caso de um defeito de serviço que cause uma interrupção de um aplicativo.

### **Portabilidade**

Os recursos são disponibilizados para diversas plataformas.

### **Recursos**

- Mapas personalizáveis.
- Navegação e roteamento.
- Mapas offline.
- Geocodificação.

### **Seguranca**

A Mapbox utiliza sistemas de APIKEY para lidar com o consumo. Podemos restringir a chave para o consumo com restrições de URL.

### **Feedbacks**

- Apps como Strava, BMW, Toyota, CNN, IBM, entre outros, utilizam recursos do Mapbox.

### **Escalabilidade**

???

### **Limite de uso**

O uso da API de Imagens Estáticas e da API de Telhas Estáticas é limitado com um limite de taxa padrão de 1.200 solicitações por minuto e 5.000 solicitações por minuto, respectivamente. Exceder esses limites resultará em uma resposta HTTP 429.

### **Preço**

Ao criar uma conta, já é necessário associar a um cartão de crédito.

Para a Maps SDK, temos o custo de 25.000 usuários ativos por mês gratuitamente.

| Requisições         | Preço por 1.000 requisições          |
|---------------------|--------------------------------------|
| 25.001 – 125.000    | $4.00                                |
| 125.001 – 250.000   | $3.20                                |
| 250.001+            | $2.40                                |
| 1.250.000+          | Acordo com a equipe de vendas do Mapbox |



## **MapBox Static Images**

### **Preço**

Para a Maps Static Images, temos o custo de 50.000 requisições iniciais gratuitamente.

| Requisições         | Preço por 1.000 requisições          |
|---------------------|--------------------------------------|
| 50.001 - 500.000    | $1.00                                |
| 500.001 - 1.000.000 | $0.80                                |
| 1.000.001+          | $0.60                                |
| 5.000.000+          | Acordo com a equipe de vendas do Mapbox |

### **Integracao com o Flutter**

Por ser basicamente uma imagem, existe uma enorme facilidade para configurar a requisição no Flutter.