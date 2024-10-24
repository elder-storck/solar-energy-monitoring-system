# solar-energy-monitoring-system

# Métricas importantes
Para um sistema de monitoramento de um sistema fotovoltaico, algumas métricas importantes a serem monitoradas incluem:

1. **Produção de Energia**:
   - Energia gerada (kWh) em tempo real e acumulada.
   - Comparação com a produção esperada.
<!--
2. **Desempenho do Sistema**:
   - Coeficiente de Performance (CP) ou Performance Ratio (PR).
   - Eficiência dos painéis solares.
-->
3. **Irradiação Solar**:
   - Níveis de irradiação solar (W/m²) em tempo real.
   - Dados históricos de irradiação.

4. **Temperatura dos Painéis**:
   - Temperatura ambiente e temperatura dos módulos.
   - Impacto da temperatura na eficiência.

5. **Consumo de Energia**:
   - Consumo em tempo real e histórico da estação.
   - Comparação entre produção e consumo.

6. **Status do Sistema**:
   - Monitoramento de falhas e manutenção.

7. **Baterias (se aplicável)**:
   - Nível de carga e descarga das baterias.
   - Ciclos de vida e estado de saúde das baterias.

8. **Dados Climáticos**:
   - Umidade, vento e outras condições climáticas que podem afetar a produção.

9. **Alertas e Notificações**:
   - Alertas sobre falhas, baixa produção ou manutenção necessária.

10. **Análise Financeira**:
    - Economia gerada em relação a custos com energia elétrica.
    - Retorno sobre o investimento (ROI).

Essas métricas permitem um acompanhamento detalhado do desempenho do sistema e ajudam a otimizar a produção de energia.

Aqui estão alguns componentes e etapas a serem consideradas para criar o sistema embarcado e, assim, coletar as métricas necessárias:

# Arquitetura Do Projeto


### 1. **Hardware**:
   - **Microcontroladores**: Utilizar microcontroladores como Arduino, Raspberry Pi ou ESP32 para o processamento de dados.
   - **Sensores**:
     - **Irradiação Solar**: Sensores de luz (como fotocélulas ou sensores de irradiação).
     - **Temperatura**: Termômetros digitais (como DHT11 ou DS18B20).
     - **Energia**: Módulos de medição de energia (como o PZEM-004T) para monitorar a produção e consumo.
   - **Módulos de Comunicação**: Módulos Wi-Fi (como ESP8266 ou ESP32) ou GSM para enviar dados para a nuvem.

### 2. **Software**:
   - **Firmware**: Escrever o firmware para coletar dados dos sensores e processá-los. Pode-se usar Arduino IDE, MicroPython, ou outras linguagens de programação.
   - **Interface de Usuário**: Criar um painel web ou um aplicativo móvel para visualizar os dados coletados.
   - **Banco de Dados**: Usar um banco de dados em nuvem para armazenar os dados históricos (como Firebase, MongoDB ou SQL).

### 3. **Monitoramento e Controle**:
   - **Alertas**: Implementar um sistema de notificação para alertar sobre falhas ou desempenho abaixo do esperado.
   - **Análise de Dados**: Criar algoritmos para analisar a eficiência e gerar relatórios.

### 4. **Integração**:
   - **APIs**: Se necessário, integrar com APIs de serviços meteorológicos para obter dados climáticos adicionais.
   - **Segurança**: Garantir a segurança dos dados transmitidos, usando criptografia e autenticação.

### 5. **Teste e Validação**:
   - Realizar testes para garantir que os dados sejam precisos e o sistema funcione como esperado.

# Etapas do Desenvolvimento

Seguem os passos necessários para o desenvolvimento do sistema de monitoramento de sistema fotovoltaico:

### 1. **Definição do Escopo**

   - **Objetivos**: Definir o que será monitorado (ex: produção de energia, temperatura, etc.).
   - **Requisitos**: Listar as métricas e funcionalidades necessárias.

