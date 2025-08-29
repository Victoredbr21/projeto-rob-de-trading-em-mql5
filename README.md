# Robo de Trading – Versão Open Source (Demonstração)

⚠️ **Aviso importante:** Esta versão do código **não deve ser usada para operar no mercado real**.  
O objetivo deste repositório é **mostrar a evolução do projeto e habilidades em MQL5**, apenas para portfólio e aprendizado.

Atualização: Eu coloquei uma trava nos indicadores que disponibilizei no iCustom para funcionar apenas em conta demonstrativas, ou seja, o robô não vai funcionar em conta real.

---

## Sobre o projeto

Este é um projeto de um **robô de trading** criado para fins de estudo e demonstração.  
A versão open source contém **uma lógica de trading propositalmente simplificada e aleatória**, sem uso de indicadores avançados como delta, ATR ou rastreio de Wyckoff.  

O código completo da versão privada possui lógica avançada, incluindo:

- Rastreio de Wyckoff e absorção
- Detecção de tendência usando delta e volatilidade
- Operações baseadas em fluxo de ordens
- Stop, Take Profit e gerenciamento de risco

⚠️ A versão open source **não utiliza nenhuma dessas funcionalidades avançadas**. É apenas um esqueleto para estudo e portfólio.

---

## Commits Principais

- Criação das funções básicas do robô (`OnInit`, `OnDeInit`, `OnTick`)
- a função OnInit inicia o robô, a OnDeInit desliga e a OnTick calcula
- Inicialização de handles para indicadores (CVD, ATR, VWMA e Volume)
- Ajustes de parâmetros de entrada (contratos, stop loss, take profit, horários)
- Testes e criação de buffers e arrays dinâmicas do MQL5
- Implementação de lógica aleatória de trading apenas para demonstração
- Tratamento de erros com `GetLastError` e booleanas de verificação
- Uso de enumeradores para simplificar sinais no código
- Desalocação de buffers com `ArrayFree` e funções de shutdown na função 'OnDeInit'
- Observações gerais sobre a IDE MetaEditor e como o código é recompilado

> Nota: O código pode estar incompleto, possivelmente com erros de compilação e redundâncias.  
> O foco deste repositório **não é operar**, e sim **mostrar a estrutura do projeto e as habilidades em programação MQL5**.

---

## Estrutura do Código

- `OnInit()`: Inicializa o robô, handles e buffers
- `OnDeInit()`: Desliga o robô e limpa buffers
- `OnTick()`: Implementa a lógica de trading (simplificada nesta versão)
- Buffers e handles para indicadores: CVD, ATR, Média Móvel Ponderada pelo Volume e Volume Nativo

---

## Como usar

1. Clone este repositório para estudo e análise.
2. Abra o arquivo `.mq5` no MetaEditor.
3. **Não use para trading real**.
4. Explore a estrutura do código, a inicialização de handles, buffers e parâmetros de entrada.

---

## Licença

Este código é **open source**, mas **não possui licença de uso financeiro real**.  
É destinado apenas a **estudo, aprendizado e portfólio**.

---

## Conclusão

Esta versão é uma demonstração do projeto.  
A versão completa contém toda a lógica avançada de trading, mas não está disponível publicamente por questões de segurança e integridade financeira.

> Lembre-se: **não coloque dinheiro real neste código!** É apenas para aprendizado, você foi avisado.

