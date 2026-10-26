<div align="center">

# Bécaye Doumbouya
### Lead Backend Engineer & Distributed Systems Architect

[![Portfolio](https://img.shields.io/badge/Portfolio-Vercel-black?style=for-the-badge&logo=vercel&logoColor=white)](https://mon-portfolio-five-livid.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Becaye_Doumbouya-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/becaye-doumbouya-b90947411/)
[![GitHub](https://img.shields.io/badge/GitHub-HYPNOTYZEDCHART-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/HYPNOTYZEDCHART)
[![Email](https://img.shields.io/badge/Contact-doumbiabecaye7%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:doumbiabecaye7@gmail.com)

<br/>

```
Architecturant des systèmes résilients, des moteurs de paiement FinTech et des flux temps réel à haute concurrence.
```

</div>

---

### ⚡ Profil & Pôle d'Expertise

Principal Backend Engineer concevant des architectures distribuées hautement scalables, avec un accent intransigeant sur l'intégrité financière (ACID), la sécurité DevSecOps et le streaming temps réel.

* **Systèmes Financiers & Séquestre (FinTech)** : Orchestration de workflows transactionnels complexes, intégrations Wave & Orange Money (Max It), réconciliation de webhooks cryptographiques (HMAC SHA-256) et zéro perte de centime FCFA.
* **Moteurs Événementiels & Temps Réel** : Passerelles WebSockets à faible latence (Socket.io), gestion des salles de streaming, négociation bilatérale asynchrone et diffusion flash.
* **Clean Architecture & Multi-Tenant** : Conception modulaire sous NestJS 11 / Node.js, ORM Prisma 7, bases de données relationnelles optimisées (MySQL 8 / PostgreSQL) avec isolation stricte des données par tenant.

---

### 🛠️ Stack Technique de Production

<div align="center">

#### Backend & Core Runtime
![NestJS](https://img.shields.io/badge/NestJS_11-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript_5-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js_22-339933?style=flat-square&logo=node.js&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io_4-010101?style=flat-square&logo=socket.io&logoColor=white)
![RxJS](https://img.shields.io/badge/RxJS-B7178C?style=flat-square&logo=reactivex&logoColor=white)

#### Base de Données & Persistance
![Prisma](https://img.shields.io/badge/Prisma_7-2D3748?style=flat-square&logo=prisma&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL_8-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)

#### DevOps, Cloud & Déploiement
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Clever Cloud](https://img.shields.io/badge/Clever_Cloud-2E86DE?style=flat-square&logoColor=white)
![Render](https://img.shields.io/badge/Render_Cloud-46E3B7?style=flat-square&logo=render&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

#### Sécurité, Assurance Qualité & API
![JWT](https://img.shields.io/badge/JWT_Auth-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![Jest](https://img.shields.io/badge/Jest_E2E-C21325?style=flat-square&logo=jest&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger_OpenAPI-85EA2D?style=flat-square&logo=swagger&logoColor=black)
![OWASP](https://img.shields.io/badge/OWASP_Hardened-000000?style=flat-square&logo=owasp&logoColor=white)

</div>

---

### 🚀 Projet Phare : [OpenBoutik API](https://github.com/OpenBoutik-Team/openboutik-api)
> **Moteur E-Commerce & Marketplace FinTech Sécurisée (Afrique de l'Ouest)**  
> *Rôle : Lead Backend Engineer & System Architect (Dev 3)*

```mermaid
graph LR
    subgraph Clients
        Web[Marketplace Next.js]
        Admin[Seller SaaS Next.js]
    end

    subgraph API Core [OpenBoutik API - NestJS 11]
        Auth[Guards JWT / RBAC]
        Escrow[Séquestre Wave / OM]
        Wakhale[Négociation Wakhale]
        LiveWS[Passerelle /streams]
    end

    subgraph Infrastructure
        MySQL[(MySQL 8 - Clever Cloud)]
        Deploy[Render Production Engine]
    end

    Web & Admin --> Auth
    Auth --> Escrow & Wakhale & LiveWS
    Escrow & Wakhale --> MySQL
    LiveWS -.-> Web
    API Core -.-> Deploy
```

#### Réalisations Techniques Majeures sur OpenBoutik :
* **Moteur de Séquestre Financier Garanti (Escrow)** :
  * Verrouillage atomique des fonds en FCFA via Wave & Orange Money dans des transactions `$transaction`.
  * Rapprochement strict des webhooks externes avec validation d'empreinte HMAC SHA-256 et clés d'idempotence uniques pour prévenir tout double débit.
  * Déblocage sous condition de confirmation de livraison ou d'arbitrage sécurisé.
* **Négociation Interactive « Wakhale »** :
  * Machine à états finis bilatérale asynchrone (`PENDING`, `ACCEPTED`, `REJECTED`, `COUNTER_OFFERED`, `EXPIRED`).
  * Génération cryptographique de bons de réduction exclusifs à usage unique dès accord entre les parties.
* **Passerelle Live Shopping & Streaming Temps Réel** :
  * Namespace WebSockets dédié `/streams` gérant l'interaction vidéo temps réel (format Reels/TikTok).
  * Diffusion instantanée d'épingles produits flash avec fenêtres de commande atomiques.
* **Résilience & Assurance Qualité** :
  * Suite complète de tests unitaires, E2E, stress tests de concurrence et scénarios Chaos Monkey.
  * Protection stricte Anti-IDOR, rate-limiting Throttler et validation schématique intégrale (Anti-Mass Assignment).

---

### 📊 Activité & Métriques GitHub

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=HYPNOTYZEDCHART&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" width="48%" alt="GitHub Stats" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HYPNOTYZEDCHART&layout=compact&theme=tokyonight&hide_border=true" width="48%" alt="Top Languages" />

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=HYPNOTYZEDCHART&theme=tokyonight&hide_border=true" width="97%" alt="GitHub Streak" />

</div>

---

### 📬 Entrer en Contact

* **Email Pro** : [doumbiabecaye7@gmail.com](mailto:doumbiabecaye7@gmail.com)
* **LinkedIn** : [linkedin.com/in/becaye-doumbouya-b90947411](https://www.linkedin.com/in/becaye-doumbouya-b90947411/)
* **Portfolio en Ligne** : [mon-portfolio-five-livid.vercel.app](https://mon-portfolio-five-livid.vercel.app/)
* **Localisation** : Dakar, Sénégal — Disponible pour opportunités Senior Backend / Architecte Distribué (Remote / Hybride)