### 2. **Pesquisa e Planejamento**
   - **Componentes**: Pesquisar e selecionar os sensores e microcontroladores adequados.
   - **Arquitetura do Sistema**: Definir como o sistema será estruturado (hardware e software).

### 3. **Simulação do Hardware**
   - Criar e simular um protótipo do hardware, (ex: Tinkercad)

### 4. **Desenvolvimento do Hardware**
   - **Montagem**: Montar o circuito com os sensores e o microcontrolador.
   - **Testes Iniciais**: Verificar se todos os componentes estão funcionando corretamente.

### 5. **Desenvolvimento do Software**
   - **Firmware**:
     - Escrever o código para o microcontrolador, incluindo a leitura dos sensores e a transmissão dos dados.
   - **Interface de Usuário**:
     - Criar uma interface (web ou app) para visualização dos dados.
   - **Banco de Dados**:
     - Configurar um banco de dados para armazenar os dados coletados.

### 6. **Integração de Sistemas**
   - **Conexão**: Integrar a comunicação entre o microcontrolador e o banco de dados/servidor.
   - **APIs**: Se necessário, integrar serviços externos para dados adicionais (ex: clima).

### 7. **Teste e Validação**
   - **Testes Funcionais**: Testar cada parte do sistema individualmente e em conjunto.
   - **Validação dos Dados**: Comparar os dados coletados com medições conhecidas.

### 8. **Aprimoramento**
   - **Análise de Resultados**: Avaliar os dados coletados e ajustar o sistema conforme necessário.
   - **Feedback**: Se possível, obter feedback de usuários sobre a interface e a funcionalidade.

### 9. **Documentação**
   - **Documente o Projeto**: Criar documentação detalhada sobre o funcionamento do sistema, instalação e manutenção.

### 10. **Implementação e Monitoramento**
   - **Instalação**: Instalar o sistema no local desejado.
   - **Monitoramento Contínuo**: Acompanhar o desempenho do sistema e fazer ajustes conforme necessário.

### 11. **Manutenção e Atualização**
   - **Manutenção Regular**: Verificar periodicamente os componentes e atualizar o software conforme necessário.
   - **Novas Funcionalidades**: Considerar implementar novas métricas ou funcionalidades com base em feedback ou novas tecnologias.

# Pesquisas 
Termo de Pesquisa no google acadêmico: "solar energy monitoring system"


[IoT based solar energy monitoring system](https://ieeexplore.ieee.org/abstract/document/8389711)

[IoT based solar energy monitoring system](https://www.sciencedirect.com/science/article/abs/pii/S2214785321052238)

[Solar Energy Monitoring System Using IoT](https://d1wqtxts1xzle7.cloudfront.net/94575875/1455558654Chapter_26-libre.pdf?1668993163=&response-content-disposition=inline%3B+filename%3DSOLAR_ENERGY_MONITORING_SYSTEM_USING_IoT.pdf&Expires=1729554117&Signature=RWhBJtFoOgZUTgfHLVsy33lFEOVzyuF6GguSKQc6bVGpNcV~ioPATKeMIwDnbuSJO9nWOdS8CN9o9L4~MoEzM9VHqLfYGLWKnlPf9eHhapYX~AmWCE~ZWDADuWKj5P0OemEQlmswijjHQbrkR~Pqqf6Z-WronlZCT0OvPR7bY4-Y8JtMhFo~z0zsDqmLxt8giia8Yg58~37EJomseu6QFMWhDm93J~9KiFpcaAJHixlzkzTq323NWAkSTaFz9Xf3qKZiYg0vXw5zs-5iQrqvqn9X1ykivvLnl26kg6OQbeOHN3jAiJAX3tOq9XveV52FqekiCAZan2ervss0dwYXew__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)

[Communication Architecture of Solar Energy Monitoring Systems for Telecommunication Objects](https://ieeexplore.ieee.org/abstract/document/9670354)
