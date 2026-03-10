# 1. Planejamento do projeto

### 1.1 Definição de conteúdo

* Definir seções da landing page:

  * Hero (nome do restaurante + chamada)
  * Cardápio do mês
  * Sobre a equipe
  * Informações do restaurante
  * Formulário de sugestões
  * Redes sociais
  * Contato
* Definir textos institucionais.
* Definir links das redes sociais.
* Definir número de WhatsApp oficial.

### 1.2 Identidade visual

* Definir:

  * cores principais
  * tipografia
  * estilo de imagens
* Criar logo simples caso não exista.
* Definir ícones.

### 1.3 Estrutura inicial do projeto

* Criar repositório Git.
* Definir stack:

  * Frontend: **React ou Vue**
  * Backend: **Node.js (Express) ou Flask**
* Criar estrutura de pastas.

---

# 2. Desenvolvimento Frontend (React ou Vue)

## 2.1 Configuração inicial

* Criar projeto com:

  * React → Vite ou Next
  * Vue → Vite
* Instalar dependências principais:

  * axios
  * biblioteca de ícones
  * biblioteca de UI (opcional)

# 3. Construção da Landing Page

## 3.1 Seção Hero

* Nome do restaurante **Sabor e Cia**
* Pequena descrição
* Botão "Ver Cardápio"
* Imagem de fundo relacionada a comida.

---

## 3.2 Cardápio do mês

Funcionalidade principal.

Tarefas:

* Criar botão **"Ver Cardápio do Mês"**
* Abrir PDF em:

  * nova aba
  * modal
* Alternativa:

  * botão **baixar PDF**

Extras opcionais:

* Mostrar mês atual automaticamente.

---

## 3.3 Sobre a equipe

Criar seção com:

* foto da equipe ou da cozinha
* pequeno texto:

  * missão
  * atendimento no campus

---

## 3.4 Informações do restaurante

Exibir:

* horário de funcionamento
* localização (refeitório do campus)
* tipos de serviço:

  * almoço
  * lanches
  * bebidas
  * sorvete

---

## 3.5 Redes sociais

Adicionar ícones:

* Instagram
* Facebook (se houver)

Links externos.

---

## 3.6 Botão flutuante do WhatsApp

Implementar:

* botão fixo no canto inferior
* link:

```
https://wa.me/NUMERO
```

Estilo:

* verde
* ícone WhatsApp

---

## 3.7 Formulário de sugestões

Campos:

* nome (opcional)
* email (opcional)
* mensagem

Botão:

```
Enviar sugestão
```

Após envio:

* mostrar mensagem de sucesso.

---

# 4. Responsividade (Mobile First)

Tarefas:

* layout mobile primeiro
* adaptar para:

  * celular
  * tablet
  * desktop

Testar em:

* Chrome mobile
* DevTools

---

# 5. Transformar em PWA

Funcionalidades:

* instalar como app
* funcionar offline parcialmente

Tarefas:

* adicionar `manifest.json`
* configurar service worker
* definir:

```
nome
ícone
cor do tema
modo standalone
```

Bibliotecas possíveis:

React

* vite-plugin-pwa

Vue

* vite-plugin-pwa

---

# 6. Backend (Node.js ou Flask)

O backend será simples.

Objetivo principal:

* receber sugestões do formulário.

---

# Opção 1 — Node.js (recomendado)

Stack:

* Node.js
* Express
* Nodemailer

Endpoints:

```
POST /api/sugestao
```

Função:

* receber dados do formulário
* enviar email para administração
* salvar sugestão (opcional).

---

# Opção 2 — Flask

Stack:

* Flask
* Flask-Mail

Endpoint:

```
POST /api/sugestao
```

Função:

* receber sugestão
* enviar email.
