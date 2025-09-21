# 🏛️ Gerador de Imagens Receita Federal

Serviço Flask para gerar imagens personalizadas do documento da Receita Federal com CPF, nome e vencimento dinâmicos.

## 🚀 Funcionalidades

- ✅ **3 Variáveis**: CPF, Nome e Vencimento
- ✅ **Múltiplos Campos**: Vencimento aparece em 3 lugares
- ✅ **Apenas Variáveis**: Sem texto adicional
- ✅ **Compatível**: Funciona perfeitamente no Typebot

## 📋 Como usar

### URL da API:
```
/api/gerar-imagem?cpf={{cpf}}&nome={{nome}}&vencimento={{vencimento}}
```

### Exemplo:
```
/api/gerar-imagem?cpf=123.456.789-00&nome=João Silva&vencimento=25/12/2024
```

## 🛠️ Instalação Local

1. Clone o repositório
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute o servidor:
   ```bash
   python src/main.py
   ```

## 🚀 Deploy no Railway

1. Conecte seu repositório GitHub ao Railway
2. O deploy será automático usando as configurações em `railway.json`
3. A aplicação estará disponível na URL fornecida pelo Railway

## 📁 Estrutura do Projeto

```
gerador_imagens/
├── src/
│   ├── main.py              # Aplicação Flask principal
│   ├── routes/
│   │   └── image_generator.py  # Rotas da API
│   └── static/
│       └── receita-federal.png # Imagem base
├── requirements.txt         # Dependências Python
├── Procfile                # Configuração para deploy
├── railway.json            # Configuração Railway
└── README.md               # Este arquivo
```

## 🔧 Tecnologias

- **Flask**: Framework web Python
- **Pillow**: Manipulação de imagens
- **Gunicorn**: Servidor WSGI para produção
