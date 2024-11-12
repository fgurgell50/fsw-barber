# fsw-barber
Aplicativo para Barbearia

npx create-next-app@latest fsw-barber

npm i prisma --save-dev

depois de criar as models ( as tabelas e seus campos)
npx prisma format

      POSTGRES_USER: postgres
      POSTGRES_PASSWORD: admin

npx prisma migrate dev --name init_db
para criacao das tabelass 

arquivo seed.ts

alterar o package.json e incluir
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint"
  },
  "prisma": {
    "seed": "ts-node prisma/seed.ts"
  },

  instalar
  npm i -D ts-node

  npx prisma db seed
  executa o seed
criar os dados nas tabelas no banc

  Next 
  o nome da pasta é o nome da rota
  dentro app a página page.tsx é a página principal
layout pode ser                 utilzado como rodapé ou header
  
  Todos os compenetnte sao Server Components, é executado do lado do servidor
  Um botao para interagir na tela nao é possivel
  Um estado da tela tb nao é possivel 
  utilizar o hook useState
  qdo colocamos 
  "use client" no topo da tela entao podemos usar de forma parcial Client Component
  

npm install -D prettier prettier-plugin-tailwindcss

Bibliioteca de Component
https://ui.shadcn.com/
npx shadcn@latest init

npx shadcn@latest add button
import { Button } from "@/components/ui
<Button variant="outline">Button</Button>

npx shadcn@latest add accordion 
import {
  Accordion,
  AccordionContent,
  AccordionItem,
  AccordionTrigger,
} from "@/components/ui/accordion"

<Accordion type="single" collapsible>
  <AccordionItem value="item-1">
    <AccordionTrigger>Is it accessible?</AccordionTrigger>
    <AccordionContent>
      Yes. It adheres to the WAI-ARIA design pattern.
    </AccordionContent>
  </AccordionItem>
</Accordion>

HUsky garante que sos arquivos estejam com uma formatação
Antes de ser feito o Commit é executado o link

npm i -D husky lint-staged
npx husky init

na pasta pre-commit dentro de husky 
alterar e colocar 
npx lint-staged

criar o arquivo 
.lintstagedrc.json
e colocar dentro 
{
  "*.ts?(x)": ["eslint --fix", "prettier --write"]
}

git remote add origin https://github.com/fgurgell50/fsw-barber.git
git remote -v


  git add .
  git commit -m "teste"
  Para fazer o push
  git push origin main  

11.11
  npx shadcn@latest add accordion 

  page.tsx
  Página principal

  npx shadcn@latest add input