<p align="center">
  <img src="logo.png" width="396" height="118" alt="Winlator-Brasil Logo" />
</p>

<h1 align="center">Winlator-Brasil</h1>
<p align="center"><strong>Mod brasileiro do Winlator, adaptado e mantido com foco em desempenho, compatibilidade e acessibilidade.</strong></p>
<p align="center"><strong>Feito por <a href="https://youtube.com/@FurulipoGames">🎮 Furulipo Games</a> , <a href="https://github.com/Rhustoxx">🕹️ Rhustoxx</a>, <a href="https://github.com/mpjsilva">🏎️ Mpjsilvaa</a></strong></p>
<p align="center">
  🙏 Homenagem especial ao criador original: <a href="https://github.com/brunodev85">brunodev85</a>  
</p>

<p align="center">
  <img src="https://img.shields.io/github/downloads/winlatorbrasil/Winlator-Brasil/total?style=flat-square&logo=github&label=Downloads&color=brightgreen" alt="Total Downloads"/>
  <img src="https://img.shields.io/badge/Android-8.0%2B-green?style=flat-square&logo=android" alt="Android 8.0+"/>
  <img src="https://img.shields.io/badge/Arquitetura-arm64--v8a-blue?style=flat-square" alt="arm64-v8a"/>
  <img src="https://img.shields.io/badge/Licença-Gratuito-orange?style=flat-square" alt="Gratuito"/>
</p>

<p align="center">
  <a href="https://chat.whatsapp.com/IeH3Va7W9pzFoL2Ln3ixG1">📲 Entre para o nosso grupo no WhatsApp</a>
</p>

---

## 📦 Instalação

