# 🚀 **OpenHealth**

<div align="center">

**Asystent medyczny oparty na SI | Oparty na Twoich danych, działający lokalnie**

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Web-blue?style=for-the-badge" alt="Platform">
  <img src="https://img.shields.io/badge/Language-TypeScript-blue?style=for-the-badge" alt="Language">
  <img src="https://img.shields.io/badge/Framework-Next.js-black?style=for-the-badge" alt="Framework">
</p>

### 🌍 Wybierz swój język
[polski](i18n/readme/README.pl.md) | [English](README.md) | [Français](i18n/readme/README.fr.md) | [Deutsch](i18n/readme/README.de.md) | [Español](i18n/readme/README.es.md) | [한국어](i18n/readme/README.ko.md) | [中文](i18n/readme/README.zh.md) | [日本語](i18n/readme/README.ja.md)

</div>

---

<p align="center">
  <img src="/intro/openhealth.avif" alt="OpenHealth Demo">
</p>

## 🌟 Opis

> OpenHealth pomaga Ci **opanować Twoje dane medyczne**. Wykorzystując SI i informacje o Twoim stanie zdrowia,
> OpenHealth służy za prywatnego i uruchomionego lokalnie asystenta, który pomaga Ci zrozumieć i zarządzać swoim zdrowiem.

## ✨ Funkcje

<details open>
<summary><b>Główne funkcje</b></summary>

- 📊 **Centralizacja:** Połącz wszystkie swoje dane w jednym miejscu w przystępny sposób.
- 🛠️ **Analiza:** Automatycznie analizuje Twoje dane medyczne, konwertując je do ustrukuryzowanych plików.
- 🤝 **Konwersacje:** Użyj ustrukturyzowanych danych jako kontekst w swoich interakcjach z asystentem SI opartym na GPT.

</details>

## 📥 Wspierane źródła danych i modele językowe

<table>
  <tr>
    <th>Źródła, które możesz dodać</th>
    <th>Wspierane modele językowe</th>
  </tr>
  <tr>
    <td>
      • Wyniki badań krwi<br>
      • Dane kontroli medycznych<br>
      • Informacje o zdrowiu fizycznym<br>
      • Rodzinna historia chorób<br>
      • Symptomy
    </td>
    <td>
      • LLaMA<br>
      • DeepSeek-V3<br>
      • GPT<br>
      • Claude<br>
      • Gemini
    </td>
  </tr>
</table>

## 🤔 Dlaczego zbudowaliśmy OpenHealth?

> - 💡 **Twoje zdrowie jest Twoją odpowiedzialnością.**
> - ✅ Poprawne zarządzanie zdrowiem łączy **twoje dane** + **wiedzę**, zmieniając spostrzeżenia na skuteczne plany.
> - 🧠 SI służy za bezstronne narzędzie, które pokieruje Cię oraz wesprze w długoterminowym zarządzaniu swoim zdrowiem.

## 🗺️ Diagram projektu

```mermaid
graph LR
    subgraph Źródła danych zdrowotnych
        A1[Wyniki medyczne<br>Testy krwi/Diagnozy/<br>Recepty/Zdjęcia medyczne]
        A2[Platformy fitness<br>Apple Health/Google Fit]
        A3[Smart-akcesoria<br>Oura/Whoop/Garmin]
        A4[Własne dane<br>Dieta/Symptomy/<br>Rodzinna historia chorób]
    end

    subgraph Przetwarzanie danych
        B1[Parser & standardyzacja]
        B2[Unified Health Data Format]
    end

    subgraph Integracja z SI
        C1[LLM Processing<br>Komercyjne oraz lokalne modele]
        C2[Metody interakcji<br>RAG/Cache/Agenci]
    end

    A1 & A2 & A3 & A4 --> B1
    B1 --> B2
    B2 --> C1
    C1 --> C2

    style A1 fill:#e6b3cc,stroke:#cc6699,stroke-width:2px,color:#000
    style A2 fill:#b3d9ff,stroke:#3399ff,stroke-width:2px,color:#000
    style A3 fill:#c2d6d6,stroke:#669999,stroke-width:2px,color:#000
    style A4 fill:#d9c3e6,stroke:#9966cc,stroke-width:2px,color:#000
    
    style B1 fill:#c6ecd9,stroke:#66b399,stroke-width:2px,color:#000
    style B2 fill:#c6ecd9,stroke:#66b399,stroke-width:2px,color:#000
    
    style C1 fill:#ffe6cc,stroke:#ff9933,stroke-width:2px,color:#000
    style C2 fill:#ffe6cc,stroke:#ff9933,stroke-width:2px,color:#000

    classDef default color:#000
```

> **Note:** The data parsing functionality is currently implemented in a separate Python server and is planned to be migrated to TypeScript in the future.

## Getting Started

## ⚙️ How to Run OpenHealth

<details open>
<summary><b>Installation Instructions</b></summary>

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/OpenHealthForAll/open-health.git
   cd open-health
   ```

2. **Setup and Run:**
   ```bash
   # Copy environment file
   cp .env.example .env

   # Add API keys to .env file:
   # UPSTAGE_API_KEY - For parsing (You can get $10 credit without card registration by signing up at https://www.upstage.ai)
   # OPENAI_API_KEY - For enhanced parsing capabilities

   # Start the application using Docker Compose
   docker compose --env-file .env up
   ```

   For existing users, use:
   ```bash
   docker compose --env-file .env up --build
   ```

3. **Access OpenHealth:**
   Open your browser and navigate to `http://localhost:3000` to begin using OpenHealth.

> **Note:** The system consists of two main components: parsing and LLM. Currently, parsing utilizes Upstage and OpenAI APIs (which showed the best performance in our testing) with a local parser coming soon, while the LLM component can run fully locally using Ollama.

> **Note:** If you're using Ollama with Docker, make sure to set the Ollama API endpoint to: `http://docker.for.mac.localhost:11434/`

</details>

---

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=OpenHealthForAll/open-health&type=Date)](https://star-history.com/#OpenHealthForAll/open-health&Date)

---

## 🌐 Community and Support

<div align="center">

### 💫 Share Your Story & Get Updated & Give Feedback
[![AIDoctor Subreddit](https://img.shields.io/badge/r/AIDoctor-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/r/AIDoctor/)

### 📬 Contact
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/user/Dry_Steak30/)

</div>
