# 📊 API de Operações Aritméticas

## Descrição

Esta é uma aplicação simples de API REST desenvolvida com **Node.js** e **Express**. A API permite realizar operações básicas de aritmética: **soma**, **subtração**, **multiplicação** e **divisão**. As operações são realizadas através de requisições HTTP POST, e a resposta é retornada no formato de texto.

## 🚀 Tecnologias Usadas

- **Node.js**: Ambiente de execução para JavaScript no lado do servidor.
- **Express**: Framework para Node.js que facilita a construção de APIs e aplicações web.
- **Body-parser**: Middleware para interpretar o corpo das requisições.

## 📡 Endpoints

### 1. Raiz da API

- **Método**: `GET`
- **Endpoint**: `/`
- **Descrição**: Retorna uma mensagem simples.
- **Resposta**: 
  ```
  Oi, mundo :-)
  ```

### 2. Soma

- **Método**: `POST`
- **Endpoint**: `/soma`
- **Descrição**: Realiza a soma de dois números.
- **Corpo da Requisição**:
  ```json
  {
    "a": <número1>,
    "b": <número2>
  }
  ```
- **Resposta**: 
  ```
  O resultado da soma de <número1> e <número2> é <resultado>
  ```

### 3. Subtração

- **Método**: `POST`
- **Endpoint**: `/subtrai`
- **Descrição**: Realiza a subtração de dois números.
- **Corpo da Requisição**:
  ```json
  {
    "a": <número1>,
    "b": <número2>
  }
  ```
- **Resposta**: 
  ```
  O resultado da subtração de <número1> e <número2> é <resultado>
  ```

### 4. Multiplicação

- **Método**: `POST`
- **Endpoint**: `/multiplica`
- **Descrição**: Realiza a multiplicação de dois números.
- **Corpo da Requisição**:
  ```json
  {
    "a": <número1>,
    "b": <número2>
  }
  ```
- **Resposta**: 
  ```
  O resultado da multiplicação de <número1> e <número2> é <resultado>
  ```

### 5. Divisão

- **Método**: `POST`
- **Endpoint**: `/divide`
- **Descrição**: Realiza a divisão de dois números. Retorna um erro se o divisor for zero.
- **Corpo da Requisição**:
  ```json
  {
    "a": <número1>,
    "b": <número2>
  }
  ```
- **Resposta**: 
  - Se `b` não for zero:
    ```
    O resultado da divisão de <número1> por <número2> é <resultado>
    ```
  - Se `b` for zero:
    ```
    Erro: Divisão por zero!
    ```

## 🛠️ Como Executar

1. **Clone o repositório**:
   ```bash
   git clone <URL-do-repositório>
   cd <diretório-do-repositório>
   ```

2. **Instale as dependências**:
   ```bash
   npm install
   ```

3. **Inicie o servidor**:
   ```bash
   node <nome-do-arquivo>.js
   ```

4. **Acesse a API**:
   O servidor estará escutando na porta **3001**. Você pode testar os endpoints usando ferramentas como **Postman** ou **cURL**.