1. Baixe o APK mais recente em [GitHub Releases](https://github.com/winlatorbrasil/Winlator-Brasil/releases/tag/Winlator_Brasil_10.0)
2. Instale o aplicativo no seu Android.
3. Aguarde a conclusão da instalação inicial.
4. Selecione o renderizador de acordo com o seu chip — veja os requisitos abaixo.

---

## ▶️ Testes em Vídeo

* **Em breve:** Link para demonstrações reais de uso no YouTube.
* Para mais testes e dicas, confira o [canal do criador no YouTube](#).

---

## 🛠️ Dicas e Recursos Úteis

* Problemas de desempenho? Tente mudar para Box86/Box64 em **Configurações do Contêiner > Guia Avançado**.
* Para apps com .NET Framework, instale o **Wine Mono**.
* Jogos antigos podem precisar da variável `MESA_EXTENSION_MAX_YEAR=2003`.
* Use atalhos personalizados para jogos com configurações específicas.
* Para ocultar o HUD do DXVK, modifique as variáveis de ambiente (`devinfo`, `frametimes`, `gpuload`).
* Otimize jogos Unity com `-force-gfx-direct -force-d3d11-singlethread` nos argumentos.
* Habilite `MANGOHUD` (versão glibc) e `BOX64_DYNAREC_WEAKBARRIER` para melhorar desempenho.
* Use **Tela Cheia Forçada** para jogos com resolução baixa.

---

## 📋 Requisitos de Sistema

### 📱 Dispositivo

* **Android**: 8.0 ou superior
* **RAM**: Mínimo 4 GB (recomendado 6 GB)
* **Arquitetura**: arm64-v8a
* **Armazenamento**: Suporta cartão SD, com ressalvas

### 🖼️ GPU & Driver

| Driver       | Compatibilidade                                      |
| ------------ | ---------------------------------------------------- |
| **Turnip**   | Adreno 6xx e 7xx                                     |
| **Vortek**   | Todas as GPUs, incluindo Adreno 8xx e Mali           |
| **VirGL**    | GPUs variadas (funciona bem com DX9/OpenGL 3.1)      |
| **LLVMPIPE** | Somente para apps leves (disponível no Winlator 7.1) |

---

## ⚙️ Entendendo as Limitações dos Drivers (Explicação Simples)

Nem todos os celulares funcionam igual com o Winlator-Brasil. Isso depende da **GPU** (placa de vídeo do celular) e do **driver**, que age como um "tradutor" entre o jogo e o aparelho.

### 📌 Tipos comuns de GPU

| Fabricante    | Linha de GPU         | Observações                                            |
|---------------|----------------------|---------------------------------------------------------|
| **Qualcomm**  | Adreno (Snapdragon) | Melhor desempenho e compatibilidade com Turnip         |
| **ARM**       | Mali                 | Funciona com Vortek/VirGL, mas pode ter gráficos quebrados |
| **Samsung**   | Xclipse (Exynos)     | Pode funcionar com VirGL, mas ainda instável           |
| **MediaTek**  | Mali                 | Mesmo caso das GPUs Mali — pode ter bugs visuais       |

---

### 🔍 Comparando os drivers

| Driver      | Como funciona |
|-------------|---------------|
| **Turnip**  | Muito rápido, mas só funciona bem em Adreno 6xx ou 7xx. Em Adreno 8xx, pode não funcionar direito. |
| **Vortek**  | Compatível com quase todos os aparelhos. Funciona até em Mali, mas é mais lento que Turnip. |
| **VirGL**   | Ideal para jogos antigos. Funciona em quase todos os celulares, mas pode travar em jogos novos. |
| **LLVMPIPE**| Usado apenas para apps leves. Não serve para jogar. |

---

### 🧠 Explicando para qualquer um entender

Imagine que:

- O **jogo fala inglês**
- A **GPU fala português**
- O **driver é o tradutor**

Se o tradutor não entende direito o jogo ou a GPU, tudo trava, fica feio ou nem abre. Por isso, o tipo de driver e da GPU importa tanto.

---

### 💡 Qual usar?

- ✅ **Snapdragon com Adreno 6xx/7xx**: Use o **Turnip**
- 🟡 **Adreno 8xx ou Mali**: Use o **Vortek**
- 🕹️ **Jogos antigos ou celulares fracos**: Use o **VirGL**
- 📝 **Apps leves**: Use o **LLVMPIPE**

---

### 📢 Lembrete

Mesmo com boa configuração, alguns jogos podem não funcionar. Continue testando e compartilhe resultados com a comunidade!

---

## 🐞 Problemas Conhecidos

* ❌ Cartão SD pode não ser reconhecido
* ❌ Drivers OTG USB não detectam unidades
* ✅ Problemas em Adreno 735, Xinput e VirGL (glibc) já foram resolvidos

---

## ❓ FAQ – Perguntas Frequentes

### ❗ Preciso desinstalar o Winlator original?

Sim. É necessário para evitar conflitos de arquivos.

### ❗ Preciso reinstalar toda vez que sair uma atualização?

Sim, pois os contêineres não são compatíveis entre versões modificadas.

### 🆚 Qual a diferença entre o APK normal e o “Bench”?

* **Normal**: Para uso padrão.
* **Bench**: Ideal para comparações com outras versões ou múltiplas instalações.

### 🚫 Meu jogo não abre. E agora?

* Tente alterar o driver (Turnip/Vortek)
* Verifique a predefinição do Box64
* Pode ser que o jogo ainda não seja compatível.

### ⚠️ O antivírus alertou sobre vírus. É seguro?

Sim. Detecções falsas são comuns em apps que usam emulação. Todos os builds são verificados no [VirusTotal](https://www.virustotal.com/).

### 💡 Posso sugerir recursos?

Claro, mas o projeto é modificado diretamente no celular. Recursos mais avançados exigem PC.

### 💰 Posso doar para o projeto?

Agradeço muito! Mas este projeto é gratuito para todos.

---

## 👥 Créditos

* **Criador original:** [brunodev85](https://github.com/brunodev85)
* **Box86/Box64**: [ptitSeb](https://github.com/ptitSeb)
* **Wine**: [winehq.org](https://www.winehq.org)
* **Mesa3D / Turnip / VirGL**: [mesa3d.org](https://www.mesa3d.org)
* **DXVK**: [doitsujin](https://github.com/doitsujin/dxvk)
* **Outros contribuidores**: [afeimod](https://github.com/afeimod/), [MrPhryaNikFrosty](https://github.com/MrPhryaNikFrosty), [ajay9634](https://github.com/ajay9634), [ryanfortner](https://github.com/ryanfortner), [Ph42oN](https://gitlab.com/Ph42oN/dxvk-gplasync), [AlpyneDreams](https://github.com/AlpyneDreams/d8vk), [K11MCH1](https://github.com/K11MCH1/WinlatorTurnipDrivers)

---

## ❤️ Agradecimentos Finais

Muito obrigado a toda a comunidade, testers, desenvolvedores e usuários que apoiam este mod!  
A jornada continua — e tudo isso só é possível graças a vocês!

