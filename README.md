# 🇧🇷 Expedição Brasil - Quiz e Curso EAD

Plataforma educacional gamificada sobre a História do Brasil, com módulos de aulas interativas, quizzes desafiadores com feedback didático imediato e painel completo do professor (LMS / CMS) integrado com Firebase Firestore na nuvem.

---

## 🚀 Funcionalidades

- **Módulos Históricos**:
  - Brasil Colônia (Cabral, Pau-Brasil, Açúcar, Ciclo do Ouro)
  - Brasil Império (Família Real, Independência, Lei Áurea)
  - Brasil República (Proclamação, Ciclo do Café, Brasília)
- **Gamificação Pedagógica**:
  - Quizzes desbloqueados somente após leitura completa das aulas.
  - Explicação imediata com o balão didático *"💡 Você Sabia?"*.
  - Cálculo de nota e conceito escolar (A, B, C, D).
- **Painel do Professor (Admin EAD)**:
  - Atalho de teclado: `Alt` + `Shift` + `M`
  - Relatório geral de alunos com notas e histórico.
  - Editor visual para adicionar e modificar módulos, aulas e perguntas.
  - Sincronização em tempo real com Firebase Firestore.

---

## ☁️ Conexão com Firebase

Para sincronizar o curso e as notas dos alunos na nuvem:

1. Acesse o [Firebase Console](https://console.firebase.google.com) e crie um projeto (ou use um existente).
2. Ative o **Authentication** com o provedor **Anônimo** (Anonymous).
3. Crie um banco de dados **Firestore Database** em modo de teste.
4. Adicione um App Web no Firebase e copie as credenciais para o arquivo `firebase-config.js`:
   ```javascript
   window.FIREBASE_CONFIG = {
     apiKey: "SUA_API_KEY",
     authDomain: "seu-app.firebaseapp.com",
     projectId: "seu-app",
     storageBucket: "seu-app.appspot.com",
     messagingSenderId: "...",
     appId: "..."
   };
   ```

---

## 🌐 Deploy no Vercel

Este projeto é uma aplicação estática e independente. Para publicar no Vercel:
1. Conecte o repositório GitHub `expedicao-brasil` no painel da Vercel.
2. O arquivo `index.html` e `vercel.json` estão prontos para deploy automático.
