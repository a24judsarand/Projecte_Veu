# Projecte Veu  
  
Aplicació d'escriptori amb control per veu en català, desenvolupada amb Vue.js 3 i Electron.  
  
## 🎯 Descripció  
  
El **Projecte Veu** és una aplicació d'escriptori multiplataforma que combina les tecnologies web de Vue.js amb un contenidor Electron per oferir una experiència d'usuari controlada per veu. L'aplicació demostra pràctiques modernes de desenvolupament Vue incloent registre automàtic de components, enrutament basat en fitxers i gestió d'estat reactiva, amb una interfície de comandaments de veu en català.  
  
## 🛠️ Tecnologies  
  
| Tecnologia | Versió | Propòsit |  
|------------|---------|----------|  
| **Vue.js** | 3.5.21 | Framework UI reactiu amb Composition API |  
| **Vuetify** | 3.10.1 | Biblioteca de components Material Design |  
| **Vue Router** | 4.5.1 | Enrutament client-side |  
| **Pinia** | 3.0.3 | Gestió d'estat |  
| **Electron** | 39.2.6 | Contenidor d'aplicació d'escriptori |  
| **Vite** | 7.1.5 | Eina de construcció i servidor de desenvolupament |  
  
## 🎤 Comandaments de Veu  
  
L'aplicació reconeix els següents comandaments en català:  
  
- **"saluda"** - Mostra un salutació  
- **"ajuda"** - Mostra l'ajuda  
- **"Tema"** - Canvia el tema visual  
- **"Reset"** - Reinicia la interfície  
  
## 📦 Instal·lació  
  
Instal·la les dependències amb el teu gestor de paquets preferit:  
  
 
# Amb npm  
npm init -y
npm install  
  
# Amb electron 
npm install electron --save-dev

🚀 Desenvolupament
Iniciar el servidor de desenvolupament
npm run dev
El servidor s'iniciarà a http://localhost:3000 amb recàrrega automàtica.

Construir per a producció
npm run build

Executar l'aplicació d'escriptori
npm run start

📁 Estructura del Projecte
Projecte_Veu/  
├── main.js                    # Procés principal d'Electron  
├── index.html                 # Contenidor HTML  
├── package.json              # Dependències i scripts  
├── vite.config.js            # Configuració de Vite  
├── src/  
│   ├── main.js               # Arrencada de l'aplicació Vue  
│   ├── App.vue               # Component arrel  
│   ├── pages/                # Pàgines (auto-rutes)  
│   │   └── index.vue         # Pàgina principal  
│   ├── components/           # Components (auto-registrats)  
│   │   ├── VoiceCommander.vue    # Control per veu  
│   │   ├── AppFooter.vue         # Peu de pàgina  
│   │   └── HelloWorld.vue        # Component de benvinguda  
│   ├── layouts/              # Disposicions de pàgina  
│   ├── composables/          # Funcions reutilitzables  
│   │   └── useSpeechRecognition.js  # API de reconeixement de veu  
│   ├── plugins/              # Registre de plugins Vue  
│   └── styles/               # Estils globals  
└── public/                   # Recursos estàtics  

✨ Característiques Destacades
Control per Veu: Integració amb Web Speech API per al reconeixement de comandaments en català
Auto-importació: Components i APIs de Vue s'importen automàticament
Enrutament Automàtic: Les rutes es generen a partir de l'estructura de src/pages/
Disseny Modern: Interfície Material Design amb Vuetify
Multiplataforma: Funciona a Windows, macOS i Linux gràcies a Electron
