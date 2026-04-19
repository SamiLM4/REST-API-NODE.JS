Este repositório contém exemplos práticos e códigos completos de implementações de REST APIs utilizando JavaScript, cobrindo desde conceitos fundamentais até frameworks modernos como Express.js, Next.js e NestJS.

## 📂 Estrutura do Repositório

| Pasta | Descrição |
| :--- | :--- |
| **Basic-Express-API** | API REST simples com Express.js, CRUD completo e exemplos de rotas. |
| **NextJS-API-Routes** | Implementação de rotas de API utilizando Next.js (Serverless Functions). |
| **NestJS-API** | API REST escalável e modular desenvolvida com NestJS. |
| **NodeJS-and-Express** | Código-fonte de um livro sobre Node.js e Express.js. |
| **react-native-restapi-example** | Exemplo de aplicação mobile em React Native consumindo uma REST API. |

## 🚀 Exemplos Detalhados

### 1. Express.js - CRUD Completo
Exemplo de API CRUD funcional com:
- Rotas GET, POST, PUT e DELETE.
- Interação com banco de dados MySQL.
- Estrutura modular com controllers e routes.

**Exemplo de rota (GET /products):**
```javascript
router.get('/products', (req, res) => {
    // Implementação da lógica de listagem de produtos
});
```

### 2. Next.js - API Routes
Demonstração de como criar rotas de API dentro de um projeto Next.js.

**Exemplo de arquivo de rota (pages/api/hello.js):**
```javascript
export default (req, res) => {
  res.status(200).json({ name: 'John Doe' });
};
```

### 3. NestJS - API Escalável
Estrutura completa de API com NestJS, incluindo:
- Módulos, Controllers e Services.
- Validação de dados com Pipes.
- Autenticação e Autorização.

**Exemplo de Controller:**
```typescript
@Controller('products')
export class ProductsController {
  constructor(private readonly productsService: ProductsService) {}

  @Post()
  async create(@Body() createProductDto: CreateProductDto) {
    return this.productsService.create(createProductDto);
  }
}
```

## 🛠️ Como Utilizar

### Pré-requisitos
- Node.js instalado
- npm ou yarn
- Para projetos NestJS: TypeScript

### Instalação
1. Clone o repositório:
```bash
git clone <url-do-repositório>
cd <pasta-do-exemplo>
```

2. Instale as dependências:
```bash
npm install
# ou
yarn install
```

### Execução
- **Express:**
```bash
npm start
```

- **Next.js:**
```bash
npm run dev
```

- **NestJS:**
```bash
npm run start:dev
```

## 📚 Conhecimentos Abrangidos
- CRUD (Create, Read, Update, Delete)
- HTTP Methods (GET, POST, PUT, DELETE)
- JSON Data Format
- RESTful API Principles
- API Authentication
- Database Integration (MySQL)
- Server-Side Rendering (SSR) vs Client-Side Rendering (CSR)
- Microservices Architecture
- TypeScript
