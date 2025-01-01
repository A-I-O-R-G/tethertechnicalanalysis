# 📝 Documentação do Projeto: Análise Técnica da Stablecoin Tether (USDT)

## 📖 Introdução
Este projeto visa a criação de um script para realizar a análise técnica da stablecoin Tether (USDT). O objetivo principal é coletar, analisar e visualizar dados de preços históricos em relação a outras criptomoedas e moedas fiduciárias, permitindo insights valiosos para traders e investidores.

### Funcionalidades-chave:
- Coleta de dados históricos de preços e volume de negociação da Tether.
- Cálculo de indicadores técnicos como médias móveis, bandas de Bollinger e RSI.
- Visualização interativa dos dados através de gráficos.

---

## ⚙️ Instalação

### Requisitos do Sistema:
- Python 3.x.
- Bibliotecas necessárias: 
  - `requests`
  - `pandas`
  - `numpy`
  - `plotly`
  
### Dependências Necessárias:
```bash
pip install requests pandas numpy plotly
```

### Guia Passo-a-Passo:
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu_usuario/analisetecnicatetherusdt.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd analisetecnicatetherusdt
   ```
3. Instale as dependências conforme indicado acima.

### Configuração Inicial:
- Nenhuma configuração adicional é necessária para iniciar o projeto.

---

## 🔍 Uso

### Exemplos Práticos:
Execute o script principal para coletar dados e gerar gráficos:
```bash
python main.py
```

### Comandos Principais:
- **`coletar_dados_historicos(symbol, interval='1d', limit=100)`**: Coleta dados históricos da Tether usando a API da Binance.
- **`media_movel(df, period)`**: Calcula a média móvel dos preços.
- **`calcular_rsi(df, period=14)`**: Calcula o Índice de Força Relativa (RSI).
- **`plotar_graficos(df)`**: Gera gráficos interativos.

### Configurações Disponíveis:
- `symbol`: Par de negociação (ex: 'USDTBUSD').
- `interval`: Intervalo para a coleta de dados (opcional, padrão é '1d').

### Casos de Uso Comuns:
- Análise diária de preços.
- Identificação de padrões de comportamento da Tether em relação a outras criptomoedas.

---

## 📁 Estrutura do Projeto
```
analisetecnicatetherusdt/
├── main.py             # Script principal para análise técnica
├── requirements.txt    # Dependências do projeto
└── README.md           # Documentação deste projeto
```

---

## 🌐 API

### Endpoints Disponíveis:
- `GET https://api.binance.com/api/v3/klines`: Coleta dados de preços históricos para a Tether.

### Métodos e Parâmetros:
- **Método**: `GET`
- **Parâmetros**:
  - `symbol`: O par de negociação, ex: 'USDTBUSD'.
  - `interval`: O intervalo para as velas, ex: '1d'.
  - `limit`: Limite de dados a serem coletados.

### Exemplos de Requisições:
```python
coletar_dados_historicos('USDTBUSD')
```

### Respostas Esperadas:
```json
[
    ["open_time", "open", "high", "low", "close", "volume", ...]
]
```

---

## 🤝 Contribuição

### Guia para Contribuidores:
1. Crie um fork do repositório.
2. Crie sua branch:
   ```bash
   git checkout -b feature/nome-da-sua-feature
   ```
3. Faça suas alterações e commit:
   ```bash
   git commit -m 'Adiciona nova funcionalidade'
   ```
4. Envie para o repositório remoto:
   ```bash
   git push origin feature/nome-da-sua-feature
   ```

### Padrões de Código:
- Utilize PEP 8 para a formatação Python.

### Processo de Pull Request:
- Abra um pull request na interface do GitHub descrevendo suas alterações.

### Boas Práticas:
- Documente suas funções e métodos.
- Teste suas alterações antes de enviar.

---

## 📜 Licença

### Tipo de Licença:
Este projeto está sob a Licença MIT.

### Termos de Uso:
Liberdade para uso, cópia, modificação e distribuição do software.

### Restrições:
Inclua o aviso de licença em qualquer distribuição do software.

---

## 🛠️ Manutenção Contínua
Estamos comprometidos com atualizações regulares e melhorias contínuas no script, visando sempre a precisão e a eficiência do código.

---

## 🔄 Atualizações Recentes
### Status do Desenvolvimento:
O projeto foi melhorado recentemente, incorporando as seguintes mudanças:
- Refatoração das funções para melhorar a modularidade e legibilidade.
- Adição de tratamento de erros para a requisição da API.
- Inclusão de tipagem nas funções para maior clareza.
- Melhoria na documentação do código.

### Observações:
O código agora lida melhor com erros e apresenta uma estrutura mais organizada, facilitando a manutenção e futuras expansões.

---

Esta documentação foi estruturada para fornecer informações claras e completas sobre a implementação e uso do software. Se houver mais detalhes que você gostaria de incluir ou ajustar, não hesite em avisar!