## **Open Route Service**

### **Descrição**

OpenRouteService (ORS) é uma plataforma de serviços de roteamento e geolocalização de código aberto. Oferece uma variedade de APIs para funcionalidades de mapeamento, navegação e análise espacial.

### **Funcionalidades** 

- Geração de rotas e direções de um ponto a outro. (Directions)
- Cálculo de áreas de alcance baseadas no tempo ou na distância a partir de um ponto. (Isochrones)
- Cálculo de matrizes de distâncias e tempos entre múltiplos pontos. (Matrix)
- Ajuste de pontos a estradas ou outras características geográficas.(Snap)
- Otimização de rotas para múltiplos pontos. (Optimization)
- Busca de pontos de interesse (POIs), como restaurantes, lojas...

São funcionalidades voltadas para dados em si, para exibir um mapa dinamico é preciso uma integração com outros servicos. 

### **Custos**

Possui um sistema de planos, onde todos são todos gratuitos, porém possuem alguns limites de uso.

- Standart: Para qualquer pessoa.

| Serviço                  | Limite Diário | Limite por Minuto |
|--------------------------|---------------|--------------------|
| Directions*              | 2.000         | 40                 |
| Isochrones*              | 500           | 20                 |
| Matrix*                  | 500           | 40                 |
| Snap*                    | 2.000         | 100                |
| Optimization*            | 500           | 40                 |
| Elevation points         | 2.000         | 100                |
| Elevation linestrings*   | 200           | 40                 |
| Geocoding                | 1.000         | 100                |
| Reverse geocoding        | 1.000         | 100                |
| Geocoding auto completion| 1.000         | 100                |
| Points of interest*      | 500           | 60                 |


Colaborativo: Para organização humanitária, acadêmica, governamental ou sem fins lucrativos.

| Serviço                  | Limite Diário | Limite por Minuto |
|--------------------------|---------------|--------------------|
| Directions*              | 10.000        | 60                 |
| Isochrones*              | 2.500         | 40                 |
| Matrix*                  | 2.500         | 60                 |
| Snap*                    | 10.000        | 150                |
| Optimization*            | 2.500         | 60                 |
| Elevation points         | 10.000        | 150                |
| Elevation linestrings*   | 1.000         | 60                 |
| Geocoding                | 5.000         | 150                |
| Reverse geocoding        | 5.000         | 150                |
| Geocoding auto completion| 5.000         | 150                |
| Points of interest*      | 2.500         | 90                 |

**Observação:** Uso comercial não permitido.


On-Premise: Instalação local dos serviços principais do openrouteservice em sua própria infraestrutura. As restrições de back-end da API não se aplicam e podem ser configuradas de acordo com suas necessidades (a depender da estrutura). Conta com os servicos Directions, Isochrones, Matrix e Snap.

### Observação

Cada serviço conta com restrições especificas na hora de utilizar, como por exemplo, quanto ao perfil, onde há uma restricao para o perfil de transporte "cadeirante" de 300 km, Podem ser visualizados através do [**Link**](https://openrouteservice.org/restrictions/)


### **Referências**

- https://openrouteservice.org
- https://github.com/vitordarcidasilva/api_openrouteservice