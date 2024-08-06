## Tom Tom

### **Custos**

Os custos deste SaaS serão atualizados em 12 de agosto de 2024.

O serviço oferece dois formatos de preço: Map Display non-tile e Map Display tiles.

Tiles: São pequenos blocos ou partes do mapa, geralmente no formato de imagem, que são carregados e montados no cliente (navegador ou aplicativo) para formar um mapa completo.

Non-tile: Refere-se à entrega do mapa como um único bloco ou uma área grande de uma vez, em vez de ser dividido em pequenas partes.

O modelo **Freemium** oferece:

50.000 requisições de tiles por dia.
2.500 requisições non-tile por dia.


Custo do modelo **Pay-as-you-grow** por 1000 requisições, com os preços atualizados:

| Serviço              | Preço Atual | Novo Preço |
|----------------------|-------------|------------|
| Map Display non-tile | €0.50       | €0.75      |
| Map Display tiles    | €0.05       | €0.08      |

O uso nesse tipo de modelo é pré-pago, onde o serviço se torna ininterrupto para os creditos já pagos. Esses créditos devem ser utilizados no periodo de um ano, além disso podem ser pagamentos unicos ou recorrentes.

Para o **Modelo enterprise** é preciso contactar a equipe do TomTom para saber os preços.

### **Integração com flutter**

Implementação no flutter por mais que não possua documentação especifica para ela, parece ser tranquila. 

Por meio desse [**Link**](https://medium.com/tomtom-developers/displaying-tomtom-maps-with-flutter-33c0e876e84e) podemos visualizar um pequeno exemplo de como utilizar os Servicos do TomTom para o flutter.

### **Confiabilidade**

Sobre os termos de SLA (Acordo de Nível de Serviço) e SLO (Objetivos de Nível de Serviço), não há informações específicas disponíveis.

No entanto, a plataforma oferece um Customer Portal onde você pode:

- Acompanhar incidentes com o serviço.
- Verificar manutenções planejadas em andamento e futuras.
- Conversar diretamente com o suporte de TI.

### **Limite de Uso**

Para manter a integridade das APIs de Mapas, a TomTom aplicará um limite de QPS (consultas por segundo) ao seu uso dessas APIs, nos planos **Freemium** e **Pay-as-you-grow**.

Para flexibilizar o limite de QPS, é necessário migrar para o plano **Enterprise**.