# Genius - A Modern Next.js 14 SaaS AI Platform.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![License](https://img.shields.io/badge/React.js-v18.2.0-blue.svg)](https://opensource.org/licenses/MIT)
[![Next.js](https://img.shields.io/badge/Next.js-v13.4.12-blueviolet.svg)](https://nextjs.org/)
[![OpenAI](https://img.shields.io/badge/OpenAI-API-yellow.svg)](https://openai.com/)
[![Replicate](https://img.shields.io/badge/Replicate-v0.12.3-orange.svg)](https://replicate.ai/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-v3.3.3-blue.svg)](https://tailwindcss.com/)
[![Prisma](https://img.shields.io/badge/Prisma-v5.0.0-lightgrey.svg)](https://prisma.io/)
[![Stripe](https://img.shields.io/badge/Stripe-API%20v12.16.0-green.svg)](https://stripe.com/)


![Genius - A Modern Next.js 14 SaaS AI Platform.](/.github/images/img_main.png "Genius - A Modern Next.js 14 SaaS AI Platform.")

AI-SaaS is an advanced and adaptable Software-as-a-Service (SaaS) application that harnesses the capabilities of cutting-edge technologies, including Next.js, OpenAI, Replicate, Tailwind CSS, Prisma, and Stripe. The primary goal of this application is to empower users by offering AI-powered services that facilitate easy access and utilization of artificial intelligence in their projects and workflows.

## Features

- **AI Services**: AI-SaaS provides an extensive array of AI services, including conversation, code generation, image generation, music generation, and video generation. These services are accessible through an intuitive and user-friendly interface.

- **Next.js**: AI-SaaS is built on the Next.js framework, offering server-side rendering, routing, and other essential features out of the box. This ensures superior performance and search engine optimization (SEO) for the application.

- **OpenAI Integration**: The application seamlessly integrates with OpenAI's powerful AI models and APIs, enabling users to leverage state-of-the-art AI capabilities. From generating human-like text to answering questions, AI-SaaS harnesses the full potential of OpenAI.

- **Replicate**: AI-SaaS employs Replicate to enhance model reproducibility and facilitate seamless experimentation with various AI models. This ensures the AI models used in the application are robust and reliable.

- **Tailwind CSS**: The UI of AI-SaaS is meticulously styled using Tailwind CSS, a utility-first CSS framework. This enables easy customization and consistent design throughout the application.

- **Prisma**: The application utilizes Prisma as its ORM (Object-Relational Mapping) tool, simplifying database access and management. This enhances the efficiency of handling user data and preferences.

- **Stripe Integration**: AI-SaaS seamlessly incorporates Stripe for secure and efficient payment processing. Users can subscribe to premium plans and access additional AI services based on their subscription level.

## Screenshots

![Modern UI/UX](/.github/images/img1.png "Modern UI/UX")

![Conversation Page](/.github/images/img2.png "Conversation Page")

![Image Generation](/.github/images/img3.png "Image Generation")

![Code Generation](/.github/images/img4.png "Code Generation")

<!-- Table of Contents -->
<details>

<summary>

# :notebook_with_decorative_cover: Table of Contents

</summary>

- [Folder Structure](#bangbang-folder-structure)
- [Getting Started](#toolbox-getting-started)
- [Screenshots](#camera-screenshots)
- [Tech Stack](#gear-tech-stack)
- [Stats](#wrench-stats)
- [Contribute](#raised_hands-contribute)
- [Acknowledgements](#gem-acknowledgements)
- [Buy Me a Coffee](#coffee-buy-me-a-coffee)
- [Follow Me](#rocket-follow-me)
- [Learn More](#books-learn-more)
- [Deploy on Vercel](#page_with_curl-deploy-on-vercel)
- [Give A Star](#star-give-a-star)
- [Star History](#star2-star-history)
- [Give A Star](#star-give-a-star)

</details>

## :bangbang: Folder Structure

Here is the folder structure of this app.

<!--- FOLDER_STRUCTURE_START --->
```bash
ai-saas/
  |- app/
    |-- (auth)/
    |-- (dashboard)/
    |-- (landing)/
    |-- api/
    |-- apple-icon.png
    |-- favicon.ico
    |-- globals.css
    |-- icon1.png
    |-- icon2.png
    |-- layout.tsx
  |- components/
    |-- ui/
    |-- bot-avatar.tsx
    |-- crisp-chat.tsx
    |-- empty.tsx
    |-- free-counter.tsx
    |-- heading.tsx
    |-- landing-content.tsx
    |-- landing-footer.tsx
    |-- landing-hero.tsx
    |-- landing-navbar.tsx
    |-- loader.tsx
    |-- mobile-sidebar.tsx
    |-- navbar.tsx
    |-- pro-modal.tsx
    |-- sidebar.tsx
    |-- subscription-button.tsx
    |-- user-avatar.tsx
  |- config/
    |-- index.ts
  |- constants/
    |-- index.ts
  |- hooks/
    |-- use-pro-modal.tsx
  |- lib/
    |-- api-limit.ts
    |-- db.ts
    |-- stripe.ts
    |-- subscription.ts
    |-- utils.ts
  |- prisma/
    |-- schema.prisma
  |- providers/
    |-- crisp-provider.tsx
    |-- modal-provider.tsx
    |-- toaster-provider.tsx
  |- public/
  |- schemas/
    |-- index.ts
  |- .env.example
  |- .env/.env.local
  |- .eslintrc.json
  |- .gitignore
  |- bun.lock
  |- components.json
  |- environment.d.ts
  |- middleware.ts
  |- netlify.toml
  |- next.config.js
  |- package.json
  |- postcss.config.js
  |- tailwind.config.ts
  |- tsconfig.json
```
<!--- FOLDER_STRUCTURE_END --->

<br />


## :toolbox: Getting Started

1. Make sure **Git** and **NodeJS** is installed.
2. Clone this repository to your local computer.
3. Create `.env` file in **root** directory.
4. Contents of `.env`:

### 5. Clerk Authentication Keys

- Visit the Clerk dashboard: [https://clerk.dev](https://clerk.dev)
- Log in to your Clerk account or sign up if you don't have one.
- Go to the "Projects" section and select your project.
- Navigate to the "API Keys" tab.
- Copy the "Publishable Key" and replace `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY` in the `.env.local` file with the copied key.
- Copy the "Secret Key" and replace `CLERK_SECRET_KEY` in the `.env.local` file with the copied key.

### 6. OpenAI API Key

Visit [OpenAI](https://platform.openai.com/signup/) and sign up for an account. Once registered, you can find your API key in the API section of your account settings. Copy the key and set it as the `OPENAI_API_KEY` in your project's environment.

### 7. Replicate API Token

Sign up or log in to [Replicate](https://replicate.ai/). Once logged in, navigate to your account settings, and you'll find your API token. Copy the token and set it as the `REPLICATE_API_TOKEN` in your project's environment.

### 8. Aiven Database URL

If you don't have an Aiven account, sign up [here](https://aiven.io/). After creating an account, set up a MySQL database. In the Aiven dashboard, find your database connection details and construct the `DATABASE_URL` in the following format:


### 9. Stripe API and Webhook Keys

For Stripe, sign up or log in to your [Stripe Dashboard](https://dashboard.stripe.com/register). Once logged in, go to Developers > API keys to find your API secret key and webhook secret. Set them as `STRIPE_API_SECRET_KEY` and `STRIPE_WEBHOOK_SECRET` in your project's environment.

### 10. App Base URL

Set the base URL of your application as `NEXT_PUBLIC_APP_URL` in your project's environment.


### 11. Crisp Website ID

Sign up on [Crisp](https://crisp.chat/en/) and create a website. Once created, find your website ID in the Crisp dashboard and set it as `NEXT_PUBLIC_CRISP_WEBSITE_ID` in your project's environment.


12. Open terminal in root directory. Run `npm install --legacy-peer-deps` or `yarn install --legacy-peer-deps`.

13. Now app is fully configured 👍 and you can start using this app using either one of `npm run dev` or `yarn dev`.

**NOTE:** Please make sure to keep your API keys and configuration values secure and do not expose them publicly.

## :camera: Screenshots:

![Modern UI/UX](/.github/images/img1.png "Modern UI/UX")

![Conversation Page](/.github/images/img2.png "Conversation Page")

![Image Generation](/.github/images/img3.png "Image Generation")

![Code Generation](/.github/images/img4.png "Code Generation")

## :gear: Tech Stack

[![React JS](https://skillicons.dev/icons?i=react "React JS")](https://react.dev/ "React JS") [![Next JS](https://skillicons.dev/icons?i=next "Next JS")](https://nextjs.org/ "Next JS") [![Typescript](https://skillicons.dev/icons?i=ts "Typescript")](https://www.typescriptlang.org/ "Typescript") [![Tailwind CSS](https://skillicons.dev/icons?i=tailwind "Tailwind CSS")](https://tailwindcss.com/ "Tailwind CSS") [![Netlify](https://skillicons.dev/icons?i=netlify "Netlify")](https://netlify.app/ "Netlify") [![Prisma](https://skillicons.dev/icons?i=prisma "Prisma")](https://prisma.io/ "Prisma") [![MySQL](https://skillicons.dev/icons?i=mysql "MySQL")](https://mysql.com/ "MySQL")

## :raised_hands: Contribute

You might encounter some bugs while using this app. You are more than welcome to contribute. Just submit changes via pull request and I will review them before merging. Make sure you follow community guidelines.

## :gem: Acknowledgements

Useful resources and dependencies that are used in Genius.

- Thanks to CodeWithAntonio: https://codewithantonio.com/
<!--- DEPENDENCIES_START --->
- [@clerk/nextjs](https://www.npmjs.com/package/@clerk/nextjs): ^4.31.5
- [@hookform/resolvers](https://www.npmjs.com/package/@hookform/resolvers): ^3.10.0
- [@prisma/client](https://www.npmjs.com/package/@prisma/client): ^5.8.0
- [@radix-ui/react-avatar](https://www.npmjs.com/package/@radix-ui/react-avatar): ^1.1.11
- [@radix-ui/react-dialog](https://www.npmjs.com/package/@radix-ui/react-dialog): ^1.1.15
- [@radix-ui/react-label](https://www.npmjs.com/package/@radix-ui/react-label): ^2.1.8
- [@radix-ui/react-progress](https://www.npmjs.com/package/@radix-ui/react-progress): ^1.1.8
- [@radix-ui/react-select](https://www.npmjs.com/package/@radix-ui/react-select): ^2.2.6
- [@radix-ui/react-slot](https://www.npmjs.com/package/@radix-ui/react-slot): ^1.2.4
- [@types/node](https://www.npmjs.com/package/@types/node): ^25.2.3
- [@types/react](https://www.npmjs.com/package/@types/react): ^19.2.14
- [@types/react-dom](https://www.npmjs.com/package/@types/react-dom): ^19.2.3
- [autoprefixer](https://www.npmjs.com/package/autoprefixer): ^10.4.24
- [axios](https://www.npmjs.com/package/axios): ^1.13.5
- [class-variance-authority](https://www.npmjs.com/package/class-variance-authority): ^0.7.1
- [clsx](https://www.npmjs.com/package/clsx): ^2.1.1
- [crisp-sdk-web](https://www.npmjs.com/package/crisp-sdk-web): ^1.0.27
- [eslint](https://www.npmjs.com/package/eslint): ^8
- [eslint-config-next](https://www.npmjs.com/package/eslint-config-next): 14.0.4
- [lucide-react](https://www.npmjs.com/package/lucide-react): ^0.574.0
- [next](https://www.npmjs.com/package/next): 15.5.10
- [openai](https://www.npmjs.com/package/openai): ^6.22.0
- [postcss](https://www.npmjs.com/package/postcss): ^8
- [prisma](https://www.npmjs.com/package/prisma): ^5.8.0
- [react](https://www.npmjs.com/package/react): ^19.2.4
- [react-dom](https://www.npmjs.com/package/react-dom): ^19.2.4
- [react-hook-form](https://www.npmjs.com/package/react-hook-form): ^7.71.1
- [react-markdown](https://www.npmjs.com/package/react-markdown): ^10.1.0
- [replicate](https://www.npmjs.com/package/replicate): ^0.25.2
- [sonner](https://www.npmjs.com/package/sonner): ^2.0.7
- [stripe](https://www.npmjs.com/package/stripe): ^20.3.1
- [tailwind-merge](https://www.npmjs.com/package/tailwind-merge): ^2.6.1
- [tailwindcss](https://www.npmjs.com/package/tailwindcss): ^3.3.0
- [tailwindcss-animate](https://www.npmjs.com/package/tailwindcss-animate): ^1.0.7
- [typescript](https://www.npmjs.com/package/typescript): ^5.9.3
- [typewriter-effect](https://www.npmjs.com/package/typewriter-effect): ^2.22.0
- [zod](https://www.npmjs.com/package/zod): ^4.3.6
- [zustand](https://www.npmjs.com/package/zustand): ^5.0.11

## Getting Started

To run AI-SaaS locally, follow these steps:

1. **Clone the repository**:

```bash
git clone https://github.com/ayusshrathore/ai-saas.git
cd ai-saas
```

2. **Install dependencies**:

```bash
npm install
# or
yarn install
```

3. **Configure environment variables**:

To ensure proper functionality, set up environment variables for API keys and other sensitive information. Create a `.env` file in the root directory and populate it with the necessary variables. For reference, consult the `.env.example` file for the required variables.

4. **Run the application**:

```bash
npm run dev
# or
yarn dev
```

The application should now be running locally at `http://localhost:3000`.

## Deployment

AI-SaaS can be deployed to various hosting platforms that support Next.js applications. Before deployment, make sure you have configured the necessary environment variables for production.

## Contributions

Contributions to AI-SaaS are highly appreciated! If you encounter any bugs or have suggestions for new features, please feel free to open an issue or submit a pull request.

When contributing, adhere to the existing code style and include comprehensive test cases for the new features.

## License

AI-SaaS is released under the [MIT License](https://opensource.org/licenses/MIT).

## Acknowledgments

AI-SaaS is built with the invaluable support and integration of several open-source projects and technologies. I extend my gratitude to the developers and maintainers of Next.js, OpenAI, Replicate, Tailwind CSS, Prisma, and Stripe for their significant contributions to the development community.
