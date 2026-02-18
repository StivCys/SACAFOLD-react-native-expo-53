App

Aplicativo mobile + web desenvolvido com Expo SDK, utilizando NativeWind para estilização com Tailwind e preparado para integração com Supabase como backend.

🚀 Stack Tecnológica
Core

Expo ~53.0.27

React 19.0.0

React Native 0.79.6

TypeScript ~5.8.3

Web Support

react-dom 19.0.0

react-native-web ^0.20.0

@expo/metro-runtime ~5.0.5

Estilização

NativeWind ^2.0.11

TailwindCSS ^3.3.2

📦 Scripts Disponíveis
npm start        # Inicia Expo
npm run android  # Abre no Android
npm run ios      # Abre no iOS
npm run web      # Abre no navegador

🏗 Estrutura Atual do Projeto
petshop-app/
│
├── App.tsx
├── index.ts
├── babel.config.js
├── tailwind.config.js
├── package.json
│
├── assets/
├── node_modules/

🎨 Estilização

O projeto utiliza NativeWind v2 (compatível com SDK 53).

Exemplo de uso:

<View className="flex-1 items-center justify-center bg-green-500">
  <Text className="text-white text-xl font-bold">
    PetShop App
  </Text>
</View>

Configuração do Babel
module.exports = function(api) {
  api.cache(true);
  return {
    presets: ["babel-preset-expo"],
    plugins: ["nativewind/babel"],
  };
};

Configuração do Tailwind
module.exports = {
  content: ["./App.{js,jsx,ts,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

🌐 Backend

O backend será implementado com Supabase.

Planejado para suportar:

Configuração dinâmica de cores

Banner dinâmico

Nome da loja

Sistema multi-loja (futuro)

🖥 Plataformas Suportadas

✅ Android

✅ iOS

✅ Web

🔧 Requisitos

Node.js 20+

npm 10+

Expo CLI via npx

Verificar versões:

node -v
npm -v
npx expo --version

🧠 Arquitetura Atual

Expo com new architecture habilitado

NativeWind v2 para evitar conflitos com React 19

Configuração limpa de Babel

Web totalmente funcional

📌 Observações Técnicas

NativeWind v4 não foi utilizado devido a conflitos com SDK 53 + React 19.

O projeto está configurado com versões estáveis e compatíveis.

Web depende de react-dom e react-native-web instalados.


🔜 Próximos Passos

Integração com Supabase

Tema dinâmico via backend

Estrutura de pastas profissional

Componentização (Button, Card, Input)

Sistema multi-loja

Se quiser, posso gerar também:

📄 README em formato mais corporativo

📦 README preparado para GitHub (com badges)

🏗 Documento de arquitetura técnica

📊 Roadmap do projeto

🧩 Modelo SaaS do PetShop
