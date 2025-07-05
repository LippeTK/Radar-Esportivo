# Radar de futebol

Radar de partidas de futebol em tempo real, com integração entre frontend e backend próprio via rotas REST.
Consumo de API externa com Node, atualizações dinâmicas via polling, cache com Redis e interface responsiva em React.

## Tecnologias

### 🖥️ Frontend

- **React.js** com **Vite**
- **React Router DOM** para navegação entre páginas
- Requisições assíncronas ao backend via `axios`
- CSS **responsivo**, adaptadando a interface para telas menores

### ⚙️ Backend

- **Node.js** com **Express**
- Estrutura com `controller` e `routes`
- Integração com **API externa** da [api-football](https://www.api-football.com/)
- Atualização de dados com **polling**
- Uso de **Redis** para cache e redução de requisições repetidas

## Funcionalidades

- Lista de partidas ao vivo
- Detalhamento completo da partida:
  - Placar em tempo real
  - Tempo de jogo
  - Escalações
  - Eventos
  - Estatísticas

## Sobre a API

Este projeto utiliza a [API da api-football](https://www.api-football.com/) para obter dados em tempo real de partidas de futebol.

⚠️ **Atenção:** a API requer uma chave de acesso (API Key), que atualmente está vinculada a um plano pago.  
Por isso, o projeto **não funcionará corretamente sem uma chave válida**.

Caso deseje testar localmente, você pode:

- Solicitar acesso à API no site oficial
- Criar `.env` com base no `.env.example`

A estrutura do código está preparada para funcionar assim que uma chave for fornecida no `.env`.

## 🛠️ Como rodar localmente

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/radar.git

   ```

2. Instale as dependências:

   cd backend && npm install

   cd ../frontend && npm install

3. Crie o arquivo .env na pasta backend com sua chave da API.

4. Rode o backend e o frontend separadamente:

```
  cd backend
  npm start
  cd ../frontend
  npm run dev
```

## 📸 Preview

Quer ver o projeto em ação? Confira **[aqui](https://imgur.com/a/6acBmpG)**!

Desenvolvido por
Felipe Carvalho
